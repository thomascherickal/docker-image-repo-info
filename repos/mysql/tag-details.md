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
$ docker pull mysql@sha256:7a3a7b7a29e6fbff433c339fc52245435fa2c308586481f2f92ab1df239d6a29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:208315e5f89d822547065fc4e29433e23cd135289342c200407b658e4c651618
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154848607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b43c6af2ad08d95cdcb415d245446909a6cbc1875604c48c4325972e5b00442`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:32:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 17 Nov 2021 10:32:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:32:58 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 10:33:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 10:33:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 10:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:33:29 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 17 Nov 2021 10:34:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 17 Nov 2021 10:34:10 GMT
ENV MYSQL_VERSION=5.7.36-1debian10
# Wed, 17 Nov 2021 10:34:11 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 17 Nov 2021 10:34:39 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 17 Nov 2021 10:34:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 17 Nov 2021 10:34:41 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 17 Nov 2021 10:34:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 17 Nov 2021 10:34:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 10:34:43 GMT
EXPOSE 3306 33060
# Wed, 17 Nov 2021 10:34:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76a7eb51ffd66492d1e2fae9037d992666e4f0b1fa0a33b62c1de3037c17406`  
		Last Modified: Wed, 17 Nov 2021 10:36:04 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258223f927e4301d4af97e9cfda9d928a9571fff93b0fdb8306cea7478e20a16`  
		Last Modified: Wed, 17 Nov 2021 10:36:05 GMT  
		Size: 4.2 MB (4179250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2c75386df9e05399af79ae74eed16fbd80524032273f41b9fb30c9eb5fd11c`  
		Last Modified: Wed, 17 Nov 2021 10:36:03 GMT  
		Size: 1.4 MB (1419452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e92e4046c9d1ef967aef94e50a2d6731427561436bfe693ebc7d31ac198c52`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5845c7315445bc6fdaadd999741235e564b2d0c2329c7ac20d6bbc018d693e8`  
		Last Modified: Wed, 17 Nov 2021 10:36:06 GMT  
		Size: 13.4 MB (13448643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0401123a9bb1165a0c29b245575aaa8a3b918a8e9462b6b2922e688554cc4a`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2724b2da64fdec0b649e0336c8a5596b5ead25d59960382dd200af6e3c326277`  
		Last Modified: Wed, 17 Nov 2021 10:36:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a7e9e325c461f936592cb8a83ffd470b41726578d7007b8ccea35c580795c`  
		Last Modified: Wed, 17 Nov 2021 10:36:49 GMT  
		Size: 108.6 MB (108637946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5fd9c3683d5de4f54dff3476c2692c6a09de5c4072e58c086e61ece1645ca5`  
		Last Modified: Wed, 17 Nov 2021 10:36:33 GMT  
		Size: 5.5 KB (5540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e35f83a12e9cb1af2b4d08665e9958d08c4f08399977766e57003c6a28575d0`  
		Last Modified: Wed, 17 Nov 2021 10:36:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:740eb9fb4fdedfa9edb60c656db104f7cc497f0aab55a8df412d51e73a0615ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:8bd695def30f2f4a32774a3233f70709e1c5046efa21b40f0d2a8475fb7bbe08
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102971684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10de32843f9157f341f3e742640b49a702ef644f78b4ace43deff5f94ae3c063`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:38 GMT
ADD file:2868c3af63afe6b8aadac07b8776e5468a3ed135fd84ad22df15e48f0610c7ba in / 
# Wed, 17 Nov 2021 02:22:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:34:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 17 Nov 2021 10:35:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:35:00 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 10:35:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 10:35:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 10:35:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:35:24 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 17 Nov 2021 10:35:24 GMT
ENV MYSQL_MAJOR=5.6
# Wed, 17 Nov 2021 10:35:24 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Wed, 17 Nov 2021 10:35:25 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Wed, 17 Nov 2021 10:35:41 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 17 Nov 2021 10:35:42 GMT
VOLUME [/var/lib/mysql]
# Wed, 17 Nov 2021 10:35:42 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 17 Nov 2021 10:35:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 17 Nov 2021 10:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 10:35:44 GMT
EXPOSE 3306
# Wed, 17 Nov 2021 10:35:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89166b5eeae47d8c878cb88f20cc67eda2a550a697f4be317c7b7abea566b76f`  
		Last Modified: Wed, 17 Nov 2021 02:29:32 GMT  
		Size: 22.5 MB (22527686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73631a7ee13b400e10866868fbf0667fa1827689c8112ded7262f0f8d7a46ad0`  
		Last Modified: Wed, 17 Nov 2021 10:37:07 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f287d5f3290c68f206c6ddd3790534d98068b9b5f7889d69228c1fbd56b40279`  
		Last Modified: Wed, 17 Nov 2021 10:37:07 GMT  
		Size: 4.5 MB (4503836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a24ae08d840d53c9137ef617a35fd4078c51406a05dfab9083ea1ca3d46f08d`  
		Last Modified: Wed, 17 Nov 2021 10:37:05 GMT  
		Size: 1.4 MB (1412228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b749bd83c0e68067e56f2b48c1cb8a30efc5d6b990a46f95476a3128c8285a3`  
		Last Modified: Wed, 17 Nov 2021 10:37:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69787256215e7a608a1f37f4349c6243d104e9254f08f027bf0a36b905f603a6`  
		Last Modified: Wed, 17 Nov 2021 10:37:09 GMT  
		Size: 10.2 MB (10225786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d273eb6cdd86afd2ed0017bdef8b7d3d2308c9cd56075ff9854b3669ed8717f`  
		Last Modified: Wed, 17 Nov 2021 10:37:02 GMT  
		Size: 20.0 KB (19999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a897b78ad8f86b2fc4bed220a614a205f9fcdf0d75f968ddc1b25483eeb82e5`  
		Last Modified: Wed, 17 Nov 2021 10:37:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6019f701200cccecc94989192d6e24d516c0caf6dac8cf738a52dc692cdcc5`  
		Last Modified: Wed, 17 Nov 2021 10:37:16 GMT  
		Size: 64.3 MB (64274357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfeaf47594ee6eb3ba95c4973b0208a13fdf6ec53fc0ce5e92c1f508bc5d4b1`  
		Last Modified: Wed, 17 Nov 2021 10:37:02 GMT  
		Size: 5.6 KB (5558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ead5a0e294b3e58b381630d28bdec23b6ab8491adff71c22f83e4db39202fd4`  
		Last Modified: Wed, 17 Nov 2021 10:37:02 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.51`

```console
$ docker pull mysql@sha256:740eb9fb4fdedfa9edb60c656db104f7cc497f0aab55a8df412d51e73a0615ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.6.51` - linux; amd64

```console
$ docker pull mysql@sha256:8bd695def30f2f4a32774a3233f70709e1c5046efa21b40f0d2a8475fb7bbe08
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102971684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10de32843f9157f341f3e742640b49a702ef644f78b4ace43deff5f94ae3c063`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:38 GMT
ADD file:2868c3af63afe6b8aadac07b8776e5468a3ed135fd84ad22df15e48f0610c7ba in / 
# Wed, 17 Nov 2021 02:22:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:34:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 17 Nov 2021 10:35:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:35:00 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 10:35:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 10:35:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 10:35:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:35:24 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 17 Nov 2021 10:35:24 GMT
ENV MYSQL_MAJOR=5.6
# Wed, 17 Nov 2021 10:35:24 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Wed, 17 Nov 2021 10:35:25 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Wed, 17 Nov 2021 10:35:41 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 17 Nov 2021 10:35:42 GMT
VOLUME [/var/lib/mysql]
# Wed, 17 Nov 2021 10:35:42 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 17 Nov 2021 10:35:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 17 Nov 2021 10:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 10:35:44 GMT
EXPOSE 3306
# Wed, 17 Nov 2021 10:35:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89166b5eeae47d8c878cb88f20cc67eda2a550a697f4be317c7b7abea566b76f`  
		Last Modified: Wed, 17 Nov 2021 02:29:32 GMT  
		Size: 22.5 MB (22527686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73631a7ee13b400e10866868fbf0667fa1827689c8112ded7262f0f8d7a46ad0`  
		Last Modified: Wed, 17 Nov 2021 10:37:07 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f287d5f3290c68f206c6ddd3790534d98068b9b5f7889d69228c1fbd56b40279`  
		Last Modified: Wed, 17 Nov 2021 10:37:07 GMT  
		Size: 4.5 MB (4503836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a24ae08d840d53c9137ef617a35fd4078c51406a05dfab9083ea1ca3d46f08d`  
		Last Modified: Wed, 17 Nov 2021 10:37:05 GMT  
		Size: 1.4 MB (1412228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b749bd83c0e68067e56f2b48c1cb8a30efc5d6b990a46f95476a3128c8285a3`  
		Last Modified: Wed, 17 Nov 2021 10:37:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69787256215e7a608a1f37f4349c6243d104e9254f08f027bf0a36b905f603a6`  
		Last Modified: Wed, 17 Nov 2021 10:37:09 GMT  
		Size: 10.2 MB (10225786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d273eb6cdd86afd2ed0017bdef8b7d3d2308c9cd56075ff9854b3669ed8717f`  
		Last Modified: Wed, 17 Nov 2021 10:37:02 GMT  
		Size: 20.0 KB (19999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a897b78ad8f86b2fc4bed220a614a205f9fcdf0d75f968ddc1b25483eeb82e5`  
		Last Modified: Wed, 17 Nov 2021 10:37:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6019f701200cccecc94989192d6e24d516c0caf6dac8cf738a52dc692cdcc5`  
		Last Modified: Wed, 17 Nov 2021 10:37:16 GMT  
		Size: 64.3 MB (64274357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfeaf47594ee6eb3ba95c4973b0208a13fdf6ec53fc0ce5e92c1f508bc5d4b1`  
		Last Modified: Wed, 17 Nov 2021 10:37:02 GMT  
		Size: 5.6 KB (5558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ead5a0e294b3e58b381630d28bdec23b6ab8491adff71c22f83e4db39202fd4`  
		Last Modified: Wed, 17 Nov 2021 10:37:02 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:7a3a7b7a29e6fbff433c339fc52245435fa2c308586481f2f92ab1df239d6a29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:208315e5f89d822547065fc4e29433e23cd135289342c200407b658e4c651618
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154848607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b43c6af2ad08d95cdcb415d245446909a6cbc1875604c48c4325972e5b00442`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:32:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 17 Nov 2021 10:32:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:32:58 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 10:33:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 10:33:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 10:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:33:29 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 17 Nov 2021 10:34:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 17 Nov 2021 10:34:10 GMT
ENV MYSQL_VERSION=5.7.36-1debian10
# Wed, 17 Nov 2021 10:34:11 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 17 Nov 2021 10:34:39 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 17 Nov 2021 10:34:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 17 Nov 2021 10:34:41 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 17 Nov 2021 10:34:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 17 Nov 2021 10:34:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 10:34:43 GMT
EXPOSE 3306 33060
# Wed, 17 Nov 2021 10:34:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76a7eb51ffd66492d1e2fae9037d992666e4f0b1fa0a33b62c1de3037c17406`  
		Last Modified: Wed, 17 Nov 2021 10:36:04 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258223f927e4301d4af97e9cfda9d928a9571fff93b0fdb8306cea7478e20a16`  
		Last Modified: Wed, 17 Nov 2021 10:36:05 GMT  
		Size: 4.2 MB (4179250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2c75386df9e05399af79ae74eed16fbd80524032273f41b9fb30c9eb5fd11c`  
		Last Modified: Wed, 17 Nov 2021 10:36:03 GMT  
		Size: 1.4 MB (1419452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e92e4046c9d1ef967aef94e50a2d6731427561436bfe693ebc7d31ac198c52`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5845c7315445bc6fdaadd999741235e564b2d0c2329c7ac20d6bbc018d693e8`  
		Last Modified: Wed, 17 Nov 2021 10:36:06 GMT  
		Size: 13.4 MB (13448643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0401123a9bb1165a0c29b245575aaa8a3b918a8e9462b6b2922e688554cc4a`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2724b2da64fdec0b649e0336c8a5596b5ead25d59960382dd200af6e3c326277`  
		Last Modified: Wed, 17 Nov 2021 10:36:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a7e9e325c461f936592cb8a83ffd470b41726578d7007b8ccea35c580795c`  
		Last Modified: Wed, 17 Nov 2021 10:36:49 GMT  
		Size: 108.6 MB (108637946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5fd9c3683d5de4f54dff3476c2692c6a09de5c4072e58c086e61ece1645ca5`  
		Last Modified: Wed, 17 Nov 2021 10:36:33 GMT  
		Size: 5.5 KB (5540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e35f83a12e9cb1af2b4d08665e9958d08c4f08399977766e57003c6a28575d0`  
		Last Modified: Wed, 17 Nov 2021 10:36:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.36`

```console
$ docker pull mysql@sha256:7a3a7b7a29e6fbff433c339fc52245435fa2c308586481f2f92ab1df239d6a29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.36` - linux; amd64

```console
$ docker pull mysql@sha256:208315e5f89d822547065fc4e29433e23cd135289342c200407b658e4c651618
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154848607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b43c6af2ad08d95cdcb415d245446909a6cbc1875604c48c4325972e5b00442`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:32:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 17 Nov 2021 10:32:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:32:58 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 10:33:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 10:33:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 10:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:33:29 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 17 Nov 2021 10:34:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 17 Nov 2021 10:34:10 GMT
ENV MYSQL_VERSION=5.7.36-1debian10
# Wed, 17 Nov 2021 10:34:11 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 17 Nov 2021 10:34:39 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 17 Nov 2021 10:34:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 17 Nov 2021 10:34:41 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 17 Nov 2021 10:34:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 17 Nov 2021 10:34:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 10:34:43 GMT
EXPOSE 3306 33060
# Wed, 17 Nov 2021 10:34:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76a7eb51ffd66492d1e2fae9037d992666e4f0b1fa0a33b62c1de3037c17406`  
		Last Modified: Wed, 17 Nov 2021 10:36:04 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258223f927e4301d4af97e9cfda9d928a9571fff93b0fdb8306cea7478e20a16`  
		Last Modified: Wed, 17 Nov 2021 10:36:05 GMT  
		Size: 4.2 MB (4179250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2c75386df9e05399af79ae74eed16fbd80524032273f41b9fb30c9eb5fd11c`  
		Last Modified: Wed, 17 Nov 2021 10:36:03 GMT  
		Size: 1.4 MB (1419452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e92e4046c9d1ef967aef94e50a2d6731427561436bfe693ebc7d31ac198c52`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5845c7315445bc6fdaadd999741235e564b2d0c2329c7ac20d6bbc018d693e8`  
		Last Modified: Wed, 17 Nov 2021 10:36:06 GMT  
		Size: 13.4 MB (13448643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0401123a9bb1165a0c29b245575aaa8a3b918a8e9462b6b2922e688554cc4a`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2724b2da64fdec0b649e0336c8a5596b5ead25d59960382dd200af6e3c326277`  
		Last Modified: Wed, 17 Nov 2021 10:36:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a7e9e325c461f936592cb8a83ffd470b41726578d7007b8ccea35c580795c`  
		Last Modified: Wed, 17 Nov 2021 10:36:49 GMT  
		Size: 108.6 MB (108637946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5fd9c3683d5de4f54dff3476c2692c6a09de5c4072e58c086e61ece1645ca5`  
		Last Modified: Wed, 17 Nov 2021 10:36:33 GMT  
		Size: 5.5 KB (5540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e35f83a12e9cb1af2b4d08665e9958d08c4f08399977766e57003c6a28575d0`  
		Last Modified: Wed, 17 Nov 2021 10:36:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:aeecae58035f3868bf4f00e5fc623630d8b438db9d05f4d8c6538deb14d4c31b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:1ea233722275afb6bf54bdb53bcb162bdb9f3ceed69c64836250f72bc641f63a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.4 MB (151446094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b05128b000ddbafb0a0d2713086c6a1cc23280dee3529d37f03c98c97c8cf1ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:32:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 17 Nov 2021 10:32:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:32:58 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 10:33:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 10:33:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 10:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:33:29 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 17 Nov 2021 10:33:29 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 17 Nov 2021 10:33:30 GMT
ENV MYSQL_VERSION=8.0.27-1debian10
# Wed, 17 Nov 2021 10:33:31 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 17 Nov 2021 10:33:54 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 17 Nov 2021 10:33:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 17 Nov 2021 10:33:55 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 17 Nov 2021 10:33:56 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 17 Nov 2021 10:33:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 17 Nov 2021 10:33:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 10:33:58 GMT
EXPOSE 3306 33060
# Wed, 17 Nov 2021 10:33:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76a7eb51ffd66492d1e2fae9037d992666e4f0b1fa0a33b62c1de3037c17406`  
		Last Modified: Wed, 17 Nov 2021 10:36:04 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258223f927e4301d4af97e9cfda9d928a9571fff93b0fdb8306cea7478e20a16`  
		Last Modified: Wed, 17 Nov 2021 10:36:05 GMT  
		Size: 4.2 MB (4179250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2c75386df9e05399af79ae74eed16fbd80524032273f41b9fb30c9eb5fd11c`  
		Last Modified: Wed, 17 Nov 2021 10:36:03 GMT  
		Size: 1.4 MB (1419452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e92e4046c9d1ef967aef94e50a2d6731427561436bfe693ebc7d31ac198c52`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5845c7315445bc6fdaadd999741235e564b2d0c2329c7ac20d6bbc018d693e8`  
		Last Modified: Wed, 17 Nov 2021 10:36:06 GMT  
		Size: 13.4 MB (13448643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0401123a9bb1165a0c29b245575aaa8a3b918a8e9462b6b2922e688554cc4a`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef07ec35f1acc5f120c415c26458032f9c1c71b4c0b08e95b9baa31536c2fe2`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a3131508999a6432320cc4640da6c1ceba643b1beba31a44dde45e39ee0a7`  
		Last Modified: Wed, 17 Nov 2021 10:36:18 GMT  
		Size: 105.2 MB (105234588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349ed800d44ace17a743d8a66586380109c70d1b53adbebd60c7fc240f2ecb5`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01857ca4c1930f391968213d7b37f363e5f986b5b0cc3623345d0b649755fb`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 5.5 KB (5542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc13890eda8422bcbb932fd2d6d157d7819cb4c76e9673b22d38d11226c8d1a`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:aeecae58035f3868bf4f00e5fc623630d8b438db9d05f4d8c6538deb14d4c31b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:1ea233722275afb6bf54bdb53bcb162bdb9f3ceed69c64836250f72bc641f63a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.4 MB (151446094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b05128b000ddbafb0a0d2713086c6a1cc23280dee3529d37f03c98c97c8cf1ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:32:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 17 Nov 2021 10:32:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:32:58 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 10:33:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 10:33:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 10:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:33:29 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 17 Nov 2021 10:33:29 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 17 Nov 2021 10:33:30 GMT
ENV MYSQL_VERSION=8.0.27-1debian10
# Wed, 17 Nov 2021 10:33:31 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 17 Nov 2021 10:33:54 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 17 Nov 2021 10:33:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 17 Nov 2021 10:33:55 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 17 Nov 2021 10:33:56 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 17 Nov 2021 10:33:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 17 Nov 2021 10:33:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 10:33:58 GMT
EXPOSE 3306 33060
# Wed, 17 Nov 2021 10:33:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76a7eb51ffd66492d1e2fae9037d992666e4f0b1fa0a33b62c1de3037c17406`  
		Last Modified: Wed, 17 Nov 2021 10:36:04 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258223f927e4301d4af97e9cfda9d928a9571fff93b0fdb8306cea7478e20a16`  
		Last Modified: Wed, 17 Nov 2021 10:36:05 GMT  
		Size: 4.2 MB (4179250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2c75386df9e05399af79ae74eed16fbd80524032273f41b9fb30c9eb5fd11c`  
		Last Modified: Wed, 17 Nov 2021 10:36:03 GMT  
		Size: 1.4 MB (1419452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e92e4046c9d1ef967aef94e50a2d6731427561436bfe693ebc7d31ac198c52`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5845c7315445bc6fdaadd999741235e564b2d0c2329c7ac20d6bbc018d693e8`  
		Last Modified: Wed, 17 Nov 2021 10:36:06 GMT  
		Size: 13.4 MB (13448643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0401123a9bb1165a0c29b245575aaa8a3b918a8e9462b6b2922e688554cc4a`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef07ec35f1acc5f120c415c26458032f9c1c71b4c0b08e95b9baa31536c2fe2`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a3131508999a6432320cc4640da6c1ceba643b1beba31a44dde45e39ee0a7`  
		Last Modified: Wed, 17 Nov 2021 10:36:18 GMT  
		Size: 105.2 MB (105234588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349ed800d44ace17a743d8a66586380109c70d1b53adbebd60c7fc240f2ecb5`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01857ca4c1930f391968213d7b37f363e5f986b5b0cc3623345d0b649755fb`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 5.5 KB (5542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc13890eda8422bcbb932fd2d6d157d7819cb4c76e9673b22d38d11226c8d1a`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.27`

```console
$ docker pull mysql@sha256:aeecae58035f3868bf4f00e5fc623630d8b438db9d05f4d8c6538deb14d4c31b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.27` - linux; amd64

```console
$ docker pull mysql@sha256:1ea233722275afb6bf54bdb53bcb162bdb9f3ceed69c64836250f72bc641f63a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.4 MB (151446094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b05128b000ddbafb0a0d2713086c6a1cc23280dee3529d37f03c98c97c8cf1ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:32:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 17 Nov 2021 10:32:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:32:58 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 10:33:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 10:33:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 10:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:33:29 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 17 Nov 2021 10:33:29 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 17 Nov 2021 10:33:30 GMT
ENV MYSQL_VERSION=8.0.27-1debian10
# Wed, 17 Nov 2021 10:33:31 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 17 Nov 2021 10:33:54 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 17 Nov 2021 10:33:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 17 Nov 2021 10:33:55 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 17 Nov 2021 10:33:56 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 17 Nov 2021 10:33:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 17 Nov 2021 10:33:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 10:33:58 GMT
EXPOSE 3306 33060
# Wed, 17 Nov 2021 10:33:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76a7eb51ffd66492d1e2fae9037d992666e4f0b1fa0a33b62c1de3037c17406`  
		Last Modified: Wed, 17 Nov 2021 10:36:04 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258223f927e4301d4af97e9cfda9d928a9571fff93b0fdb8306cea7478e20a16`  
		Last Modified: Wed, 17 Nov 2021 10:36:05 GMT  
		Size: 4.2 MB (4179250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2c75386df9e05399af79ae74eed16fbd80524032273f41b9fb30c9eb5fd11c`  
		Last Modified: Wed, 17 Nov 2021 10:36:03 GMT  
		Size: 1.4 MB (1419452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e92e4046c9d1ef967aef94e50a2d6731427561436bfe693ebc7d31ac198c52`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5845c7315445bc6fdaadd999741235e564b2d0c2329c7ac20d6bbc018d693e8`  
		Last Modified: Wed, 17 Nov 2021 10:36:06 GMT  
		Size: 13.4 MB (13448643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0401123a9bb1165a0c29b245575aaa8a3b918a8e9462b6b2922e688554cc4a`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef07ec35f1acc5f120c415c26458032f9c1c71b4c0b08e95b9baa31536c2fe2`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a3131508999a6432320cc4640da6c1ceba643b1beba31a44dde45e39ee0a7`  
		Last Modified: Wed, 17 Nov 2021 10:36:18 GMT  
		Size: 105.2 MB (105234588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349ed800d44ace17a743d8a66586380109c70d1b53adbebd60c7fc240f2ecb5`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01857ca4c1930f391968213d7b37f363e5f986b5b0cc3623345d0b649755fb`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 5.5 KB (5542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc13890eda8422bcbb932fd2d6d157d7819cb4c76e9673b22d38d11226c8d1a`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:aeecae58035f3868bf4f00e5fc623630d8b438db9d05f4d8c6538deb14d4c31b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:1ea233722275afb6bf54bdb53bcb162bdb9f3ceed69c64836250f72bc641f63a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.4 MB (151446094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b05128b000ddbafb0a0d2713086c6a1cc23280dee3529d37f03c98c97c8cf1ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:32:47 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 17 Nov 2021 10:32:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:32:58 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 10:33:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 10:33:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 10:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:33:29 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Wed, 17 Nov 2021 10:33:29 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 17 Nov 2021 10:33:30 GMT
ENV MYSQL_VERSION=8.0.27-1debian10
# Wed, 17 Nov 2021 10:33:31 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 17 Nov 2021 10:33:54 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 17 Nov 2021 10:33:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 17 Nov 2021 10:33:55 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 17 Nov 2021 10:33:56 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Wed, 17 Nov 2021 10:33:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 17 Nov 2021 10:33:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 10:33:58 GMT
EXPOSE 3306 33060
# Wed, 17 Nov 2021 10:33:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76a7eb51ffd66492d1e2fae9037d992666e4f0b1fa0a33b62c1de3037c17406`  
		Last Modified: Wed, 17 Nov 2021 10:36:04 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258223f927e4301d4af97e9cfda9d928a9571fff93b0fdb8306cea7478e20a16`  
		Last Modified: Wed, 17 Nov 2021 10:36:05 GMT  
		Size: 4.2 MB (4179250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2c75386df9e05399af79ae74eed16fbd80524032273f41b9fb30c9eb5fd11c`  
		Last Modified: Wed, 17 Nov 2021 10:36:03 GMT  
		Size: 1.4 MB (1419452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e92e4046c9d1ef967aef94e50a2d6731427561436bfe693ebc7d31ac198c52`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5845c7315445bc6fdaadd999741235e564b2d0c2329c7ac20d6bbc018d693e8`  
		Last Modified: Wed, 17 Nov 2021 10:36:06 GMT  
		Size: 13.4 MB (13448643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0401123a9bb1165a0c29b245575aaa8a3b918a8e9462b6b2922e688554cc4a`  
		Last Modified: Wed, 17 Nov 2021 10:36:02 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef07ec35f1acc5f120c415c26458032f9c1c71b4c0b08e95b9baa31536c2fe2`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93a3131508999a6432320cc4640da6c1ceba643b1beba31a44dde45e39ee0a7`  
		Last Modified: Wed, 17 Nov 2021 10:36:18 GMT  
		Size: 105.2 MB (105234588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349ed800d44ace17a743d8a66586380109c70d1b53adbebd60c7fc240f2ecb5`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01857ca4c1930f391968213d7b37f363e5f986b5b0cc3623345d0b649755fb`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 5.5 KB (5542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc13890eda8422bcbb932fd2d6d157d7819cb4c76e9673b22d38d11226c8d1a`  
		Last Modified: Wed, 17 Nov 2021 10:36:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
