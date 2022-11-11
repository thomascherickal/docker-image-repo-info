<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10-jammy`](#mariadb10-jammy)
-	[`mariadb:10.10-rc`](#mariadb1010-rc)
-	[`mariadb:10.10-rc-jammy`](#mariadb1010-rc-jammy)
-	[`mariadb:10.10.1-rc`](#mariadb10101-rc)
-	[`mariadb:10.10.1-rc-jammy`](#mariadb10101-rc-jammy)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.3.37`](#mariadb10337)
-	[`mariadb:10.3.37-focal`](#mariadb10337-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.4.27`](#mariadb10427)
-	[`mariadb:10.4.27-focal`](#mariadb10427-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10.5.18`](#mariadb10518)
-	[`mariadb:10.5.18-focal`](#mariadb10518-focal)
-	[`mariadb:10.6`](#mariadb106)
-	[`mariadb:10.6-focal`](#mariadb106-focal)
-	[`mariadb:10.6.11`](#mariadb10611)
-	[`mariadb:10.6.11-focal`](#mariadb10611-focal)
-	[`mariadb:10.7`](#mariadb107)
-	[`mariadb:10.7-focal`](#mariadb107-focal)
-	[`mariadb:10.7.7`](#mariadb1077)
-	[`mariadb:10.7.7-focal`](#mariadb1077-focal)
-	[`mariadb:10.8`](#mariadb108)
-	[`mariadb:10.8-jammy`](#mariadb108-jammy)
-	[`mariadb:10.8.6`](#mariadb1086)
-	[`mariadb:10.8.6-jammy`](#mariadb1086-jammy)
-	[`mariadb:10.9`](#mariadb109)
-	[`mariadb:10.9-jammy`](#mariadb109-jammy)
-	[`mariadb:10.9.4`](#mariadb1094)
-	[`mariadb:10.9.4-jammy`](#mariadb1094-jammy)
-	[`mariadb:jammy`](#mariadbjammy)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:4d0d7e05cac3f285cb7b38226e8f61f406c6ea2527c317ec2b31a5f5270d7fb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:91323beb7c5c2fb134d13874504aea4e4608304370423019f277b1f70882f9ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121852276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825ad7e31db8cfc5ffa434e1171060e9f60db49279dd675fc562466da3bc0ea0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:50:58 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:50:59 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:50:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:51:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:51:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:51:33 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:51:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ea015f843833e7db49738387776c15cc20eafdf70ef5045dff63f0737b4f2`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c861410f2b3e963a06afa4ca24fda97e00c496b9dc2a3ced1f8affa8f94293f`  
		Last Modified: Fri, 11 Nov 2022 01:58:12 GMT  
		Size: 85.9 MB (85885285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46193445bc4f96aba11e38a4481b43380bee2c095422d3df722641dcad6bc477`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262eb9124c0aca8d6780dfa07f0a43ff16308aa84d6f2c84e5566a0d975bd9dd`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:31f677ba9b50beef8d48a3bbcab29485f5aa3a90677d1ebc44039bbc9bc8bde4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118604917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe889c390f208ce09bf8bfa7869b7d342d999c4279a8809e3a2d2a14332cf10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:07:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 20:07:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:35 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 20:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 20:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 20:07:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 20:08:36 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 20:08:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 20:08:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 20:08:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 20:08:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:08:55 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 20:08:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf568f815bdc2b755b642d6cad079d9e2e71dd364d2806bf4a9a3cb0fe3d18b7`  
		Last Modified: Wed, 02 Nov 2022 20:10:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a27635d8616b3a361adc11c7e5712c05d3edef95c0573370b2c92058ed582`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 3.7 MB (3737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce0b0cfd1e867e47d514f1de07a5da365d36bfb15513e7cf310802577ab13c`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 1.9 MB (1898793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd291b4a9d31c95c30d2580b470dd4ecbe4d2d10c11e47967a037f8b939146e`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505d811110d4c6311181f11307bd36ac49e38d1ab561c611e562b293b90a9ef`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 2.2 MB (2191982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf7ac4a18820861abff79a668773c9f881f45b6f47d10f21df0661e7190013b`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5452b6a0ce3706d857279cfa1cdaef7c8b6bc76d8d6a4b1c43367203b766cd2f`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2628f7ef3cedd084f9a47495aa153853592da56561a6e3231a78435d95ff9949`  
		Last Modified: Wed, 02 Nov 2022 20:10:44 GMT  
		Size: 82.4 MB (82378919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e903661ffaca59211d235a8061c23cc51afe2459c91999d6e191b263897d86d0`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ecec752f0246a09512597065787135cfb39650e56b627521d6b7a25b44bec`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0b3197dcaae25333f0f203038060ecdea256e57a3dbddac50f28647989b2710d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130653312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837797e389ef277d85639136b3254240872973d0626320986cfffbfb6a87f0b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:21:41 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:21:42 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:21:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:22:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:22:34 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:22:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:22:35 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:22:35 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74756e55e3348ae0fd95c532056ccfd545a53ef391306dc1e40c944f767b424`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87682e9f6b59527390239170077fb830688d0d3ecb3a00ec019774d672fb7c9a`  
		Last Modified: Fri, 11 Nov 2022 03:32:44 GMT  
		Size: 89.0 MB (88977999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e944b0bd7dc5e8a3abc0784d0bbca0b06bf94e01f94133c299086f0ab5db977b`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50240058fe79dd7c3e564cbe912654ac3d47ff0b4ec8cf8843727f57594b73bc`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; s390x

```console
$ docker pull mariadb@sha256:79b920fffb62ce6a5a5d43710462a5ee875839d137278cd648e98e4888851a0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119532750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c1a22b2569dd6f45c61a2a09a52ee5ac7577df02b9e510c73e4ef5e0798155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:03:13 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:03:13 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:03:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:03:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:03:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:03:44 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:03:45 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:03:45 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:03:45 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272871ff5a39e7f724ba60200020bda369282194ceb0a7fbacace8a0c1a6bd3`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a8ba951405415f1411b29b725fc469af2374cb7c4f24018f4f0ff7802d236d`  
		Last Modified: Fri, 11 Nov 2022 03:09:54 GMT  
		Size: 85.5 MB (85468667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89a1761c7bc6b466cd2efb4d28b9a0fc4fb55be84ded124f3922236ecf7c3af`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4932db4ceb6992a81f9ab516f105280d520e93584dc1b3302f0fa0d9feb96e57`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 7.0 KB (6952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-jammy`

```console
$ docker pull mariadb@sha256:4d0d7e05cac3f285cb7b38226e8f61f406c6ea2527c317ec2b31a5f5270d7fb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:91323beb7c5c2fb134d13874504aea4e4608304370423019f277b1f70882f9ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121852276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825ad7e31db8cfc5ffa434e1171060e9f60db49279dd675fc562466da3bc0ea0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:50:58 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:50:59 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:50:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:51:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:51:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:51:33 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:51:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ea015f843833e7db49738387776c15cc20eafdf70ef5045dff63f0737b4f2`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c861410f2b3e963a06afa4ca24fda97e00c496b9dc2a3ced1f8affa8f94293f`  
		Last Modified: Fri, 11 Nov 2022 01:58:12 GMT  
		Size: 85.9 MB (85885285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46193445bc4f96aba11e38a4481b43380bee2c095422d3df722641dcad6bc477`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262eb9124c0aca8d6780dfa07f0a43ff16308aa84d6f2c84e5566a0d975bd9dd`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:31f677ba9b50beef8d48a3bbcab29485f5aa3a90677d1ebc44039bbc9bc8bde4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118604917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe889c390f208ce09bf8bfa7869b7d342d999c4279a8809e3a2d2a14332cf10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:07:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 20:07:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:35 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 20:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 20:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 20:07:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 20:08:36 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 20:08:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 20:08:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 20:08:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 20:08:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:08:55 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 20:08:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf568f815bdc2b755b642d6cad079d9e2e71dd364d2806bf4a9a3cb0fe3d18b7`  
		Last Modified: Wed, 02 Nov 2022 20:10:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a27635d8616b3a361adc11c7e5712c05d3edef95c0573370b2c92058ed582`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 3.7 MB (3737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce0b0cfd1e867e47d514f1de07a5da365d36bfb15513e7cf310802577ab13c`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 1.9 MB (1898793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd291b4a9d31c95c30d2580b470dd4ecbe4d2d10c11e47967a037f8b939146e`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505d811110d4c6311181f11307bd36ac49e38d1ab561c611e562b293b90a9ef`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 2.2 MB (2191982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf7ac4a18820861abff79a668773c9f881f45b6f47d10f21df0661e7190013b`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5452b6a0ce3706d857279cfa1cdaef7c8b6bc76d8d6a4b1c43367203b766cd2f`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2628f7ef3cedd084f9a47495aa153853592da56561a6e3231a78435d95ff9949`  
		Last Modified: Wed, 02 Nov 2022 20:10:44 GMT  
		Size: 82.4 MB (82378919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e903661ffaca59211d235a8061c23cc51afe2459c91999d6e191b263897d86d0`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ecec752f0246a09512597065787135cfb39650e56b627521d6b7a25b44bec`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0b3197dcaae25333f0f203038060ecdea256e57a3dbddac50f28647989b2710d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130653312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837797e389ef277d85639136b3254240872973d0626320986cfffbfb6a87f0b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:21:41 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:21:42 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:21:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:22:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:22:34 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:22:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:22:35 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:22:35 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74756e55e3348ae0fd95c532056ccfd545a53ef391306dc1e40c944f767b424`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87682e9f6b59527390239170077fb830688d0d3ecb3a00ec019774d672fb7c9a`  
		Last Modified: Fri, 11 Nov 2022 03:32:44 GMT  
		Size: 89.0 MB (88977999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e944b0bd7dc5e8a3abc0784d0bbca0b06bf94e01f94133c299086f0ab5db977b`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50240058fe79dd7c3e564cbe912654ac3d47ff0b4ec8cf8843727f57594b73bc`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:79b920fffb62ce6a5a5d43710462a5ee875839d137278cd648e98e4888851a0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119532750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c1a22b2569dd6f45c61a2a09a52ee5ac7577df02b9e510c73e4ef5e0798155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:03:13 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:03:13 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:03:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:03:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:03:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:03:44 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:03:45 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:03:45 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:03:45 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272871ff5a39e7f724ba60200020bda369282194ceb0a7fbacace8a0c1a6bd3`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a8ba951405415f1411b29b725fc469af2374cb7c4f24018f4f0ff7802d236d`  
		Last Modified: Fri, 11 Nov 2022 03:09:54 GMT  
		Size: 85.5 MB (85468667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89a1761c7bc6b466cd2efb4d28b9a0fc4fb55be84ded124f3922236ecf7c3af`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4932db4ceb6992a81f9ab516f105280d520e93584dc1b3302f0fa0d9feb96e57`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 7.0 KB (6952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10-rc`

```console
$ docker pull mariadb@sha256:e6bd0fe24e4fabed4c0e0b9d83f72d1264b3b4cf39fad4f3bbf6fd8c671b221e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.10-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:a3b14c15225b4788b562d48f1910ba34eeb4282d3ca62f0db3d2bf4db4621144
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125335699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57de3e4d4a4748bd9f256af1c8adae44736c8aaece6f7137449c6186da2ec20f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:48:17 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:48:17 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 01:48:17 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 01:48:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:48:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:50:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:50:48 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:50:49 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:50:49 GMT
COPY file:25990863e4bd169447bf1d169dbaf3eeaf1299650f69524839fe736dc4358be0 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:50:49 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:50:49 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4e42c6b3fe74b8807bf126325d60167b163c7c5bd9ee0b7460cf9926995c66`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eff5b9b68025fd41eb88195a612cf7b369d1b72e362cc866379a52576b6c9dd`  
		Last Modified: Fri, 11 Nov 2022 01:57:44 GMT  
		Size: 89.4 MB (89368635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd587236afdff8a5bf7d9da2aeaee605fbe028289b1c2cb3bb60da87afd907a`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5532f5c0f6753ade67cf121ab73589101b07dbc713333a77c9f1ccdf55bba93`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 7.0 KB (7022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:963f93b32ec3cf17946c29f0fcc3a88fa3e9c938dc28840c0df410ae22c0eec3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104564191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10e5a505ae3328dff1184514c083e7d637f801fb9176dc3f8645070c1a394c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:07:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 20:07:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:35 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 20:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 20:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 20:07:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 20:07:53 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Wed, 02 Nov 2022 20:07:53 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Wed, 02 Nov 2022 20:07:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 20:08:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 20:08:26 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 20:08:26 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 20:08:26 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 20:08:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:08:26 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 20:08:27 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf568f815bdc2b755b642d6cad079d9e2e71dd364d2806bf4a9a3cb0fe3d18b7`  
		Last Modified: Wed, 02 Nov 2022 20:10:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a27635d8616b3a361adc11c7e5712c05d3edef95c0573370b2c92058ed582`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 3.7 MB (3737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce0b0cfd1e867e47d514f1de07a5da365d36bfb15513e7cf310802577ab13c`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 1.9 MB (1898793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd291b4a9d31c95c30d2580b470dd4ecbe4d2d10c11e47967a037f8b939146e`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505d811110d4c6311181f11307bd36ac49e38d1ab561c611e562b293b90a9ef`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 2.2 MB (2191982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf7ac4a18820861abff79a668773c9f881f45b6f47d10f21df0661e7190013b`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16759adaacc369b316e50cfb18576aea210022969ccdde95d0ae70cb4a0cffc3`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee076b67e8d0c5d62c7f7050a79ad3b8c0be044937447d244161f5bc46393e`  
		Last Modified: Wed, 02 Nov 2022 20:10:18 GMT  
		Size: 68.3 MB (68338186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062fe35f14777880e0fe5635d6e44b97fd9656588003d18fa32f537d2022c606`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f81b6128476aa69662040adf0f309bd0cd1e7040b7204a13f8cc59a2087af`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:15b62e749a352f5bfb085d3738a3a91d1ab406bce91061c1304f783d8561161d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115983169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b281624168c3acc055ed6e929a9ad3a4c638d560c78eee1011509affb7d6016a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:20:29 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:20:29 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:20:29 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:20:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:20:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:21:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:21:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:21:24 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:21:24 GMT
COPY file:25990863e4bd169447bf1d169dbaf3eeaf1299650f69524839fe736dc4358be0 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:21:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:21:24 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:21:25 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb0cb936a2acb37318aa66371678b6469b36746892f168d82b7706d88ee5e66`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e602f542ba8ca5f4968ee5548312642c4d1e76db438d942db4d2ee99e72b498`  
		Last Modified: Fri, 11 Nov 2022 03:32:02 GMT  
		Size: 74.3 MB (74307783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0986c6bfbaa39f32aae79c3ec673fc22b9e8030aeac54a0c14e47642ac7a7354`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b44c6640977e16593702be6faf1d8b7988875f0acc12f7de2af04ed65a0dab0`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 7.0 KB (7026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:466a016787fc9a48bfd06706f5d1e7a24e593e7a788f11ec1fed3f2d395d26ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.9 MB (104862261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a0c7d9cf40a49a33350585ea00c7398e95a455a80386a6479115593f534f9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:02:19 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:02:19 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:02:20 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:02:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:02:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:02:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:03:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:03:02 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:03:02 GMT
COPY file:25990863e4bd169447bf1d169dbaf3eeaf1299650f69524839fe736dc4358be0 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:03:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:03:03 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:03:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa489e6e7f3fdeb5bac9c4b5cce35652d00bc7d9fc72d5da1772f086584487`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ffd151a74ea6b4a58d22cf4e113cc8cf9fe9a61a3ec747c849241c743c0459`  
		Last Modified: Fri, 11 Nov 2022 03:09:31 GMT  
		Size: 70.8 MB (70798106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15994a6a65b30fcf96d0cd37e85d6b0e59a5ecc9b62eccd0b552354134804d0a`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdd51647580f8135f9404596921295fd19a2bfc046400390541bbc101e7216c`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 7.0 KB (7025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10-rc-jammy`

```console
$ docker pull mariadb@sha256:e6bd0fe24e4fabed4c0e0b9d83f72d1264b3b4cf39fad4f3bbf6fd8c671b221e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.10-rc-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:a3b14c15225b4788b562d48f1910ba34eeb4282d3ca62f0db3d2bf4db4621144
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125335699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57de3e4d4a4748bd9f256af1c8adae44736c8aaece6f7137449c6186da2ec20f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:48:17 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:48:17 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 01:48:17 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 01:48:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:48:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:50:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:50:48 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:50:49 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:50:49 GMT
COPY file:25990863e4bd169447bf1d169dbaf3eeaf1299650f69524839fe736dc4358be0 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:50:49 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:50:49 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4e42c6b3fe74b8807bf126325d60167b163c7c5bd9ee0b7460cf9926995c66`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eff5b9b68025fd41eb88195a612cf7b369d1b72e362cc866379a52576b6c9dd`  
		Last Modified: Fri, 11 Nov 2022 01:57:44 GMT  
		Size: 89.4 MB (89368635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd587236afdff8a5bf7d9da2aeaee605fbe028289b1c2cb3bb60da87afd907a`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5532f5c0f6753ade67cf121ab73589101b07dbc713333a77c9f1ccdf55bba93`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 7.0 KB (7022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-rc-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:963f93b32ec3cf17946c29f0fcc3a88fa3e9c938dc28840c0df410ae22c0eec3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104564191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10e5a505ae3328dff1184514c083e7d637f801fb9176dc3f8645070c1a394c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:07:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 20:07:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:35 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 20:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 20:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 20:07:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 20:07:53 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Wed, 02 Nov 2022 20:07:53 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Wed, 02 Nov 2022 20:07:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 20:08:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 20:08:26 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 20:08:26 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 20:08:26 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 20:08:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:08:26 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 20:08:27 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf568f815bdc2b755b642d6cad079d9e2e71dd364d2806bf4a9a3cb0fe3d18b7`  
		Last Modified: Wed, 02 Nov 2022 20:10:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a27635d8616b3a361adc11c7e5712c05d3edef95c0573370b2c92058ed582`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 3.7 MB (3737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce0b0cfd1e867e47d514f1de07a5da365d36bfb15513e7cf310802577ab13c`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 1.9 MB (1898793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd291b4a9d31c95c30d2580b470dd4ecbe4d2d10c11e47967a037f8b939146e`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505d811110d4c6311181f11307bd36ac49e38d1ab561c611e562b293b90a9ef`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 2.2 MB (2191982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf7ac4a18820861abff79a668773c9f881f45b6f47d10f21df0661e7190013b`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16759adaacc369b316e50cfb18576aea210022969ccdde95d0ae70cb4a0cffc3`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee076b67e8d0c5d62c7f7050a79ad3b8c0be044937447d244161f5bc46393e`  
		Last Modified: Wed, 02 Nov 2022 20:10:18 GMT  
		Size: 68.3 MB (68338186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062fe35f14777880e0fe5635d6e44b97fd9656588003d18fa32f537d2022c606`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f81b6128476aa69662040adf0f309bd0cd1e7040b7204a13f8cc59a2087af`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-rc-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:15b62e749a352f5bfb085d3738a3a91d1ab406bce91061c1304f783d8561161d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115983169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b281624168c3acc055ed6e929a9ad3a4c638d560c78eee1011509affb7d6016a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:20:29 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:20:29 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:20:29 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:20:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:20:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:21:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:21:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:21:24 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:21:24 GMT
COPY file:25990863e4bd169447bf1d169dbaf3eeaf1299650f69524839fe736dc4358be0 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:21:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:21:24 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:21:25 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb0cb936a2acb37318aa66371678b6469b36746892f168d82b7706d88ee5e66`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e602f542ba8ca5f4968ee5548312642c4d1e76db438d942db4d2ee99e72b498`  
		Last Modified: Fri, 11 Nov 2022 03:32:02 GMT  
		Size: 74.3 MB (74307783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0986c6bfbaa39f32aae79c3ec673fc22b9e8030aeac54a0c14e47642ac7a7354`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b44c6640977e16593702be6faf1d8b7988875f0acc12f7de2af04ed65a0dab0`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 7.0 KB (7026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-rc-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:466a016787fc9a48bfd06706f5d1e7a24e593e7a788f11ec1fed3f2d395d26ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.9 MB (104862261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a0c7d9cf40a49a33350585ea00c7398e95a455a80386a6479115593f534f9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:02:19 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:02:19 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:02:20 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:02:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:02:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:02:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:03:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:03:02 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:03:02 GMT
COPY file:25990863e4bd169447bf1d169dbaf3eeaf1299650f69524839fe736dc4358be0 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:03:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:03:03 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:03:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa489e6e7f3fdeb5bac9c4b5cce35652d00bc7d9fc72d5da1772f086584487`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ffd151a74ea6b4a58d22cf4e113cc8cf9fe9a61a3ec747c849241c743c0459`  
		Last Modified: Fri, 11 Nov 2022 03:09:31 GMT  
		Size: 70.8 MB (70798106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15994a6a65b30fcf96d0cd37e85d6b0e59a5ecc9b62eccd0b552354134804d0a`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdd51647580f8135f9404596921295fd19a2bfc046400390541bbc101e7216c`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 7.0 KB (7025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10.1-rc`

```console
$ docker pull mariadb@sha256:e6bd0fe24e4fabed4c0e0b9d83f72d1264b3b4cf39fad4f3bbf6fd8c671b221e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.10.1-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:a3b14c15225b4788b562d48f1910ba34eeb4282d3ca62f0db3d2bf4db4621144
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125335699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57de3e4d4a4748bd9f256af1c8adae44736c8aaece6f7137449c6186da2ec20f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:48:17 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:48:17 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 01:48:17 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 01:48:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:48:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:50:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:50:48 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:50:49 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:50:49 GMT
COPY file:25990863e4bd169447bf1d169dbaf3eeaf1299650f69524839fe736dc4358be0 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:50:49 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:50:49 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4e42c6b3fe74b8807bf126325d60167b163c7c5bd9ee0b7460cf9926995c66`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eff5b9b68025fd41eb88195a612cf7b369d1b72e362cc866379a52576b6c9dd`  
		Last Modified: Fri, 11 Nov 2022 01:57:44 GMT  
		Size: 89.4 MB (89368635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd587236afdff8a5bf7d9da2aeaee605fbe028289b1c2cb3bb60da87afd907a`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5532f5c0f6753ade67cf121ab73589101b07dbc713333a77c9f1ccdf55bba93`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 7.0 KB (7022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.1-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:963f93b32ec3cf17946c29f0fcc3a88fa3e9c938dc28840c0df410ae22c0eec3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104564191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10e5a505ae3328dff1184514c083e7d637f801fb9176dc3f8645070c1a394c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:07:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 20:07:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:35 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 20:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 20:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 20:07:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 20:07:53 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Wed, 02 Nov 2022 20:07:53 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Wed, 02 Nov 2022 20:07:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 20:08:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 20:08:26 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 20:08:26 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 20:08:26 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 20:08:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:08:26 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 20:08:27 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf568f815bdc2b755b642d6cad079d9e2e71dd364d2806bf4a9a3cb0fe3d18b7`  
		Last Modified: Wed, 02 Nov 2022 20:10:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a27635d8616b3a361adc11c7e5712c05d3edef95c0573370b2c92058ed582`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 3.7 MB (3737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce0b0cfd1e867e47d514f1de07a5da365d36bfb15513e7cf310802577ab13c`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 1.9 MB (1898793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd291b4a9d31c95c30d2580b470dd4ecbe4d2d10c11e47967a037f8b939146e`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505d811110d4c6311181f11307bd36ac49e38d1ab561c611e562b293b90a9ef`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 2.2 MB (2191982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf7ac4a18820861abff79a668773c9f881f45b6f47d10f21df0661e7190013b`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16759adaacc369b316e50cfb18576aea210022969ccdde95d0ae70cb4a0cffc3`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee076b67e8d0c5d62c7f7050a79ad3b8c0be044937447d244161f5bc46393e`  
		Last Modified: Wed, 02 Nov 2022 20:10:18 GMT  
		Size: 68.3 MB (68338186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062fe35f14777880e0fe5635d6e44b97fd9656588003d18fa32f537d2022c606`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f81b6128476aa69662040adf0f309bd0cd1e7040b7204a13f8cc59a2087af`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.1-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:15b62e749a352f5bfb085d3738a3a91d1ab406bce91061c1304f783d8561161d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115983169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b281624168c3acc055ed6e929a9ad3a4c638d560c78eee1011509affb7d6016a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:20:29 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:20:29 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:20:29 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:20:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:20:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:21:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:21:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:21:24 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:21:24 GMT
COPY file:25990863e4bd169447bf1d169dbaf3eeaf1299650f69524839fe736dc4358be0 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:21:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:21:24 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:21:25 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb0cb936a2acb37318aa66371678b6469b36746892f168d82b7706d88ee5e66`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e602f542ba8ca5f4968ee5548312642c4d1e76db438d942db4d2ee99e72b498`  
		Last Modified: Fri, 11 Nov 2022 03:32:02 GMT  
		Size: 74.3 MB (74307783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0986c6bfbaa39f32aae79c3ec673fc22b9e8030aeac54a0c14e47642ac7a7354`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b44c6640977e16593702be6faf1d8b7988875f0acc12f7de2af04ed65a0dab0`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 7.0 KB (7026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.1-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:466a016787fc9a48bfd06706f5d1e7a24e593e7a788f11ec1fed3f2d395d26ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.9 MB (104862261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a0c7d9cf40a49a33350585ea00c7398e95a455a80386a6479115593f534f9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:02:19 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:02:19 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:02:20 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:02:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:02:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:02:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:03:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:03:02 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:03:02 GMT
COPY file:25990863e4bd169447bf1d169dbaf3eeaf1299650f69524839fe736dc4358be0 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:03:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:03:03 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:03:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa489e6e7f3fdeb5bac9c4b5cce35652d00bc7d9fc72d5da1772f086584487`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ffd151a74ea6b4a58d22cf4e113cc8cf9fe9a61a3ec747c849241c743c0459`  
		Last Modified: Fri, 11 Nov 2022 03:09:31 GMT  
		Size: 70.8 MB (70798106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15994a6a65b30fcf96d0cd37e85d6b0e59a5ecc9b62eccd0b552354134804d0a`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdd51647580f8135f9404596921295fd19a2bfc046400390541bbc101e7216c`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 7.0 KB (7025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10.1-rc-jammy`

```console
$ docker pull mariadb@sha256:e6bd0fe24e4fabed4c0e0b9d83f72d1264b3b4cf39fad4f3bbf6fd8c671b221e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.10.1-rc-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:a3b14c15225b4788b562d48f1910ba34eeb4282d3ca62f0db3d2bf4db4621144
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125335699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57de3e4d4a4748bd9f256af1c8adae44736c8aaece6f7137449c6186da2ec20f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:48:17 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:48:17 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 01:48:17 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 01:48:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:48:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:50:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:50:48 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:50:49 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:50:49 GMT
COPY file:25990863e4bd169447bf1d169dbaf3eeaf1299650f69524839fe736dc4358be0 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:50:49 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:50:49 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4e42c6b3fe74b8807bf126325d60167b163c7c5bd9ee0b7460cf9926995c66`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eff5b9b68025fd41eb88195a612cf7b369d1b72e362cc866379a52576b6c9dd`  
		Last Modified: Fri, 11 Nov 2022 01:57:44 GMT  
		Size: 89.4 MB (89368635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd587236afdff8a5bf7d9da2aeaee605fbe028289b1c2cb3bb60da87afd907a`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5532f5c0f6753ade67cf121ab73589101b07dbc713333a77c9f1ccdf55bba93`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 7.0 KB (7022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.1-rc-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:963f93b32ec3cf17946c29f0fcc3a88fa3e9c938dc28840c0df410ae22c0eec3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104564191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10e5a505ae3328dff1184514c083e7d637f801fb9176dc3f8645070c1a394c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:07:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 20:07:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:35 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 20:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 20:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 20:07:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 20:07:53 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Wed, 02 Nov 2022 20:07:53 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Wed, 02 Nov 2022 20:07:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 20:08:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 20:08:26 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 20:08:26 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 20:08:26 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 20:08:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:08:26 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 20:08:27 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf568f815bdc2b755b642d6cad079d9e2e71dd364d2806bf4a9a3cb0fe3d18b7`  
		Last Modified: Wed, 02 Nov 2022 20:10:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a27635d8616b3a361adc11c7e5712c05d3edef95c0573370b2c92058ed582`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 3.7 MB (3737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce0b0cfd1e867e47d514f1de07a5da365d36bfb15513e7cf310802577ab13c`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 1.9 MB (1898793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd291b4a9d31c95c30d2580b470dd4ecbe4d2d10c11e47967a037f8b939146e`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505d811110d4c6311181f11307bd36ac49e38d1ab561c611e562b293b90a9ef`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 2.2 MB (2191982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf7ac4a18820861abff79a668773c9f881f45b6f47d10f21df0661e7190013b`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16759adaacc369b316e50cfb18576aea210022969ccdde95d0ae70cb4a0cffc3`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee076b67e8d0c5d62c7f7050a79ad3b8c0be044937447d244161f5bc46393e`  
		Last Modified: Wed, 02 Nov 2022 20:10:18 GMT  
		Size: 68.3 MB (68338186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062fe35f14777880e0fe5635d6e44b97fd9656588003d18fa32f537d2022c606`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f81b6128476aa69662040adf0f309bd0cd1e7040b7204a13f8cc59a2087af`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.1-rc-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:15b62e749a352f5bfb085d3738a3a91d1ab406bce91061c1304f783d8561161d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115983169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b281624168c3acc055ed6e929a9ad3a4c638d560c78eee1011509affb7d6016a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:20:29 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:20:29 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:20:29 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:20:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:20:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:21:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:21:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:21:24 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:21:24 GMT
COPY file:25990863e4bd169447bf1d169dbaf3eeaf1299650f69524839fe736dc4358be0 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:21:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:21:24 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:21:25 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb0cb936a2acb37318aa66371678b6469b36746892f168d82b7706d88ee5e66`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e602f542ba8ca5f4968ee5548312642c4d1e76db438d942db4d2ee99e72b498`  
		Last Modified: Fri, 11 Nov 2022 03:32:02 GMT  
		Size: 74.3 MB (74307783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0986c6bfbaa39f32aae79c3ec673fc22b9e8030aeac54a0c14e47642ac7a7354`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b44c6640977e16593702be6faf1d8b7988875f0acc12f7de2af04ed65a0dab0`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 7.0 KB (7026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.1-rc-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:466a016787fc9a48bfd06706f5d1e7a24e593e7a788f11ec1fed3f2d395d26ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.9 MB (104862261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a0c7d9cf40a49a33350585ea00c7398e95a455a80386a6479115593f534f9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:02:19 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.10.1 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:02:19 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:02:20 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 11 Nov 2022 03:02:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:02:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:02:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:03:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:03:02 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:03:02 GMT
COPY file:25990863e4bd169447bf1d169dbaf3eeaf1299650f69524839fe736dc4358be0 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:03:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:03:03 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:03:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa489e6e7f3fdeb5bac9c4b5cce35652d00bc7d9fc72d5da1772f086584487`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ffd151a74ea6b4a58d22cf4e113cc8cf9fe9a61a3ec747c849241c743c0459`  
		Last Modified: Fri, 11 Nov 2022 03:09:31 GMT  
		Size: 70.8 MB (70798106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15994a6a65b30fcf96d0cd37e85d6b0e59a5ecc9b62eccd0b552354134804d0a`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdd51647580f8135f9404596921295fd19a2bfc046400390541bbc101e7216c`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 7.0 KB (7025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:229f16b7b0db12542a03b5558532fb4547bfa096573733b40d5ce97960172392
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:88315725f8961ab4d91c20fbecd9fe8ed94e1308d9a43753dc854e2e9b77d5e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.3 MB (116254671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12dbf81334e66564cf622ceeb3ef2eba25496f89c496016d75511dc84a95b4b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:56:07 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.37 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:56:07 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 01:56:07 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 01:56:08 GMT
ARG MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 01:56:08 GMT
ENV MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 01:56:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:56:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:56:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:56:48 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:56:48 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:56:48 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:56:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 01:56:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:56:49 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:56:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865982e3cee20383fcd698d2e069997a2f6e75285bfbdbe4e22055a6490e7583`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b4fed4869f52bf82650dd21e0c0b857c7bc2e11cbbf1ad0a9d051e4be78f7`  
		Last Modified: Fri, 11 Nov 2022 02:01:16 GMT  
		Size: 80.6 MB (80605489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab4df2cb047830c5e95e3da6b86db4229c039c3e17b9fc0480b40cf10782630`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4369125e079bbfc6b7f6d2c178a984eb2df90f4cdf804f49b3f04f019f69d`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e319f1926e9374c6947ec1cf5edac811e8c43a541e638b30a56174497b19d99`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6e1cf33ddb9f60daf2d5589c37a8cd52b5608e336a293ce7baf8437de0ed2dd1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.9 MB (117887693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:729e60a10768f8fd0ac693422371c236789581d64b3c669eb01ad39c772a4971`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 02:04:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 26 Oct 2022 02:04:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Oct 2022 02:04:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Oct 2022 02:04:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Oct 2022 02:04:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 26 Oct 2022 02:04:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 26 Oct 2022 02:06:56 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 26 Oct 2022 02:06:56 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 26 Oct 2022 02:06:56 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Wed, 26 Oct 2022 02:06:56 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Wed, 26 Oct 2022 02:06:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Wed, 26 Oct 2022 02:06:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 26 Oct 2022 02:07:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 26 Oct 2022 02:07:23 GMT
VOLUME [/var/lib/mysql]
# Wed, 26 Oct 2022 02:07:23 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Wed, 26 Oct 2022 02:07:23 GMT
COPY file:1cbfae6200694fb67440ab571faea87cbbd737228ff9f3193338e54312e6bd67 in /usr/local/bin/ 
# Wed, 26 Oct 2022 02:07:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 26 Oct 2022 02:07:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 02:07:24 GMT
EXPOSE 3306
# Wed, 26 Oct 2022 02:07:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5059476c4efaaefd5639d62272cf873b43fc4dd354f29aa2d424f5672f98d7`  
		Last Modified: Wed, 26 Oct 2022 02:09:48 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b512e3647ec22a314bc3b404b44b891220289f7918fc3fb90dec28d934b622f7`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 5.5 MB (5474279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4034a198751d9b8465f987f8cd51acc3b45288510ea70f4f50588aca7ab03e`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 3.4 MB (3368397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a303c93f3f2afdbf7461aaa57d2e0376745b909ca61dc1ab04bed8a727844135`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a95ecb4d8b5c99728b7e239140c0c9127f6b8286e033494da3d7b938d10669`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 2.2 MB (2186475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c381f22b0bfdceb13b81f9105a5b0965c5d34d0a2800bc7ae58461d1661aae`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5e4ae6fa721db243d094858081ca19bdd1913dd7dbc52cebf012b7f4b5f28e`  
		Last Modified: Wed, 26 Oct 2022 02:11:37 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d6ed2e45c44a5242ab5143fb2cde22180df8de6443f78bac2b820fd86fe611`  
		Last Modified: Wed, 26 Oct 2022 02:11:46 GMT  
		Size: 79.6 MB (79647166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04ed73a30385efc9f1556a2ba502e00fc1f363c08dcbc006c2d2253a7da2283`  
		Last Modified: Wed, 26 Oct 2022 02:11:37 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ab85d4aef4566129044d4bc578b3368544bbd868b6fa582e9b948564b7a0d3`  
		Last Modified: Wed, 26 Oct 2022 02:11:37 GMT  
		Size: 7.0 KB (7048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b97fe511cff91cce26db83a9eb005fa3938f985894b873de070b22ee6c9ea6`  
		Last Modified: Wed, 26 Oct 2022 02:11:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6914b5541752a4b47c5d0698b58980f28cd680b0a8da00ab1959cd3af6972ac5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126293912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ab84e4c8e343b7688bff5b878df4926d657f1ad27d784b78e80643893b08f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:29:17 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.37 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:29:17 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 03:29:18 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 03:29:18 GMT
ARG MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 03:29:18 GMT
ENV MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 03:29:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:29:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:30:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:30:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:30:14 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:30:14 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:30:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 03:30:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:30:16 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:30:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c359b928c28b00c68c533dc07e237364f3c3f10b9e239c535d51f8b5ec77bb8`  
		Last Modified: Fri, 11 Nov 2022 03:37:00 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea9e01eda7f4572e36f937bf0190b81219587649fa614ad36448056d8099769`  
		Last Modified: Fri, 11 Nov 2022 03:37:22 GMT  
		Size: 85.2 MB (85214900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c57973f8a817db494573220882174ba7b2e7387fd2b2f4d1446af69bcf8bf0a`  
		Last Modified: Fri, 11 Nov 2022 03:36:59 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7319f795babe08a364c35c84d77b63c9adf9e6a621494dc45f1dc8ddefe054`  
		Last Modified: Fri, 11 Nov 2022 03:36:59 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc7fc0c0d2819e4a9b4e4afe2421952561761557476c5c4d1b8e948c2ee34f1`  
		Last Modified: Fri, 11 Nov 2022 03:37:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:229f16b7b0db12542a03b5558532fb4547bfa096573733b40d5ce97960172392
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:88315725f8961ab4d91c20fbecd9fe8ed94e1308d9a43753dc854e2e9b77d5e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.3 MB (116254671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12dbf81334e66564cf622ceeb3ef2eba25496f89c496016d75511dc84a95b4b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:56:07 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.37 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:56:07 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 01:56:07 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 01:56:08 GMT
ARG MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 01:56:08 GMT
ENV MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 01:56:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:56:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:56:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:56:48 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:56:48 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:56:48 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:56:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 01:56:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:56:49 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:56:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865982e3cee20383fcd698d2e069997a2f6e75285bfbdbe4e22055a6490e7583`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b4fed4869f52bf82650dd21e0c0b857c7bc2e11cbbf1ad0a9d051e4be78f7`  
		Last Modified: Fri, 11 Nov 2022 02:01:16 GMT  
		Size: 80.6 MB (80605489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab4df2cb047830c5e95e3da6b86db4229c039c3e17b9fc0480b40cf10782630`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4369125e079bbfc6b7f6d2c178a984eb2df90f4cdf804f49b3f04f019f69d`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e319f1926e9374c6947ec1cf5edac811e8c43a541e638b30a56174497b19d99`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6e1cf33ddb9f60daf2d5589c37a8cd52b5608e336a293ce7baf8437de0ed2dd1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.9 MB (117887693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:729e60a10768f8fd0ac693422371c236789581d64b3c669eb01ad39c772a4971`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 02:04:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 26 Oct 2022 02:04:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Oct 2022 02:04:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Oct 2022 02:04:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Oct 2022 02:04:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 26 Oct 2022 02:04:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 26 Oct 2022 02:06:56 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 26 Oct 2022 02:06:56 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 26 Oct 2022 02:06:56 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Wed, 26 Oct 2022 02:06:56 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Wed, 26 Oct 2022 02:06:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Wed, 26 Oct 2022 02:06:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 26 Oct 2022 02:07:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 26 Oct 2022 02:07:23 GMT
VOLUME [/var/lib/mysql]
# Wed, 26 Oct 2022 02:07:23 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Wed, 26 Oct 2022 02:07:23 GMT
COPY file:1cbfae6200694fb67440ab571faea87cbbd737228ff9f3193338e54312e6bd67 in /usr/local/bin/ 
# Wed, 26 Oct 2022 02:07:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 26 Oct 2022 02:07:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 02:07:24 GMT
EXPOSE 3306
# Wed, 26 Oct 2022 02:07:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5059476c4efaaefd5639d62272cf873b43fc4dd354f29aa2d424f5672f98d7`  
		Last Modified: Wed, 26 Oct 2022 02:09:48 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b512e3647ec22a314bc3b404b44b891220289f7918fc3fb90dec28d934b622f7`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 5.5 MB (5474279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4034a198751d9b8465f987f8cd51acc3b45288510ea70f4f50588aca7ab03e`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 3.4 MB (3368397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a303c93f3f2afdbf7461aaa57d2e0376745b909ca61dc1ab04bed8a727844135`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a95ecb4d8b5c99728b7e239140c0c9127f6b8286e033494da3d7b938d10669`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 2.2 MB (2186475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c381f22b0bfdceb13b81f9105a5b0965c5d34d0a2800bc7ae58461d1661aae`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5e4ae6fa721db243d094858081ca19bdd1913dd7dbc52cebf012b7f4b5f28e`  
		Last Modified: Wed, 26 Oct 2022 02:11:37 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d6ed2e45c44a5242ab5143fb2cde22180df8de6443f78bac2b820fd86fe611`  
		Last Modified: Wed, 26 Oct 2022 02:11:46 GMT  
		Size: 79.6 MB (79647166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04ed73a30385efc9f1556a2ba502e00fc1f363c08dcbc006c2d2253a7da2283`  
		Last Modified: Wed, 26 Oct 2022 02:11:37 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ab85d4aef4566129044d4bc578b3368544bbd868b6fa582e9b948564b7a0d3`  
		Last Modified: Wed, 26 Oct 2022 02:11:37 GMT  
		Size: 7.0 KB (7048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b97fe511cff91cce26db83a9eb005fa3938f985894b873de070b22ee6c9ea6`  
		Last Modified: Wed, 26 Oct 2022 02:11:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6914b5541752a4b47c5d0698b58980f28cd680b0a8da00ab1959cd3af6972ac5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126293912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ab84e4c8e343b7688bff5b878df4926d657f1ad27d784b78e80643893b08f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:29:17 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.37 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:29:17 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 03:29:18 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 03:29:18 GMT
ARG MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 03:29:18 GMT
ENV MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 03:29:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:29:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:30:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:30:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:30:14 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:30:14 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:30:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 03:30:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:30:16 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:30:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c359b928c28b00c68c533dc07e237364f3c3f10b9e239c535d51f8b5ec77bb8`  
		Last Modified: Fri, 11 Nov 2022 03:37:00 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea9e01eda7f4572e36f937bf0190b81219587649fa614ad36448056d8099769`  
		Last Modified: Fri, 11 Nov 2022 03:37:22 GMT  
		Size: 85.2 MB (85214900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c57973f8a817db494573220882174ba7b2e7387fd2b2f4d1446af69bcf8bf0a`  
		Last Modified: Fri, 11 Nov 2022 03:36:59 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7319f795babe08a364c35c84d77b63c9adf9e6a621494dc45f1dc8ddefe054`  
		Last Modified: Fri, 11 Nov 2022 03:36:59 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc7fc0c0d2819e4a9b4e4afe2421952561761557476c5c4d1b8e948c2ee34f1`  
		Last Modified: Fri, 11 Nov 2022 03:37:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.37`

```console
$ docker pull mariadb@sha256:0f4bd818bcfd076b4ff3c95c452970c8389826e784d981ff2889d31f7dccd245
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; ppc64le

### `mariadb:10.3.37` - linux; amd64

```console
$ docker pull mariadb@sha256:88315725f8961ab4d91c20fbecd9fe8ed94e1308d9a43753dc854e2e9b77d5e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.3 MB (116254671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12dbf81334e66564cf622ceeb3ef2eba25496f89c496016d75511dc84a95b4b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:56:07 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.37 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:56:07 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 01:56:07 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 01:56:08 GMT
ARG MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 01:56:08 GMT
ENV MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 01:56:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:56:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:56:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:56:48 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:56:48 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:56:48 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:56:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 01:56:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:56:49 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:56:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865982e3cee20383fcd698d2e069997a2f6e75285bfbdbe4e22055a6490e7583`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b4fed4869f52bf82650dd21e0c0b857c7bc2e11cbbf1ad0a9d051e4be78f7`  
		Last Modified: Fri, 11 Nov 2022 02:01:16 GMT  
		Size: 80.6 MB (80605489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab4df2cb047830c5e95e3da6b86db4229c039c3e17b9fc0480b40cf10782630`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4369125e079bbfc6b7f6d2c178a984eb2df90f4cdf804f49b3f04f019f69d`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e319f1926e9374c6947ec1cf5edac811e8c43a541e638b30a56174497b19d99`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.37` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6914b5541752a4b47c5d0698b58980f28cd680b0a8da00ab1959cd3af6972ac5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126293912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ab84e4c8e343b7688bff5b878df4926d657f1ad27d784b78e80643893b08f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:29:17 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.37 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:29:17 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 03:29:18 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 03:29:18 GMT
ARG MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 03:29:18 GMT
ENV MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 03:29:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:29:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:30:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:30:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:30:14 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:30:14 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:30:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 03:30:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:30:16 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:30:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c359b928c28b00c68c533dc07e237364f3c3f10b9e239c535d51f8b5ec77bb8`  
		Last Modified: Fri, 11 Nov 2022 03:37:00 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea9e01eda7f4572e36f937bf0190b81219587649fa614ad36448056d8099769`  
		Last Modified: Fri, 11 Nov 2022 03:37:22 GMT  
		Size: 85.2 MB (85214900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c57973f8a817db494573220882174ba7b2e7387fd2b2f4d1446af69bcf8bf0a`  
		Last Modified: Fri, 11 Nov 2022 03:36:59 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7319f795babe08a364c35c84d77b63c9adf9e6a621494dc45f1dc8ddefe054`  
		Last Modified: Fri, 11 Nov 2022 03:36:59 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc7fc0c0d2819e4a9b4e4afe2421952561761557476c5c4d1b8e948c2ee34f1`  
		Last Modified: Fri, 11 Nov 2022 03:37:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.37-focal`

```console
$ docker pull mariadb@sha256:0f4bd818bcfd076b4ff3c95c452970c8389826e784d981ff2889d31f7dccd245
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; ppc64le

### `mariadb:10.3.37-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:88315725f8961ab4d91c20fbecd9fe8ed94e1308d9a43753dc854e2e9b77d5e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.3 MB (116254671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12dbf81334e66564cf622ceeb3ef2eba25496f89c496016d75511dc84a95b4b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:56:07 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.37 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:56:07 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 01:56:07 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 01:56:08 GMT
ARG MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 01:56:08 GMT
ENV MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 01:56:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:56:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:56:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:56:48 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:56:48 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:56:48 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:56:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 01:56:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:56:49 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:56:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865982e3cee20383fcd698d2e069997a2f6e75285bfbdbe4e22055a6490e7583`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b4fed4869f52bf82650dd21e0c0b857c7bc2e11cbbf1ad0a9d051e4be78f7`  
		Last Modified: Fri, 11 Nov 2022 02:01:16 GMT  
		Size: 80.6 MB (80605489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab4df2cb047830c5e95e3da6b86db4229c039c3e17b9fc0480b40cf10782630`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb4369125e079bbfc6b7f6d2c178a984eb2df90f4cdf804f49b3f04f019f69d`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e319f1926e9374c6947ec1cf5edac811e8c43a541e638b30a56174497b19d99`  
		Last Modified: Fri, 11 Nov 2022 02:01:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.37-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6914b5541752a4b47c5d0698b58980f28cd680b0a8da00ab1959cd3af6972ac5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126293912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ab84e4c8e343b7688bff5b878df4926d657f1ad27d784b78e80643893b08f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:29:17 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.3.37 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:29:17 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 03:29:18 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 11 Nov 2022 03:29:18 GMT
ARG MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 03:29:18 GMT
ENV MARIADB_VERSION=1:10.3.37+maria~ubu2004
# Fri, 11 Nov 2022 03:29:19 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:29:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:30:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:30:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:30:14 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:30:14 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:30:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.37/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 03:30:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:30:16 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:30:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c359b928c28b00c68c533dc07e237364f3c3f10b9e239c535d51f8b5ec77bb8`  
		Last Modified: Fri, 11 Nov 2022 03:37:00 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea9e01eda7f4572e36f937bf0190b81219587649fa614ad36448056d8099769`  
		Last Modified: Fri, 11 Nov 2022 03:37:22 GMT  
		Size: 85.2 MB (85214900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c57973f8a817db494573220882174ba7b2e7387fd2b2f4d1446af69bcf8bf0a`  
		Last Modified: Fri, 11 Nov 2022 03:36:59 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7319f795babe08a364c35c84d77b63c9adf9e6a621494dc45f1dc8ddefe054`  
		Last Modified: Fri, 11 Nov 2022 03:36:59 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc7fc0c0d2819e4a9b4e4afe2421952561761557476c5c4d1b8e948c2ee34f1`  
		Last Modified: Fri, 11 Nov 2022 03:37:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:a2b8a37b071263f983405b869033aede3790e14e5b8409ea51e6f89af9a537e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:d7f7680b742731010cbcc86d15b0bfec0eec95b6fcaef8a5160241d148ad6bd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121923597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7220d96a2feed7c791377c09fe450448290a4c327cbe8477f9fc0d4963b1c5ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:55:33 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.27 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:55:33 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 01:55:33 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 01:55:33 GMT
ARG MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 01:55:34 GMT
ENV MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 01:55:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:55:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:56:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:56:03 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:56:03 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:56:04 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:56:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 01:56:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:56:04 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:56:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6e90cd3bce21ed4946e731cfc8f23169254aadcbcc1a016c7d6baa294132bc`  
		Last Modified: Fri, 11 Nov 2022 02:00:35 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a943b84fc5e1a1e6556772cf850dc2060ab41fda93afc28797a587610c14c72`  
		Last Modified: Fri, 11 Nov 2022 02:00:48 GMT  
		Size: 86.3 MB (86274416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1ebae0292e37c961340e710b8a36d30134c6916fe57276d18a377a33b66d61`  
		Last Modified: Fri, 11 Nov 2022 02:00:35 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d204f8bf4f983cca85995bfa2a0cc87fbeece980a77e8cb6300648352f41f156`  
		Last Modified: Fri, 11 Nov 2022 02:00:36 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165ae61fef4ff1b53edbaf36e2879572e437e1dbce6da8dfb81855cc29b58511`  
		Last Modified: Fri, 11 Nov 2022 02:00:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:3130c8b3cfe902ca64fc1acd954018418a9d6fe08cba5b7d546bd0cd0655a697
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123380408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd7aa1b396921e68965a55c3a268a8cb5d705d13f6a33eeb3b76a1d3aa74e9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 02:04:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 26 Oct 2022 02:04:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Oct 2022 02:04:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Oct 2022 02:04:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Oct 2022 02:04:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 26 Oct 2022 02:04:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 26 Oct 2022 02:06:27 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 26 Oct 2022 02:06:27 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 26 Oct 2022 02:06:27 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Wed, 26 Oct 2022 02:06:28 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Wed, 26 Oct 2022 02:06:28 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Wed, 26 Oct 2022 02:06:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 26 Oct 2022 02:06:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 26 Oct 2022 02:06:52 GMT
VOLUME [/var/lib/mysql]
# Wed, 26 Oct 2022 02:06:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Wed, 26 Oct 2022 02:06:52 GMT
COPY file:1cbfae6200694fb67440ab571faea87cbbd737228ff9f3193338e54312e6bd67 in /usr/local/bin/ 
# Wed, 26 Oct 2022 02:06:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 26 Oct 2022 02:06:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 02:06:53 GMT
EXPOSE 3306
# Wed, 26 Oct 2022 02:06:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5059476c4efaaefd5639d62272cf873b43fc4dd354f29aa2d424f5672f98d7`  
		Last Modified: Wed, 26 Oct 2022 02:09:48 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b512e3647ec22a314bc3b404b44b891220289f7918fc3fb90dec28d934b622f7`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 5.5 MB (5474279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4034a198751d9b8465f987f8cd51acc3b45288510ea70f4f50588aca7ab03e`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 3.4 MB (3368397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a303c93f3f2afdbf7461aaa57d2e0376745b909ca61dc1ab04bed8a727844135`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a95ecb4d8b5c99728b7e239140c0c9127f6b8286e033494da3d7b938d10669`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 2.2 MB (2186475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c381f22b0bfdceb13b81f9105a5b0965c5d34d0a2800bc7ae58461d1661aae`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49abf541d1422a95d8e41b69fd3e1486aab8e60372a17f173741885d2eaed6a`  
		Last Modified: Wed, 26 Oct 2022 02:11:11 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8db3abcfcfa29a6cb75bb8bdd527882817830b1210f3ea6d3490c1fd840525`  
		Last Modified: Wed, 26 Oct 2022 02:11:21 GMT  
		Size: 85.1 MB (85139880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d7cb4e1258ee2bab27a064345a399aa11b2255737f7900fab8a91a01fbb93b`  
		Last Modified: Wed, 26 Oct 2022 02:11:10 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d748f549470cd2311d8ec1bce4581218a4d585a4759631c469c1de18781d66`  
		Last Modified: Wed, 26 Oct 2022 02:11:11 GMT  
		Size: 7.0 KB (7048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e58f14536007bd56cd2f752f47936667c94b867d5b48081d21cb7958257d7`  
		Last Modified: Wed, 26 Oct 2022 02:11:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:3d33948117c745a723e3660a5e98da02deb59c91d760eab6624ea23777598eca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (131950954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:663094144fc4c0214b7f23fee349fafcfd7f922c864a00ea45c2a9d88db33787`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:28:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.27 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:28:06 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 03:28:07 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 03:28:07 GMT
ARG MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 03:28:07 GMT
ENV MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 03:28:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:28:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:28:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:29:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:29:00 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:29:01 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:29:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 03:29:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:29:03 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:29:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cc9c4586a97ab1df55258596a5e68ae50ac80efab4c6360e4f492a2f6c641a`  
		Last Modified: Fri, 11 Nov 2022 03:36:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058c2fb9453cc4bd712af794998480c02537d96da71d9bb4c55b664a9c56d426`  
		Last Modified: Fri, 11 Nov 2022 03:36:40 GMT  
		Size: 90.9 MB (90871942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6728d5641795fbf5e994603fa5e13a52f0c8c9282883cdbd354bb0262511b81f`  
		Last Modified: Fri, 11 Nov 2022 03:36:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe08026ebb836258113e1c62c23b52f7cb9039a2df89510cabd08ab2a4f52477`  
		Last Modified: Fri, 11 Nov 2022 03:36:16 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20592e2a2cf289010898977e6f77fa3bb2691a20a4e3a34e17ae98ada6995900`  
		Last Modified: Fri, 11 Nov 2022 03:36:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:a2b8a37b071263f983405b869033aede3790e14e5b8409ea51e6f89af9a537e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:d7f7680b742731010cbcc86d15b0bfec0eec95b6fcaef8a5160241d148ad6bd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121923597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7220d96a2feed7c791377c09fe450448290a4c327cbe8477f9fc0d4963b1c5ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:55:33 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.27 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:55:33 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 01:55:33 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 01:55:33 GMT
ARG MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 01:55:34 GMT
ENV MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 01:55:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:55:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:56:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:56:03 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:56:03 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:56:04 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:56:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 01:56:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:56:04 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:56:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6e90cd3bce21ed4946e731cfc8f23169254aadcbcc1a016c7d6baa294132bc`  
		Last Modified: Fri, 11 Nov 2022 02:00:35 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a943b84fc5e1a1e6556772cf850dc2060ab41fda93afc28797a587610c14c72`  
		Last Modified: Fri, 11 Nov 2022 02:00:48 GMT  
		Size: 86.3 MB (86274416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1ebae0292e37c961340e710b8a36d30134c6916fe57276d18a377a33b66d61`  
		Last Modified: Fri, 11 Nov 2022 02:00:35 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d204f8bf4f983cca85995bfa2a0cc87fbeece980a77e8cb6300648352f41f156`  
		Last Modified: Fri, 11 Nov 2022 02:00:36 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165ae61fef4ff1b53edbaf36e2879572e437e1dbce6da8dfb81855cc29b58511`  
		Last Modified: Fri, 11 Nov 2022 02:00:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:3130c8b3cfe902ca64fc1acd954018418a9d6fe08cba5b7d546bd0cd0655a697
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123380408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd7aa1b396921e68965a55c3a268a8cb5d705d13f6a33eeb3b76a1d3aa74e9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 02:04:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 26 Oct 2022 02:04:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Oct 2022 02:04:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Oct 2022 02:04:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Oct 2022 02:04:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 26 Oct 2022 02:04:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 26 Oct 2022 02:06:27 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 26 Oct 2022 02:06:27 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 26 Oct 2022 02:06:27 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Wed, 26 Oct 2022 02:06:28 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Wed, 26 Oct 2022 02:06:28 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Wed, 26 Oct 2022 02:06:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 26 Oct 2022 02:06:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 26 Oct 2022 02:06:52 GMT
VOLUME [/var/lib/mysql]
# Wed, 26 Oct 2022 02:06:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Wed, 26 Oct 2022 02:06:52 GMT
COPY file:1cbfae6200694fb67440ab571faea87cbbd737228ff9f3193338e54312e6bd67 in /usr/local/bin/ 
# Wed, 26 Oct 2022 02:06:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 26 Oct 2022 02:06:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 02:06:53 GMT
EXPOSE 3306
# Wed, 26 Oct 2022 02:06:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5059476c4efaaefd5639d62272cf873b43fc4dd354f29aa2d424f5672f98d7`  
		Last Modified: Wed, 26 Oct 2022 02:09:48 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b512e3647ec22a314bc3b404b44b891220289f7918fc3fb90dec28d934b622f7`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 5.5 MB (5474279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4034a198751d9b8465f987f8cd51acc3b45288510ea70f4f50588aca7ab03e`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 3.4 MB (3368397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a303c93f3f2afdbf7461aaa57d2e0376745b909ca61dc1ab04bed8a727844135`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a95ecb4d8b5c99728b7e239140c0c9127f6b8286e033494da3d7b938d10669`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 2.2 MB (2186475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c381f22b0bfdceb13b81f9105a5b0965c5d34d0a2800bc7ae58461d1661aae`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49abf541d1422a95d8e41b69fd3e1486aab8e60372a17f173741885d2eaed6a`  
		Last Modified: Wed, 26 Oct 2022 02:11:11 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8db3abcfcfa29a6cb75bb8bdd527882817830b1210f3ea6d3490c1fd840525`  
		Last Modified: Wed, 26 Oct 2022 02:11:21 GMT  
		Size: 85.1 MB (85139880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d7cb4e1258ee2bab27a064345a399aa11b2255737f7900fab8a91a01fbb93b`  
		Last Modified: Wed, 26 Oct 2022 02:11:10 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d748f549470cd2311d8ec1bce4581218a4d585a4759631c469c1de18781d66`  
		Last Modified: Wed, 26 Oct 2022 02:11:11 GMT  
		Size: 7.0 KB (7048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e58f14536007bd56cd2f752f47936667c94b867d5b48081d21cb7958257d7`  
		Last Modified: Wed, 26 Oct 2022 02:11:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:3d33948117c745a723e3660a5e98da02deb59c91d760eab6624ea23777598eca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (131950954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:663094144fc4c0214b7f23fee349fafcfd7f922c864a00ea45c2a9d88db33787`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:28:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.27 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:28:06 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 03:28:07 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 03:28:07 GMT
ARG MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 03:28:07 GMT
ENV MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 03:28:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:28:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:28:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:29:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:29:00 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:29:01 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:29:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 03:29:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:29:03 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:29:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cc9c4586a97ab1df55258596a5e68ae50ac80efab4c6360e4f492a2f6c641a`  
		Last Modified: Fri, 11 Nov 2022 03:36:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058c2fb9453cc4bd712af794998480c02537d96da71d9bb4c55b664a9c56d426`  
		Last Modified: Fri, 11 Nov 2022 03:36:40 GMT  
		Size: 90.9 MB (90871942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6728d5641795fbf5e994603fa5e13a52f0c8c9282883cdbd354bb0262511b81f`  
		Last Modified: Fri, 11 Nov 2022 03:36:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe08026ebb836258113e1c62c23b52f7cb9039a2df89510cabd08ab2a4f52477`  
		Last Modified: Fri, 11 Nov 2022 03:36:16 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20592e2a2cf289010898977e6f77fa3bb2691a20a4e3a34e17ae98ada6995900`  
		Last Modified: Fri, 11 Nov 2022 03:36:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.27`

```console
$ docker pull mariadb@sha256:f334a798e2cdec36cc52bda6a966e956a80cb02c27175fa246099b268cd16b35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; ppc64le

### `mariadb:10.4.27` - linux; amd64

```console
$ docker pull mariadb@sha256:d7f7680b742731010cbcc86d15b0bfec0eec95b6fcaef8a5160241d148ad6bd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121923597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7220d96a2feed7c791377c09fe450448290a4c327cbe8477f9fc0d4963b1c5ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:55:33 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.27 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:55:33 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 01:55:33 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 01:55:33 GMT
ARG MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 01:55:34 GMT
ENV MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 01:55:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:55:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:56:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:56:03 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:56:03 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:56:04 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:56:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 01:56:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:56:04 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:56:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6e90cd3bce21ed4946e731cfc8f23169254aadcbcc1a016c7d6baa294132bc`  
		Last Modified: Fri, 11 Nov 2022 02:00:35 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a943b84fc5e1a1e6556772cf850dc2060ab41fda93afc28797a587610c14c72`  
		Last Modified: Fri, 11 Nov 2022 02:00:48 GMT  
		Size: 86.3 MB (86274416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1ebae0292e37c961340e710b8a36d30134c6916fe57276d18a377a33b66d61`  
		Last Modified: Fri, 11 Nov 2022 02:00:35 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d204f8bf4f983cca85995bfa2a0cc87fbeece980a77e8cb6300648352f41f156`  
		Last Modified: Fri, 11 Nov 2022 02:00:36 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165ae61fef4ff1b53edbaf36e2879572e437e1dbce6da8dfb81855cc29b58511`  
		Last Modified: Fri, 11 Nov 2022 02:00:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.27` - linux; ppc64le

```console
$ docker pull mariadb@sha256:3d33948117c745a723e3660a5e98da02deb59c91d760eab6624ea23777598eca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (131950954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:663094144fc4c0214b7f23fee349fafcfd7f922c864a00ea45c2a9d88db33787`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:28:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.27 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:28:06 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 03:28:07 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 03:28:07 GMT
ARG MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 03:28:07 GMT
ENV MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 03:28:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:28:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:28:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:29:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:29:00 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:29:01 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:29:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 03:29:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:29:03 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:29:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cc9c4586a97ab1df55258596a5e68ae50ac80efab4c6360e4f492a2f6c641a`  
		Last Modified: Fri, 11 Nov 2022 03:36:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058c2fb9453cc4bd712af794998480c02537d96da71d9bb4c55b664a9c56d426`  
		Last Modified: Fri, 11 Nov 2022 03:36:40 GMT  
		Size: 90.9 MB (90871942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6728d5641795fbf5e994603fa5e13a52f0c8c9282883cdbd354bb0262511b81f`  
		Last Modified: Fri, 11 Nov 2022 03:36:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe08026ebb836258113e1c62c23b52f7cb9039a2df89510cabd08ab2a4f52477`  
		Last Modified: Fri, 11 Nov 2022 03:36:16 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20592e2a2cf289010898977e6f77fa3bb2691a20a4e3a34e17ae98ada6995900`  
		Last Modified: Fri, 11 Nov 2022 03:36:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.27-focal`

```console
$ docker pull mariadb@sha256:f334a798e2cdec36cc52bda6a966e956a80cb02c27175fa246099b268cd16b35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; ppc64le

### `mariadb:10.4.27-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:d7f7680b742731010cbcc86d15b0bfec0eec95b6fcaef8a5160241d148ad6bd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121923597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7220d96a2feed7c791377c09fe450448290a4c327cbe8477f9fc0d4963b1c5ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:55:33 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.27 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:55:33 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 01:55:33 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 01:55:33 GMT
ARG MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 01:55:34 GMT
ENV MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 01:55:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:55:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:56:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:56:03 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:56:03 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:56:04 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:56:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 01:56:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:56:04 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:56:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6e90cd3bce21ed4946e731cfc8f23169254aadcbcc1a016c7d6baa294132bc`  
		Last Modified: Fri, 11 Nov 2022 02:00:35 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a943b84fc5e1a1e6556772cf850dc2060ab41fda93afc28797a587610c14c72`  
		Last Modified: Fri, 11 Nov 2022 02:00:48 GMT  
		Size: 86.3 MB (86274416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1ebae0292e37c961340e710b8a36d30134c6916fe57276d18a377a33b66d61`  
		Last Modified: Fri, 11 Nov 2022 02:00:35 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d204f8bf4f983cca85995bfa2a0cc87fbeece980a77e8cb6300648352f41f156`  
		Last Modified: Fri, 11 Nov 2022 02:00:36 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165ae61fef4ff1b53edbaf36e2879572e437e1dbce6da8dfb81855cc29b58511`  
		Last Modified: Fri, 11 Nov 2022 02:00:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.27-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:3d33948117c745a723e3660a5e98da02deb59c91d760eab6624ea23777598eca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (131950954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:663094144fc4c0214b7f23fee349fafcfd7f922c864a00ea45c2a9d88db33787`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:28:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.4.27 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:28:06 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 03:28:07 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 11 Nov 2022 03:28:07 GMT
ARG MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 03:28:07 GMT
ENV MARIADB_VERSION=1:10.4.27+maria~ubu2004
# Fri, 11 Nov 2022 03:28:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:28:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:28:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:29:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:29:00 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:29:01 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:29:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.27/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Nov 2022 03:29:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:29:03 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:29:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cc9c4586a97ab1df55258596a5e68ae50ac80efab4c6360e4f492a2f6c641a`  
		Last Modified: Fri, 11 Nov 2022 03:36:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058c2fb9453cc4bd712af794998480c02537d96da71d9bb4c55b664a9c56d426`  
		Last Modified: Fri, 11 Nov 2022 03:36:40 GMT  
		Size: 90.9 MB (90871942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6728d5641795fbf5e994603fa5e13a52f0c8c9282883cdbd354bb0262511b81f`  
		Last Modified: Fri, 11 Nov 2022 03:36:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe08026ebb836258113e1c62c23b52f7cb9039a2df89510cabd08ab2a4f52477`  
		Last Modified: Fri, 11 Nov 2022 03:36:16 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20592e2a2cf289010898977e6f77fa3bb2691a20a4e3a34e17ae98ada6995900`  
		Last Modified: Fri, 11 Nov 2022 03:36:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:427c8a1e08b84b8dcb8256bb3e2e1608353aa7ee216bb62d682ca495069e5810
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:7dbef335ec2b32219491e718e93170598ba42bc1e7c8de77018c75ffe9824f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124186245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff56a02874cff48f63dd41974a64ecb00305e98f56f011da318079ab3a2aca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:54:53 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.18 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:54:53 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 01:54:53 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 01:54:53 GMT
ARG MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 01:54:53 GMT
ENV MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 01:54:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:54:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:55:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:55:28 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:55:28 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:55:29 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:55:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:55:29 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:55:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff10c4143de9f3ad7e4dd0d9a4cb9b28a940a5b3ffc25088a06deeec8c0bf0ce`  
		Last Modified: Fri, 11 Nov 2022 02:00:07 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86940c6e6b472adeee37ad0dfc05851e4c586adf0ac914c7eaa2088a89dd0bd2`  
		Last Modified: Fri, 11 Nov 2022 02:00:20 GMT  
		Size: 88.5 MB (88537185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb690670c568195e04ea4a7b82f19e5ae97cd9c7cff01d58fcda25d34afef844`  
		Last Modified: Fri, 11 Nov 2022 02:00:07 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c944b15571b4cca5909e3c98ad41fd5646e5a058476d4772dc89f06e8fed9`  
		Last Modified: Fri, 11 Nov 2022 02:00:07 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:75147e4a7b58fbfa6073548d3ff6a71c666f8471a82d3051b36ee7ff496e5d6f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125598592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa2997900745409815ed380f76f0f3b02a73491e05d762c6e3ee84e056538b1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 02:04:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 26 Oct 2022 02:04:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Oct 2022 02:04:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Oct 2022 02:04:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Oct 2022 02:04:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 26 Oct 2022 02:04:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 26 Oct 2022 02:06:00 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 26 Oct 2022 02:06:00 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 26 Oct 2022 02:06:00 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Wed, 26 Oct 2022 02:06:00 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Wed, 26 Oct 2022 02:06:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Wed, 26 Oct 2022 02:06:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 26 Oct 2022 02:06:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 26 Oct 2022 02:06:21 GMT
VOLUME [/var/lib/mysql]
# Wed, 26 Oct 2022 02:06:21 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Wed, 26 Oct 2022 02:06:22 GMT
COPY file:1cbfae6200694fb67440ab571faea87cbbd737228ff9f3193338e54312e6bd67 in /usr/local/bin/ 
# Wed, 26 Oct 2022 02:06:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 02:06:22 GMT
EXPOSE 3306
# Wed, 26 Oct 2022 02:06:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5059476c4efaaefd5639d62272cf873b43fc4dd354f29aa2d424f5672f98d7`  
		Last Modified: Wed, 26 Oct 2022 02:09:48 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b512e3647ec22a314bc3b404b44b891220289f7918fc3fb90dec28d934b622f7`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 5.5 MB (5474279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4034a198751d9b8465f987f8cd51acc3b45288510ea70f4f50588aca7ab03e`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 3.4 MB (3368397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a303c93f3f2afdbf7461aaa57d2e0376745b909ca61dc1ab04bed8a727844135`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a95ecb4d8b5c99728b7e239140c0c9127f6b8286e033494da3d7b938d10669`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 2.2 MB (2186475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c381f22b0bfdceb13b81f9105a5b0965c5d34d0a2800bc7ae58461d1661aae`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9317c133d22bf1a053a47870a13631dfaaa76e4aa19884640b0ada12d4392a`  
		Last Modified: Wed, 26 Oct 2022 02:10:44 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f30e678460e0f8e823655d65ea2b9548d676018bff8779c02d4e18849e3cfa`  
		Last Modified: Wed, 26 Oct 2022 02:10:55 GMT  
		Size: 87.4 MB (87358188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b426e3a31bb98d15adcd307617ecfcde7b58d10667ab34f285af458393b4919`  
		Last Modified: Wed, 26 Oct 2022 02:10:44 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3365d363ba6d0608da76aac797894b103b784e955279bfbdf9f58345101395d`  
		Last Modified: Wed, 26 Oct 2022 02:10:44 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5e4a81c0a27e73a31f7d73d7f6a06813d0059c9e0c30718f3e70b0630ca5e02d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.2 MB (134216051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db0f5b095527d06c59e3b2108f212aa6f4383289c68ef6e96f5f74154207ff22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:27:05 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.18 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:27:05 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:27:05 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:27:06 GMT
ARG MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:27:06 GMT
ENV MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:27:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:27:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:27:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:27:58 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:27:58 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:27:59 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:27:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:27:59 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:28:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa562e05c60903709ebe3e3a87dea9e04c63d505a87cda0033d11a09c38eb27`  
		Last Modified: Fri, 11 Nov 2022 03:35:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5619a4518dc98a993a8a8f4ce937b5755bea84cc79ca51782c0ddab754139ea`  
		Last Modified: Fri, 11 Nov 2022 03:35:57 GMT  
		Size: 93.1 MB (93137159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95ce40dabcc6107f427cdcaaadd7821252fad6a92798da43b93a85977a2d582`  
		Last Modified: Fri, 11 Nov 2022 03:35:32 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feec22237b39a1302e6c30d3859c1bcb379fb3402ff13a8404a6d54bfccc36d7`  
		Last Modified: Fri, 11 Nov 2022 03:35:32 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; s390x

```console
$ docker pull mariadb@sha256:4a591435e25485e0d6f70d402278e5d8a390f1722637aa611302b1dad6aa5c91
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123220333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b28297f6fb56ed53dce45751a20bc5f3ab94a585976cda3effcf5102950f904d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:51:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:04:47 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:04:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:05:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:05:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:05:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:07:26 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.18 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:07:26 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:07:27 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:07:27 GMT
ARG MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:07:27 GMT
ENV MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:07:28 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:07:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:08:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:08:10 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:08:10 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:08:10 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:08:10 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:08:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c5044aaae9e9803c63085684d6340fffb48767ac91fa592d662702d71aff1`  
		Last Modified: Tue, 25 Oct 2022 08:57:06 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e797e665b3dcac7015b2708bfc1e2a7e59440583bb0dc4ce190816045b7dc697`  
		Last Modified: Fri, 11 Nov 2022 03:10:38 GMT  
		Size: 6.6 MB (6609162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172ce120405e0ffc7c9898c55d47e408d08615b0d187e3dafb6c6e38feba596`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4c1eb499142bfd92c04ca2dc0c36df446c04e8e035c734bb37f390921545a5`  
		Last Modified: Fri, 11 Nov 2022 03:11:25 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290522ae60e32569f86549b3e87b60053ccd1e7db6d3be94bab6824016bc3aaf`  
		Last Modified: Fri, 11 Nov 2022 03:11:38 GMT  
		Size: 89.6 MB (89582485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3431466ec98755dda6974981005f4ff27971f80a4a8806705f45bdd9f2a3429c`  
		Last Modified: Fri, 11 Nov 2022 03:11:25 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e831a14f382a889f57143fa64d5f34390d49dde6c3b1c812af732d4d6270ad`  
		Last Modified: Fri, 11 Nov 2022 03:11:25 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:427c8a1e08b84b8dcb8256bb3e2e1608353aa7ee216bb62d682ca495069e5810
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:7dbef335ec2b32219491e718e93170598ba42bc1e7c8de77018c75ffe9824f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124186245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff56a02874cff48f63dd41974a64ecb00305e98f56f011da318079ab3a2aca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:54:53 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.18 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:54:53 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 01:54:53 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 01:54:53 GMT
ARG MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 01:54:53 GMT
ENV MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 01:54:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:54:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:55:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:55:28 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:55:28 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:55:29 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:55:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:55:29 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:55:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff10c4143de9f3ad7e4dd0d9a4cb9b28a940a5b3ffc25088a06deeec8c0bf0ce`  
		Last Modified: Fri, 11 Nov 2022 02:00:07 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86940c6e6b472adeee37ad0dfc05851e4c586adf0ac914c7eaa2088a89dd0bd2`  
		Last Modified: Fri, 11 Nov 2022 02:00:20 GMT  
		Size: 88.5 MB (88537185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb690670c568195e04ea4a7b82f19e5ae97cd9c7cff01d58fcda25d34afef844`  
		Last Modified: Fri, 11 Nov 2022 02:00:07 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c944b15571b4cca5909e3c98ad41fd5646e5a058476d4772dc89f06e8fed9`  
		Last Modified: Fri, 11 Nov 2022 02:00:07 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:75147e4a7b58fbfa6073548d3ff6a71c666f8471a82d3051b36ee7ff496e5d6f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125598592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa2997900745409815ed380f76f0f3b02a73491e05d762c6e3ee84e056538b1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 02:04:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 26 Oct 2022 02:04:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Oct 2022 02:04:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Oct 2022 02:04:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Oct 2022 02:04:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 26 Oct 2022 02:04:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 26 Oct 2022 02:06:00 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 26 Oct 2022 02:06:00 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 26 Oct 2022 02:06:00 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Wed, 26 Oct 2022 02:06:00 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Wed, 26 Oct 2022 02:06:00 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Wed, 26 Oct 2022 02:06:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 26 Oct 2022 02:06:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 26 Oct 2022 02:06:21 GMT
VOLUME [/var/lib/mysql]
# Wed, 26 Oct 2022 02:06:21 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Wed, 26 Oct 2022 02:06:22 GMT
COPY file:1cbfae6200694fb67440ab571faea87cbbd737228ff9f3193338e54312e6bd67 in /usr/local/bin/ 
# Wed, 26 Oct 2022 02:06:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 02:06:22 GMT
EXPOSE 3306
# Wed, 26 Oct 2022 02:06:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5059476c4efaaefd5639d62272cf873b43fc4dd354f29aa2d424f5672f98d7`  
		Last Modified: Wed, 26 Oct 2022 02:09:48 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b512e3647ec22a314bc3b404b44b891220289f7918fc3fb90dec28d934b622f7`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 5.5 MB (5474279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4034a198751d9b8465f987f8cd51acc3b45288510ea70f4f50588aca7ab03e`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 3.4 MB (3368397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a303c93f3f2afdbf7461aaa57d2e0376745b909ca61dc1ab04bed8a727844135`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a95ecb4d8b5c99728b7e239140c0c9127f6b8286e033494da3d7b938d10669`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 2.2 MB (2186475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c381f22b0bfdceb13b81f9105a5b0965c5d34d0a2800bc7ae58461d1661aae`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9317c133d22bf1a053a47870a13631dfaaa76e4aa19884640b0ada12d4392a`  
		Last Modified: Wed, 26 Oct 2022 02:10:44 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f30e678460e0f8e823655d65ea2b9548d676018bff8779c02d4e18849e3cfa`  
		Last Modified: Wed, 26 Oct 2022 02:10:55 GMT  
		Size: 87.4 MB (87358188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b426e3a31bb98d15adcd307617ecfcde7b58d10667ab34f285af458393b4919`  
		Last Modified: Wed, 26 Oct 2022 02:10:44 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3365d363ba6d0608da76aac797894b103b784e955279bfbdf9f58345101395d`  
		Last Modified: Wed, 26 Oct 2022 02:10:44 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5e4a81c0a27e73a31f7d73d7f6a06813d0059c9e0c30718f3e70b0630ca5e02d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.2 MB (134216051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db0f5b095527d06c59e3b2108f212aa6f4383289c68ef6e96f5f74154207ff22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:27:05 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.18 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:27:05 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:27:05 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:27:06 GMT
ARG MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:27:06 GMT
ENV MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:27:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:27:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:27:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:27:58 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:27:58 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:27:59 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:27:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:27:59 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:28:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa562e05c60903709ebe3e3a87dea9e04c63d505a87cda0033d11a09c38eb27`  
		Last Modified: Fri, 11 Nov 2022 03:35:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5619a4518dc98a993a8a8f4ce937b5755bea84cc79ca51782c0ddab754139ea`  
		Last Modified: Fri, 11 Nov 2022 03:35:57 GMT  
		Size: 93.1 MB (93137159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95ce40dabcc6107f427cdcaaadd7821252fad6a92798da43b93a85977a2d582`  
		Last Modified: Fri, 11 Nov 2022 03:35:32 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feec22237b39a1302e6c30d3859c1bcb379fb3402ff13a8404a6d54bfccc36d7`  
		Last Modified: Fri, 11 Nov 2022 03:35:32 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:4a591435e25485e0d6f70d402278e5d8a390f1722637aa611302b1dad6aa5c91
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123220333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b28297f6fb56ed53dce45751a20bc5f3ab94a585976cda3effcf5102950f904d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:51:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:04:47 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:04:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:05:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:05:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:05:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:07:26 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.18 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:07:26 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:07:27 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:07:27 GMT
ARG MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:07:27 GMT
ENV MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:07:28 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:07:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:08:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:08:10 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:08:10 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:08:10 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:08:10 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:08:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c5044aaae9e9803c63085684d6340fffb48767ac91fa592d662702d71aff1`  
		Last Modified: Tue, 25 Oct 2022 08:57:06 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e797e665b3dcac7015b2708bfc1e2a7e59440583bb0dc4ce190816045b7dc697`  
		Last Modified: Fri, 11 Nov 2022 03:10:38 GMT  
		Size: 6.6 MB (6609162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172ce120405e0ffc7c9898c55d47e408d08615b0d187e3dafb6c6e38feba596`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4c1eb499142bfd92c04ca2dc0c36df446c04e8e035c734bb37f390921545a5`  
		Last Modified: Fri, 11 Nov 2022 03:11:25 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290522ae60e32569f86549b3e87b60053ccd1e7db6d3be94bab6824016bc3aaf`  
		Last Modified: Fri, 11 Nov 2022 03:11:38 GMT  
		Size: 89.6 MB (89582485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3431466ec98755dda6974981005f4ff27971f80a4a8806705f45bdd9f2a3429c`  
		Last Modified: Fri, 11 Nov 2022 03:11:25 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e831a14f382a889f57143fa64d5f34390d49dde6c3b1c812af732d4d6270ad`  
		Last Modified: Fri, 11 Nov 2022 03:11:25 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.18`

```console
$ docker pull mariadb@sha256:ee159af7e76fc4cbd406eae2bd3ce655fa10d6f0a510f234ba641343ed844c67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.18` - linux; amd64

```console
$ docker pull mariadb@sha256:7dbef335ec2b32219491e718e93170598ba42bc1e7c8de77018c75ffe9824f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124186245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff56a02874cff48f63dd41974a64ecb00305e98f56f011da318079ab3a2aca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:54:53 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.18 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:54:53 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 01:54:53 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 01:54:53 GMT
ARG MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 01:54:53 GMT
ENV MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 01:54:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:54:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:55:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:55:28 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:55:28 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:55:29 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:55:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:55:29 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:55:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff10c4143de9f3ad7e4dd0d9a4cb9b28a940a5b3ffc25088a06deeec8c0bf0ce`  
		Last Modified: Fri, 11 Nov 2022 02:00:07 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86940c6e6b472adeee37ad0dfc05851e4c586adf0ac914c7eaa2088a89dd0bd2`  
		Last Modified: Fri, 11 Nov 2022 02:00:20 GMT  
		Size: 88.5 MB (88537185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb690670c568195e04ea4a7b82f19e5ae97cd9c7cff01d58fcda25d34afef844`  
		Last Modified: Fri, 11 Nov 2022 02:00:07 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c944b15571b4cca5909e3c98ad41fd5646e5a058476d4772dc89f06e8fed9`  
		Last Modified: Fri, 11 Nov 2022 02:00:07 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.18` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5e4a81c0a27e73a31f7d73d7f6a06813d0059c9e0c30718f3e70b0630ca5e02d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.2 MB (134216051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db0f5b095527d06c59e3b2108f212aa6f4383289c68ef6e96f5f74154207ff22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:27:05 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.18 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:27:05 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:27:05 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:27:06 GMT
ARG MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:27:06 GMT
ENV MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:27:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:27:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:27:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:27:58 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:27:58 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:27:59 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:27:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:27:59 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:28:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa562e05c60903709ebe3e3a87dea9e04c63d505a87cda0033d11a09c38eb27`  
		Last Modified: Fri, 11 Nov 2022 03:35:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5619a4518dc98a993a8a8f4ce937b5755bea84cc79ca51782c0ddab754139ea`  
		Last Modified: Fri, 11 Nov 2022 03:35:57 GMT  
		Size: 93.1 MB (93137159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95ce40dabcc6107f427cdcaaadd7821252fad6a92798da43b93a85977a2d582`  
		Last Modified: Fri, 11 Nov 2022 03:35:32 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feec22237b39a1302e6c30d3859c1bcb379fb3402ff13a8404a6d54bfccc36d7`  
		Last Modified: Fri, 11 Nov 2022 03:35:32 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.18` - linux; s390x

```console
$ docker pull mariadb@sha256:4a591435e25485e0d6f70d402278e5d8a390f1722637aa611302b1dad6aa5c91
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123220333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b28297f6fb56ed53dce45751a20bc5f3ab94a585976cda3effcf5102950f904d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:51:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:04:47 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:04:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:05:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:05:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:05:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:07:26 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.18 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:07:26 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:07:27 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:07:27 GMT
ARG MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:07:27 GMT
ENV MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:07:28 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:07:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:08:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:08:10 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:08:10 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:08:10 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:08:10 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:08:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c5044aaae9e9803c63085684d6340fffb48767ac91fa592d662702d71aff1`  
		Last Modified: Tue, 25 Oct 2022 08:57:06 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e797e665b3dcac7015b2708bfc1e2a7e59440583bb0dc4ce190816045b7dc697`  
		Last Modified: Fri, 11 Nov 2022 03:10:38 GMT  
		Size: 6.6 MB (6609162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172ce120405e0ffc7c9898c55d47e408d08615b0d187e3dafb6c6e38feba596`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4c1eb499142bfd92c04ca2dc0c36df446c04e8e035c734bb37f390921545a5`  
		Last Modified: Fri, 11 Nov 2022 03:11:25 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290522ae60e32569f86549b3e87b60053ccd1e7db6d3be94bab6824016bc3aaf`  
		Last Modified: Fri, 11 Nov 2022 03:11:38 GMT  
		Size: 89.6 MB (89582485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3431466ec98755dda6974981005f4ff27971f80a4a8806705f45bdd9f2a3429c`  
		Last Modified: Fri, 11 Nov 2022 03:11:25 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e831a14f382a889f57143fa64d5f34390d49dde6c3b1c812af732d4d6270ad`  
		Last Modified: Fri, 11 Nov 2022 03:11:25 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.18-focal`

```console
$ docker pull mariadb@sha256:ee159af7e76fc4cbd406eae2bd3ce655fa10d6f0a510f234ba641343ed844c67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.18-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:7dbef335ec2b32219491e718e93170598ba42bc1e7c8de77018c75ffe9824f40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124186245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff56a02874cff48f63dd41974a64ecb00305e98f56f011da318079ab3a2aca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:54:53 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.18 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:54:53 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 01:54:53 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 01:54:53 GMT
ARG MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 01:54:53 GMT
ENV MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 01:54:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:54:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:55:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:55:28 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:55:28 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:55:29 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:55:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:55:29 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:55:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff10c4143de9f3ad7e4dd0d9a4cb9b28a940a5b3ffc25088a06deeec8c0bf0ce`  
		Last Modified: Fri, 11 Nov 2022 02:00:07 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86940c6e6b472adeee37ad0dfc05851e4c586adf0ac914c7eaa2088a89dd0bd2`  
		Last Modified: Fri, 11 Nov 2022 02:00:20 GMT  
		Size: 88.5 MB (88537185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb690670c568195e04ea4a7b82f19e5ae97cd9c7cff01d58fcda25d34afef844`  
		Last Modified: Fri, 11 Nov 2022 02:00:07 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c944b15571b4cca5909e3c98ad41fd5646e5a058476d4772dc89f06e8fed9`  
		Last Modified: Fri, 11 Nov 2022 02:00:07 GMT  
		Size: 6.9 KB (6946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.18-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5e4a81c0a27e73a31f7d73d7f6a06813d0059c9e0c30718f3e70b0630ca5e02d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.2 MB (134216051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db0f5b095527d06c59e3b2108f212aa6f4383289c68ef6e96f5f74154207ff22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:27:05 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.18 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:27:05 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:27:05 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:27:06 GMT
ARG MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:27:06 GMT
ENV MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:27:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:27:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:27:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:27:58 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:27:58 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:27:59 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:27:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:27:59 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:28:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa562e05c60903709ebe3e3a87dea9e04c63d505a87cda0033d11a09c38eb27`  
		Last Modified: Fri, 11 Nov 2022 03:35:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5619a4518dc98a993a8a8f4ce937b5755bea84cc79ca51782c0ddab754139ea`  
		Last Modified: Fri, 11 Nov 2022 03:35:57 GMT  
		Size: 93.1 MB (93137159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95ce40dabcc6107f427cdcaaadd7821252fad6a92798da43b93a85977a2d582`  
		Last Modified: Fri, 11 Nov 2022 03:35:32 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feec22237b39a1302e6c30d3859c1bcb379fb3402ff13a8404a6d54bfccc36d7`  
		Last Modified: Fri, 11 Nov 2022 03:35:32 GMT  
		Size: 6.9 KB (6948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.18-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:4a591435e25485e0d6f70d402278e5d8a390f1722637aa611302b1dad6aa5c91
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123220333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b28297f6fb56ed53dce45751a20bc5f3ab94a585976cda3effcf5102950f904d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:51:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:04:47 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:04:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:05:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:05:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:05:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:07:26 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.5.18 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:07:26 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:07:27 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 11 Nov 2022 03:07:27 GMT
ARG MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:07:27 GMT
ENV MARIADB_VERSION=1:10.5.18+maria~ubu2004
# Fri, 11 Nov 2022 03:07:28 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:07:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:08:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.18/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:08:10 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:08:10 GMT
COPY file:d1ef29581ac31aa4bb2834dc97545a6c5a3ee728dfcb95fd3598dfb219fdbae2 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:08:10 GMT
COPY file:a20d2f4de06cbd6bb5b32b07e5ddff51f8660c1cbb71d7a08ae07c03fee2ca23 in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:08:10 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:08:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c5044aaae9e9803c63085684d6340fffb48767ac91fa592d662702d71aff1`  
		Last Modified: Tue, 25 Oct 2022 08:57:06 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e797e665b3dcac7015b2708bfc1e2a7e59440583bb0dc4ce190816045b7dc697`  
		Last Modified: Fri, 11 Nov 2022 03:10:38 GMT  
		Size: 6.6 MB (6609162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172ce120405e0ffc7c9898c55d47e408d08615b0d187e3dafb6c6e38feba596`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4c1eb499142bfd92c04ca2dc0c36df446c04e8e035c734bb37f390921545a5`  
		Last Modified: Fri, 11 Nov 2022 03:11:25 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290522ae60e32569f86549b3e87b60053ccd1e7db6d3be94bab6824016bc3aaf`  
		Last Modified: Fri, 11 Nov 2022 03:11:38 GMT  
		Size: 89.6 MB (89582485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3431466ec98755dda6974981005f4ff27971f80a4a8806705f45bdd9f2a3429c`  
		Last Modified: Fri, 11 Nov 2022 03:11:25 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e831a14f382a889f57143fa64d5f34390d49dde6c3b1c812af732d4d6270ad`  
		Last Modified: Fri, 11 Nov 2022 03:11:25 GMT  
		Size: 6.9 KB (6943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:7c205ccfc7ee76df7b5dec3f6622cf67b86174108e7c3d2bbf86a551fa9742d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:ebccdc459d1ce2ba66c059e04c2a08a3492dac725ce67de56e9b1df8ff8eb6fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124522623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a62052ec34aae490abf35935ded23fba9883587aade6bd5246b7157780123e6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:54:12 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.11 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:54:12 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 01:54:13 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 01:54:13 GMT
ARG MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 01:54:13 GMT
ENV MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 01:54:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:54:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:54:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:54:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:54:47 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:54:47 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:54:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:54:47 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:54:47 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5e88c034ffbaf266a05262f08f7f9bde72b1e74b96d5181053c04d8d0843f8`  
		Last Modified: Fri, 11 Nov 2022 01:59:37 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09b3c6023668be566065d638891e53842370b25a83c884957f078c582bd297f`  
		Last Modified: Fri, 11 Nov 2022 01:59:50 GMT  
		Size: 88.9 MB (88873565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9896f95913b8f606ae2ff63227c21bef2c6adcdc19cac4ed807b7bf7d559a61f`  
		Last Modified: Fri, 11 Nov 2022 01:59:37 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad640b19225b4117f87d139ea72fb0b7c5a57faa252ee8aa8680af3e74cd96d`  
		Last Modified: Fri, 11 Nov 2022 01:59:37 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2a4f16d88b588f35d86e3f1c1ad18d0ff236715aa47a8429ffe91d21c2cd7919
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125656180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7eec748da3421b54980609f12fcf11ede45e59de3d5918644524c3b458f8010`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 02:04:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 26 Oct 2022 02:04:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Oct 2022 02:04:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Oct 2022 02:04:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Oct 2022 02:04:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 26 Oct 2022 02:04:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 26 Oct 2022 02:05:36 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 26 Oct 2022 02:05:36 GMT
ENV MARIADB_MAJOR=10.6
# Wed, 26 Oct 2022 02:05:36 GMT
ARG MARIADB_VERSION=1:10.6.10+maria~ubu2004
# Wed, 26 Oct 2022 02:05:36 GMT
ENV MARIADB_VERSION=1:10.6.10+maria~ubu2004
# Wed, 26 Oct 2022 02:05:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.10/repo/ubuntu/ focal main
# Wed, 26 Oct 2022 02:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.10/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 26 Oct 2022 02:05:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.10/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 26 Oct 2022 02:05:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 26 Oct 2022 02:05:57 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 26 Oct 2022 02:05:57 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 26 Oct 2022 02:05:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 02:05:57 GMT
EXPOSE 3306
# Wed, 26 Oct 2022 02:05:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5059476c4efaaefd5639d62272cf873b43fc4dd354f29aa2d424f5672f98d7`  
		Last Modified: Wed, 26 Oct 2022 02:09:48 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b512e3647ec22a314bc3b404b44b891220289f7918fc3fb90dec28d934b622f7`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 5.5 MB (5474279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4034a198751d9b8465f987f8cd51acc3b45288510ea70f4f50588aca7ab03e`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 3.4 MB (3368397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a303c93f3f2afdbf7461aaa57d2e0376745b909ca61dc1ab04bed8a727844135`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a95ecb4d8b5c99728b7e239140c0c9127f6b8286e033494da3d7b938d10669`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 2.2 MB (2186475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c381f22b0bfdceb13b81f9105a5b0965c5d34d0a2800bc7ae58461d1661aae`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb80a602c36bdad83f2a5208bdb9c55afd09d123f55e4a001d82579340f5c4d4`  
		Last Modified: Wed, 26 Oct 2022 02:10:13 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded0a0306f3bc15969e0b35a7782db48ddd8b3e77abd90e2407ad3dabc91238e`  
		Last Modified: Wed, 26 Oct 2022 02:10:23 GMT  
		Size: 87.4 MB (87415771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb00dea3c2afef8409982977b52d0e8271c4189878780038deaa1a7633ad4181`  
		Last Modified: Wed, 26 Oct 2022 02:10:12 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96961d266794c3ecf3e736699988bec9d35bfde44628b7406d4c656b09069bc`  
		Last Modified: Wed, 26 Oct 2022 02:10:12 GMT  
		Size: 7.1 KB (7052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:48aa52ef462938f4d96b58eb5cf0efda202eca536e6021adb18de746f1de55bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134324726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0fad581f0806c831896ff0e7a5ae0fa627b2bdc7eeea2ac9f5622c717eea75d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:25:54 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.11 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:25:54 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:25:55 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:25:56 GMT
ARG MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:25:57 GMT
ENV MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:25:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:25:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:26:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:26:51 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:26:52 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:26:52 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:26:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:26:53 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:26:53 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39e1f77fba8c984d86b412fec04f2fd9fbf70f6ff910b25d45015173310623a`  
		Last Modified: Fri, 11 Nov 2022 03:34:48 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a17089079d80596538ac3139de05dd005505ed086e6f8278fe2d224de9beb1`  
		Last Modified: Fri, 11 Nov 2022 03:35:13 GMT  
		Size: 93.2 MB (93245841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a5411ec2782ac6dcc1e8473683d51b6d02f802f3223350f3809774db0bd248`  
		Last Modified: Fri, 11 Nov 2022 03:34:48 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d16b7767429ebe554190ec59fcac7b7431a3218d1779f27fd7fefef95397bee`  
		Last Modified: Fri, 11 Nov 2022 03:34:48 GMT  
		Size: 6.9 KB (6949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; s390x

```console
$ docker pull mariadb@sha256:60b0b4d1171fe87add79aae91f3e2f455c1d485a8c27f86c59068b6588b44b7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123302041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c4d33387a45a35d1c9ddae4cb1f346f7c5a57a4d08976ad7ac576cc85966c9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:51:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:04:47 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:04:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:05:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:05:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:05:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:06:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.11 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:06:07 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:06:07 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:06:07 GMT
ARG MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:06:07 GMT
ENV MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:06:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:06:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:06:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:07:09 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:07:10 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:07:10 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:07:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:07:11 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:07:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c5044aaae9e9803c63085684d6340fffb48767ac91fa592d662702d71aff1`  
		Last Modified: Tue, 25 Oct 2022 08:57:06 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e797e665b3dcac7015b2708bfc1e2a7e59440583bb0dc4ce190816045b7dc697`  
		Last Modified: Fri, 11 Nov 2022 03:10:38 GMT  
		Size: 6.6 MB (6609162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172ce120405e0ffc7c9898c55d47e408d08615b0d187e3dafb6c6e38feba596`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444f223ece80801d19b0b72d27fa2058629c813072bed3847817a07ab61a8fca`  
		Last Modified: Fri, 11 Nov 2022 03:11:00 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e764c20949f8f71f7df4a334f195afbb8015bdbc6606f89d2b7e1403f7f0226`  
		Last Modified: Fri, 11 Nov 2022 03:11:14 GMT  
		Size: 89.7 MB (89664190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92197e38b94ae3062778f8cbc9b6763c4681084ea2f5239f49a792427415c094`  
		Last Modified: Fri, 11 Nov 2022 03:11:00 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcebf76a2664f3c9d201cdb9f349bda04af73438c716cb5221b93afe43b0ec4c`  
		Last Modified: Fri, 11 Nov 2022 03:11:00 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:7c205ccfc7ee76df7b5dec3f6622cf67b86174108e7c3d2bbf86a551fa9742d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:ebccdc459d1ce2ba66c059e04c2a08a3492dac725ce67de56e9b1df8ff8eb6fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124522623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a62052ec34aae490abf35935ded23fba9883587aade6bd5246b7157780123e6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:54:12 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.11 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:54:12 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 01:54:13 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 01:54:13 GMT
ARG MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 01:54:13 GMT
ENV MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 01:54:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:54:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:54:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:54:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:54:47 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:54:47 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:54:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:54:47 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:54:47 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5e88c034ffbaf266a05262f08f7f9bde72b1e74b96d5181053c04d8d0843f8`  
		Last Modified: Fri, 11 Nov 2022 01:59:37 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09b3c6023668be566065d638891e53842370b25a83c884957f078c582bd297f`  
		Last Modified: Fri, 11 Nov 2022 01:59:50 GMT  
		Size: 88.9 MB (88873565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9896f95913b8f606ae2ff63227c21bef2c6adcdc19cac4ed807b7bf7d559a61f`  
		Last Modified: Fri, 11 Nov 2022 01:59:37 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad640b19225b4117f87d139ea72fb0b7c5a57faa252ee8aa8680af3e74cd96d`  
		Last Modified: Fri, 11 Nov 2022 01:59:37 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2a4f16d88b588f35d86e3f1c1ad18d0ff236715aa47a8429ffe91d21c2cd7919
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125656180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7eec748da3421b54980609f12fcf11ede45e59de3d5918644524c3b458f8010`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 02:04:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 26 Oct 2022 02:04:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Oct 2022 02:04:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Oct 2022 02:04:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Oct 2022 02:04:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 26 Oct 2022 02:04:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 26 Oct 2022 02:05:36 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 26 Oct 2022 02:05:36 GMT
ENV MARIADB_MAJOR=10.6
# Wed, 26 Oct 2022 02:05:36 GMT
ARG MARIADB_VERSION=1:10.6.10+maria~ubu2004
# Wed, 26 Oct 2022 02:05:36 GMT
ENV MARIADB_VERSION=1:10.6.10+maria~ubu2004
# Wed, 26 Oct 2022 02:05:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.10/repo/ubuntu/ focal main
# Wed, 26 Oct 2022 02:05:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.10/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 26 Oct 2022 02:05:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.10/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 26 Oct 2022 02:05:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 26 Oct 2022 02:05:57 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 26 Oct 2022 02:05:57 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 26 Oct 2022 02:05:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 02:05:57 GMT
EXPOSE 3306
# Wed, 26 Oct 2022 02:05:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5059476c4efaaefd5639d62272cf873b43fc4dd354f29aa2d424f5672f98d7`  
		Last Modified: Wed, 26 Oct 2022 02:09:48 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b512e3647ec22a314bc3b404b44b891220289f7918fc3fb90dec28d934b622f7`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 5.5 MB (5474279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4034a198751d9b8465f987f8cd51acc3b45288510ea70f4f50588aca7ab03e`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 3.4 MB (3368397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a303c93f3f2afdbf7461aaa57d2e0376745b909ca61dc1ab04bed8a727844135`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a95ecb4d8b5c99728b7e239140c0c9127f6b8286e033494da3d7b938d10669`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 2.2 MB (2186475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c381f22b0bfdceb13b81f9105a5b0965c5d34d0a2800bc7ae58461d1661aae`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb80a602c36bdad83f2a5208bdb9c55afd09d123f55e4a001d82579340f5c4d4`  
		Last Modified: Wed, 26 Oct 2022 02:10:13 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded0a0306f3bc15969e0b35a7782db48ddd8b3e77abd90e2407ad3dabc91238e`  
		Last Modified: Wed, 26 Oct 2022 02:10:23 GMT  
		Size: 87.4 MB (87415771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb00dea3c2afef8409982977b52d0e8271c4189878780038deaa1a7633ad4181`  
		Last Modified: Wed, 26 Oct 2022 02:10:12 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96961d266794c3ecf3e736699988bec9d35bfde44628b7406d4c656b09069bc`  
		Last Modified: Wed, 26 Oct 2022 02:10:12 GMT  
		Size: 7.1 KB (7052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:48aa52ef462938f4d96b58eb5cf0efda202eca536e6021adb18de746f1de55bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134324726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0fad581f0806c831896ff0e7a5ae0fa627b2bdc7eeea2ac9f5622c717eea75d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:25:54 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.11 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:25:54 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:25:55 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:25:56 GMT
ARG MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:25:57 GMT
ENV MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:25:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:25:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:26:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:26:51 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:26:52 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:26:52 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:26:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:26:53 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:26:53 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39e1f77fba8c984d86b412fec04f2fd9fbf70f6ff910b25d45015173310623a`  
		Last Modified: Fri, 11 Nov 2022 03:34:48 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a17089079d80596538ac3139de05dd005505ed086e6f8278fe2d224de9beb1`  
		Last Modified: Fri, 11 Nov 2022 03:35:13 GMT  
		Size: 93.2 MB (93245841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a5411ec2782ac6dcc1e8473683d51b6d02f802f3223350f3809774db0bd248`  
		Last Modified: Fri, 11 Nov 2022 03:34:48 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d16b7767429ebe554190ec59fcac7b7431a3218d1779f27fd7fefef95397bee`  
		Last Modified: Fri, 11 Nov 2022 03:34:48 GMT  
		Size: 6.9 KB (6949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:60b0b4d1171fe87add79aae91f3e2f455c1d485a8c27f86c59068b6588b44b7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123302041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c4d33387a45a35d1c9ddae4cb1f346f7c5a57a4d08976ad7ac576cc85966c9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:51:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:04:47 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:04:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:05:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:05:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:05:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:06:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.11 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:06:07 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:06:07 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:06:07 GMT
ARG MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:06:07 GMT
ENV MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:06:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:06:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:06:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:07:09 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:07:10 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:07:10 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:07:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:07:11 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:07:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c5044aaae9e9803c63085684d6340fffb48767ac91fa592d662702d71aff1`  
		Last Modified: Tue, 25 Oct 2022 08:57:06 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e797e665b3dcac7015b2708bfc1e2a7e59440583bb0dc4ce190816045b7dc697`  
		Last Modified: Fri, 11 Nov 2022 03:10:38 GMT  
		Size: 6.6 MB (6609162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172ce120405e0ffc7c9898c55d47e408d08615b0d187e3dafb6c6e38feba596`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444f223ece80801d19b0b72d27fa2058629c813072bed3847817a07ab61a8fca`  
		Last Modified: Fri, 11 Nov 2022 03:11:00 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e764c20949f8f71f7df4a334f195afbb8015bdbc6606f89d2b7e1403f7f0226`  
		Last Modified: Fri, 11 Nov 2022 03:11:14 GMT  
		Size: 89.7 MB (89664190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92197e38b94ae3062778f8cbc9b6763c4681084ea2f5239f49a792427415c094`  
		Last Modified: Fri, 11 Nov 2022 03:11:00 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcebf76a2664f3c9d201cdb9f349bda04af73438c716cb5221b93afe43b0ec4c`  
		Last Modified: Fri, 11 Nov 2022 03:11:00 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.11`

```console
$ docker pull mariadb@sha256:40d12211272e62c1132caed63e6d3f092e7020ed4948a7e49015067497dd7197
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.11` - linux; amd64

```console
$ docker pull mariadb@sha256:ebccdc459d1ce2ba66c059e04c2a08a3492dac725ce67de56e9b1df8ff8eb6fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124522623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a62052ec34aae490abf35935ded23fba9883587aade6bd5246b7157780123e6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:54:12 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.11 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:54:12 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 01:54:13 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 01:54:13 GMT
ARG MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 01:54:13 GMT
ENV MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 01:54:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:54:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:54:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:54:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:54:47 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:54:47 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:54:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:54:47 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:54:47 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5e88c034ffbaf266a05262f08f7f9bde72b1e74b96d5181053c04d8d0843f8`  
		Last Modified: Fri, 11 Nov 2022 01:59:37 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09b3c6023668be566065d638891e53842370b25a83c884957f078c582bd297f`  
		Last Modified: Fri, 11 Nov 2022 01:59:50 GMT  
		Size: 88.9 MB (88873565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9896f95913b8f606ae2ff63227c21bef2c6adcdc19cac4ed807b7bf7d559a61f`  
		Last Modified: Fri, 11 Nov 2022 01:59:37 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad640b19225b4117f87d139ea72fb0b7c5a57faa252ee8aa8680af3e74cd96d`  
		Last Modified: Fri, 11 Nov 2022 01:59:37 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.11` - linux; ppc64le

```console
$ docker pull mariadb@sha256:48aa52ef462938f4d96b58eb5cf0efda202eca536e6021adb18de746f1de55bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134324726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0fad581f0806c831896ff0e7a5ae0fa627b2bdc7eeea2ac9f5622c717eea75d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:25:54 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.11 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:25:54 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:25:55 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:25:56 GMT
ARG MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:25:57 GMT
ENV MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:25:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:25:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:26:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:26:51 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:26:52 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:26:52 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:26:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:26:53 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:26:53 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39e1f77fba8c984d86b412fec04f2fd9fbf70f6ff910b25d45015173310623a`  
		Last Modified: Fri, 11 Nov 2022 03:34:48 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a17089079d80596538ac3139de05dd005505ed086e6f8278fe2d224de9beb1`  
		Last Modified: Fri, 11 Nov 2022 03:35:13 GMT  
		Size: 93.2 MB (93245841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a5411ec2782ac6dcc1e8473683d51b6d02f802f3223350f3809774db0bd248`  
		Last Modified: Fri, 11 Nov 2022 03:34:48 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d16b7767429ebe554190ec59fcac7b7431a3218d1779f27fd7fefef95397bee`  
		Last Modified: Fri, 11 Nov 2022 03:34:48 GMT  
		Size: 6.9 KB (6949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.11` - linux; s390x

```console
$ docker pull mariadb@sha256:60b0b4d1171fe87add79aae91f3e2f455c1d485a8c27f86c59068b6588b44b7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123302041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c4d33387a45a35d1c9ddae4cb1f346f7c5a57a4d08976ad7ac576cc85966c9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:51:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:04:47 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:04:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:05:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:05:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:05:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:06:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.11 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:06:07 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:06:07 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:06:07 GMT
ARG MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:06:07 GMT
ENV MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:06:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:06:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:06:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:07:09 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:07:10 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:07:10 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:07:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:07:11 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:07:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c5044aaae9e9803c63085684d6340fffb48767ac91fa592d662702d71aff1`  
		Last Modified: Tue, 25 Oct 2022 08:57:06 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e797e665b3dcac7015b2708bfc1e2a7e59440583bb0dc4ce190816045b7dc697`  
		Last Modified: Fri, 11 Nov 2022 03:10:38 GMT  
		Size: 6.6 MB (6609162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172ce120405e0ffc7c9898c55d47e408d08615b0d187e3dafb6c6e38feba596`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444f223ece80801d19b0b72d27fa2058629c813072bed3847817a07ab61a8fca`  
		Last Modified: Fri, 11 Nov 2022 03:11:00 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e764c20949f8f71f7df4a334f195afbb8015bdbc6606f89d2b7e1403f7f0226`  
		Last Modified: Fri, 11 Nov 2022 03:11:14 GMT  
		Size: 89.7 MB (89664190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92197e38b94ae3062778f8cbc9b6763c4681084ea2f5239f49a792427415c094`  
		Last Modified: Fri, 11 Nov 2022 03:11:00 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcebf76a2664f3c9d201cdb9f349bda04af73438c716cb5221b93afe43b0ec4c`  
		Last Modified: Fri, 11 Nov 2022 03:11:00 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.11-focal`

```console
$ docker pull mariadb@sha256:40d12211272e62c1132caed63e6d3f092e7020ed4948a7e49015067497dd7197
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.11-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:ebccdc459d1ce2ba66c059e04c2a08a3492dac725ce67de56e9b1df8ff8eb6fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124522623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a62052ec34aae490abf35935ded23fba9883587aade6bd5246b7157780123e6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:54:12 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.11 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:54:12 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 01:54:13 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 01:54:13 GMT
ARG MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 01:54:13 GMT
ENV MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 01:54:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:54:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:54:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:54:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:54:47 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:54:47 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:54:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:54:47 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:54:47 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5e88c034ffbaf266a05262f08f7f9bde72b1e74b96d5181053c04d8d0843f8`  
		Last Modified: Fri, 11 Nov 2022 01:59:37 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09b3c6023668be566065d638891e53842370b25a83c884957f078c582bd297f`  
		Last Modified: Fri, 11 Nov 2022 01:59:50 GMT  
		Size: 88.9 MB (88873565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9896f95913b8f606ae2ff63227c21bef2c6adcdc19cac4ed807b7bf7d559a61f`  
		Last Modified: Fri, 11 Nov 2022 01:59:37 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad640b19225b4117f87d139ea72fb0b7c5a57faa252ee8aa8680af3e74cd96d`  
		Last Modified: Fri, 11 Nov 2022 01:59:37 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.11-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:48aa52ef462938f4d96b58eb5cf0efda202eca536e6021adb18de746f1de55bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134324726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0fad581f0806c831896ff0e7a5ae0fa627b2bdc7eeea2ac9f5622c717eea75d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:25:54 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.11 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:25:54 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:25:55 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:25:56 GMT
ARG MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:25:57 GMT
ENV MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:25:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:25:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:26:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:26:51 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:26:52 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:26:52 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:26:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:26:53 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:26:53 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39e1f77fba8c984d86b412fec04f2fd9fbf70f6ff910b25d45015173310623a`  
		Last Modified: Fri, 11 Nov 2022 03:34:48 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a17089079d80596538ac3139de05dd005505ed086e6f8278fe2d224de9beb1`  
		Last Modified: Fri, 11 Nov 2022 03:35:13 GMT  
		Size: 93.2 MB (93245841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a5411ec2782ac6dcc1e8473683d51b6d02f802f3223350f3809774db0bd248`  
		Last Modified: Fri, 11 Nov 2022 03:34:48 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d16b7767429ebe554190ec59fcac7b7431a3218d1779f27fd7fefef95397bee`  
		Last Modified: Fri, 11 Nov 2022 03:34:48 GMT  
		Size: 6.9 KB (6949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.11-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:60b0b4d1171fe87add79aae91f3e2f455c1d485a8c27f86c59068b6588b44b7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123302041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c4d33387a45a35d1c9ddae4cb1f346f7c5a57a4d08976ad7ac576cc85966c9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:51:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:04:47 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:04:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:05:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:05:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:05:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:06:06 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.6.11 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:06:07 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:06:07 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 11 Nov 2022 03:06:07 GMT
ARG MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:06:07 GMT
ENV MARIADB_VERSION=1:10.6.11+maria~ubu2004
# Fri, 11 Nov 2022 03:06:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:06:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:06:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:07:09 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:07:10 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:07:10 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:07:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:07:11 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:07:11 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c5044aaae9e9803c63085684d6340fffb48767ac91fa592d662702d71aff1`  
		Last Modified: Tue, 25 Oct 2022 08:57:06 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e797e665b3dcac7015b2708bfc1e2a7e59440583bb0dc4ce190816045b7dc697`  
		Last Modified: Fri, 11 Nov 2022 03:10:38 GMT  
		Size: 6.6 MB (6609162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172ce120405e0ffc7c9898c55d47e408d08615b0d187e3dafb6c6e38feba596`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444f223ece80801d19b0b72d27fa2058629c813072bed3847817a07ab61a8fca`  
		Last Modified: Fri, 11 Nov 2022 03:11:00 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e764c20949f8f71f7df4a334f195afbb8015bdbc6606f89d2b7e1403f7f0226`  
		Last Modified: Fri, 11 Nov 2022 03:11:14 GMT  
		Size: 89.7 MB (89664190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92197e38b94ae3062778f8cbc9b6763c4681084ea2f5239f49a792427415c094`  
		Last Modified: Fri, 11 Nov 2022 03:11:00 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcebf76a2664f3c9d201cdb9f349bda04af73438c716cb5221b93afe43b0ec4c`  
		Last Modified: Fri, 11 Nov 2022 03:11:00 GMT  
		Size: 6.9 KB (6947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7`

```console
$ docker pull mariadb@sha256:237ebc09a1f3447ffccfcf2e0f638405ca5c31515d57d797dc4f01b6f2548c2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7` - linux; amd64

```console
$ docker pull mariadb@sha256:cfb614d5a9c5befd2438d996fc50197ec6a8c3fd91a66f55e2baa79a477eb903
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125004791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41ed88878a8e3f0bf043eeb7480f859f83742b39c5929e53bda8dacaebce0bd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:52:47 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.7.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:52:47 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 01:52:47 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 01:52:47 GMT
ARG MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 01:52:47 GMT
ENV MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 01:52:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:52:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:53:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:54:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:54:00 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:54:00 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:54:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:54:00 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:54:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f3842c61594161a6ca84cb0f7b12e885dbb45c556ddf4cbf1ce79fc70e779c`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ef296df01678ff544a14617156e7e555e8bf30a3a40c906509012f1e99fb73`  
		Last Modified: Fri, 11 Nov 2022 01:59:21 GMT  
		Size: 89.4 MB (89355727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b81fc14995cdef8ab793a00b3219bd7c062a9ee8aa2192d7e1906402f4afca`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f85c6b03d8a9c90ab88f7f0b9c5826ae1e571047821250d7a13d8434250d38`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 7.0 KB (6953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:87a98538fd9b4cbbe6741e040e4fdad13c497012b35cc2012639955e25de1eb2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126160016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e91f3cd238ac241f4e4da3b1caf3e14ea8792c13440e97d7dc5cc9f976f1f5ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 02:04:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 26 Oct 2022 02:04:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Oct 2022 02:04:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Oct 2022 02:04:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Oct 2022 02:04:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 26 Oct 2022 02:04:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 26 Oct 2022 02:04:46 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 26 Oct 2022 02:04:46 GMT
ENV MARIADB_MAJOR=10.7
# Wed, 26 Oct 2022 02:04:46 GMT
ARG MARIADB_VERSION=1:10.7.6+maria~ubu2004
# Wed, 26 Oct 2022 02:04:46 GMT
ENV MARIADB_VERSION=1:10.7.6+maria~ubu2004
# Wed, 26 Oct 2022 02:04:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.6/repo/ubuntu/ focal main
# Wed, 26 Oct 2022 02:04:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.6/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 26 Oct 2022 02:05:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.6/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 26 Oct 2022 02:05:25 GMT
VOLUME [/var/lib/mysql]
# Wed, 26 Oct 2022 02:05:26 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 26 Oct 2022 02:05:26 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 26 Oct 2022 02:05:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 02:05:26 GMT
EXPOSE 3306
# Wed, 26 Oct 2022 02:05:26 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5059476c4efaaefd5639d62272cf873b43fc4dd354f29aa2d424f5672f98d7`  
		Last Modified: Wed, 26 Oct 2022 02:09:48 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b512e3647ec22a314bc3b404b44b891220289f7918fc3fb90dec28d934b622f7`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 5.5 MB (5474279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4034a198751d9b8465f987f8cd51acc3b45288510ea70f4f50588aca7ab03e`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 3.4 MB (3368397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a303c93f3f2afdbf7461aaa57d2e0376745b909ca61dc1ab04bed8a727844135`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a95ecb4d8b5c99728b7e239140c0c9127f6b8286e033494da3d7b938d10669`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 2.2 MB (2186475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c381f22b0bfdceb13b81f9105a5b0965c5d34d0a2800bc7ae58461d1661aae`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e285a7096945cbc4dbb08b241e3e872668020d36c615adc856668a633722ffb`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d1d716822a5771930e74151a206729f0a0c4a01df00dd92c2ee3469f43f9f5`  
		Last Modified: Wed, 26 Oct 2022 02:09:54 GMT  
		Size: 87.9 MB (87919613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e9ea41ac711c364318e34a2f5d8ca8bea481e0ba0efd241c162a6260c0b6c0`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a3527aa4cc989f38e19d428becfb3ad46ab44e94e58598f3463af18fe21ec0`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 7.0 KB (7048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a2f59d68a7c700c04dc976696304b4c35ddd4ea7c279ea5e9c708d0658f9f155
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135033560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2757454fe4728af602d6316e1c18f8aa768df9366e237e97e9b9dd7723642b5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:24:30 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.7.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:24:30 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:24:30 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:24:31 GMT
ARG MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:24:31 GMT
ENV MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:24:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:24:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:25:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:25:38 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:25:38 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:25:39 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:25:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:25:40 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:25:40 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774d390910b2611b5609d6a87b55ecf21e8d8a94b0ccaa198de96da94e7f2f8f`  
		Last Modified: Fri, 11 Nov 2022 03:34:04 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48eacdaba1f21fc6dae043bada0482a0d0860c329d4f121a85b0be95747661c4`  
		Last Modified: Fri, 11 Nov 2022 03:34:29 GMT  
		Size: 94.0 MB (93954670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a52d11b9a201386b94074fd83d6cc3d16258e57d91bcbc2ae19d06cb81d5f32`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8fb1b1cdec82551447442255718445788a5acf518dc3ee63cbfc297d357b444`  
		Last Modified: Fri, 11 Nov 2022 03:34:04 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; s390x

```console
$ docker pull mariadb@sha256:78e3904a5d1367d61d4543a6eaf9484abe9b780100df5e5a3293f390f1f89cd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.8 MB (123822669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad1d81a0d9d30f27590ca96f6d6476d904c9f7b1ffebbe651c8d82ebeae73f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:51:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:04:47 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:04:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:05:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:05:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:05:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:05:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.7.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:05:14 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:05:14 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:05:14 GMT
ARG MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:05:15 GMT
ENV MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:05:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:05:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:05:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:05:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:05:54 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:05:54 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:05:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:05:55 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:05:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c5044aaae9e9803c63085684d6340fffb48767ac91fa592d662702d71aff1`  
		Last Modified: Tue, 25 Oct 2022 08:57:06 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e797e665b3dcac7015b2708bfc1e2a7e59440583bb0dc4ce190816045b7dc697`  
		Last Modified: Fri, 11 Nov 2022 03:10:38 GMT  
		Size: 6.6 MB (6609162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172ce120405e0ffc7c9898c55d47e408d08615b0d187e3dafb6c6e38feba596`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c642d0428e3f0c4261602b56e0e3979b27a7fc40c24dcbd64f947edf8a216`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f36b814486ae0e4e5492681125942dc9466b99a56cdcf60f6c7a5d7eac1162f`  
		Last Modified: Fri, 11 Nov 2022 03:10:49 GMT  
		Size: 90.2 MB (90184817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25ebb7dc2fef882c5b560839a1af91bc96ced3ddc37276e68fb54d7249a46f9`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fc9db2b8419255f6395d11377327295b351e5417ee5e38d63889c3e9a82973`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7-focal`

```console
$ docker pull mariadb@sha256:237ebc09a1f3447ffccfcf2e0f638405ca5c31515d57d797dc4f01b6f2548c2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:cfb614d5a9c5befd2438d996fc50197ec6a8c3fd91a66f55e2baa79a477eb903
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125004791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41ed88878a8e3f0bf043eeb7480f859f83742b39c5929e53bda8dacaebce0bd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:52:47 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.7.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:52:47 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 01:52:47 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 01:52:47 GMT
ARG MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 01:52:47 GMT
ENV MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 01:52:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:52:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:53:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:54:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:54:00 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:54:00 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:54:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:54:00 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:54:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f3842c61594161a6ca84cb0f7b12e885dbb45c556ddf4cbf1ce79fc70e779c`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ef296df01678ff544a14617156e7e555e8bf30a3a40c906509012f1e99fb73`  
		Last Modified: Fri, 11 Nov 2022 01:59:21 GMT  
		Size: 89.4 MB (89355727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b81fc14995cdef8ab793a00b3219bd7c062a9ee8aa2192d7e1906402f4afca`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f85c6b03d8a9c90ab88f7f0b9c5826ae1e571047821250d7a13d8434250d38`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 7.0 KB (6953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:87a98538fd9b4cbbe6741e040e4fdad13c497012b35cc2012639955e25de1eb2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126160016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e91f3cd238ac241f4e4da3b1caf3e14ea8792c13440e97d7dc5cc9f976f1f5ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 02:04:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 26 Oct 2022 02:04:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Oct 2022 02:04:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Oct 2022 02:04:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Oct 2022 02:04:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:04:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 26 Oct 2022 02:04:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 26 Oct 2022 02:04:46 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 26 Oct 2022 02:04:46 GMT
ENV MARIADB_MAJOR=10.7
# Wed, 26 Oct 2022 02:04:46 GMT
ARG MARIADB_VERSION=1:10.7.6+maria~ubu2004
# Wed, 26 Oct 2022 02:04:46 GMT
ENV MARIADB_VERSION=1:10.7.6+maria~ubu2004
# Wed, 26 Oct 2022 02:04:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.6/repo/ubuntu/ focal main
# Wed, 26 Oct 2022 02:04:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.6/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 26 Oct 2022 02:05:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.6/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 26 Oct 2022 02:05:25 GMT
VOLUME [/var/lib/mysql]
# Wed, 26 Oct 2022 02:05:26 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 26 Oct 2022 02:05:26 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 26 Oct 2022 02:05:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 02:05:26 GMT
EXPOSE 3306
# Wed, 26 Oct 2022 02:05:26 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5059476c4efaaefd5639d62272cf873b43fc4dd354f29aa2d424f5672f98d7`  
		Last Modified: Wed, 26 Oct 2022 02:09:48 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b512e3647ec22a314bc3b404b44b891220289f7918fc3fb90dec28d934b622f7`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 5.5 MB (5474279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4034a198751d9b8465f987f8cd51acc3b45288510ea70f4f50588aca7ab03e`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 3.4 MB (3368397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a303c93f3f2afdbf7461aaa57d2e0376745b909ca61dc1ab04bed8a727844135`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a95ecb4d8b5c99728b7e239140c0c9127f6b8286e033494da3d7b938d10669`  
		Last Modified: Wed, 26 Oct 2022 02:09:46 GMT  
		Size: 2.2 MB (2186475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c381f22b0bfdceb13b81f9105a5b0965c5d34d0a2800bc7ae58461d1661aae`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e285a7096945cbc4dbb08b241e3e872668020d36c615adc856668a633722ffb`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d1d716822a5771930e74151a206729f0a0c4a01df00dd92c2ee3469f43f9f5`  
		Last Modified: Wed, 26 Oct 2022 02:09:54 GMT  
		Size: 87.9 MB (87919613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e9ea41ac711c364318e34a2f5d8ca8bea481e0ba0efd241c162a6260c0b6c0`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a3527aa4cc989f38e19d428becfb3ad46ab44e94e58598f3463af18fe21ec0`  
		Last Modified: Wed, 26 Oct 2022 02:09:43 GMT  
		Size: 7.0 KB (7048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a2f59d68a7c700c04dc976696304b4c35ddd4ea7c279ea5e9c708d0658f9f155
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135033560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2757454fe4728af602d6316e1c18f8aa768df9366e237e97e9b9dd7723642b5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:24:30 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.7.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:24:30 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:24:30 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:24:31 GMT
ARG MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:24:31 GMT
ENV MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:24:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:24:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:25:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:25:38 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:25:38 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:25:39 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:25:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:25:40 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:25:40 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774d390910b2611b5609d6a87b55ecf21e8d8a94b0ccaa198de96da94e7f2f8f`  
		Last Modified: Fri, 11 Nov 2022 03:34:04 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48eacdaba1f21fc6dae043bada0482a0d0860c329d4f121a85b0be95747661c4`  
		Last Modified: Fri, 11 Nov 2022 03:34:29 GMT  
		Size: 94.0 MB (93954670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a52d11b9a201386b94074fd83d6cc3d16258e57d91bcbc2ae19d06cb81d5f32`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8fb1b1cdec82551447442255718445788a5acf518dc3ee63cbfc297d357b444`  
		Last Modified: Fri, 11 Nov 2022 03:34:04 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:78e3904a5d1367d61d4543a6eaf9484abe9b780100df5e5a3293f390f1f89cd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.8 MB (123822669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad1d81a0d9d30f27590ca96f6d6476d904c9f7b1ffebbe651c8d82ebeae73f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:51:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:04:47 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:04:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:05:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:05:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:05:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:05:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.7.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:05:14 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:05:14 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:05:14 GMT
ARG MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:05:15 GMT
ENV MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:05:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:05:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:05:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:05:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:05:54 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:05:54 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:05:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:05:55 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:05:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c5044aaae9e9803c63085684d6340fffb48767ac91fa592d662702d71aff1`  
		Last Modified: Tue, 25 Oct 2022 08:57:06 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e797e665b3dcac7015b2708bfc1e2a7e59440583bb0dc4ce190816045b7dc697`  
		Last Modified: Fri, 11 Nov 2022 03:10:38 GMT  
		Size: 6.6 MB (6609162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172ce120405e0ffc7c9898c55d47e408d08615b0d187e3dafb6c6e38feba596`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c642d0428e3f0c4261602b56e0e3979b27a7fc40c24dcbd64f947edf8a216`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f36b814486ae0e4e5492681125942dc9466b99a56cdcf60f6c7a5d7eac1162f`  
		Last Modified: Fri, 11 Nov 2022 03:10:49 GMT  
		Size: 90.2 MB (90184817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25ebb7dc2fef882c5b560839a1af91bc96ced3ddc37276e68fb54d7249a46f9`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fc9db2b8419255f6395d11377327295b351e5417ee5e38d63889c3e9a82973`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.7`

```console
$ docker pull mariadb@sha256:b0ccd3ec2d98be87ac64a302b502316135d2592b3d67c9fd2ee0d314d436f6ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.7` - linux; amd64

```console
$ docker pull mariadb@sha256:cfb614d5a9c5befd2438d996fc50197ec6a8c3fd91a66f55e2baa79a477eb903
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125004791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41ed88878a8e3f0bf043eeb7480f859f83742b39c5929e53bda8dacaebce0bd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:52:47 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.7.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:52:47 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 01:52:47 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 01:52:47 GMT
ARG MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 01:52:47 GMT
ENV MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 01:52:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:52:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:53:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:54:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:54:00 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:54:00 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:54:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:54:00 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:54:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f3842c61594161a6ca84cb0f7b12e885dbb45c556ddf4cbf1ce79fc70e779c`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ef296df01678ff544a14617156e7e555e8bf30a3a40c906509012f1e99fb73`  
		Last Modified: Fri, 11 Nov 2022 01:59:21 GMT  
		Size: 89.4 MB (89355727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b81fc14995cdef8ab793a00b3219bd7c062a9ee8aa2192d7e1906402f4afca`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f85c6b03d8a9c90ab88f7f0b9c5826ae1e571047821250d7a13d8434250d38`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 7.0 KB (6953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.7` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a2f59d68a7c700c04dc976696304b4c35ddd4ea7c279ea5e9c708d0658f9f155
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135033560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2757454fe4728af602d6316e1c18f8aa768df9366e237e97e9b9dd7723642b5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:24:30 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.7.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:24:30 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:24:30 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:24:31 GMT
ARG MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:24:31 GMT
ENV MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:24:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:24:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:25:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:25:38 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:25:38 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:25:39 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:25:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:25:40 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:25:40 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774d390910b2611b5609d6a87b55ecf21e8d8a94b0ccaa198de96da94e7f2f8f`  
		Last Modified: Fri, 11 Nov 2022 03:34:04 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48eacdaba1f21fc6dae043bada0482a0d0860c329d4f121a85b0be95747661c4`  
		Last Modified: Fri, 11 Nov 2022 03:34:29 GMT  
		Size: 94.0 MB (93954670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a52d11b9a201386b94074fd83d6cc3d16258e57d91bcbc2ae19d06cb81d5f32`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8fb1b1cdec82551447442255718445788a5acf518dc3ee63cbfc297d357b444`  
		Last Modified: Fri, 11 Nov 2022 03:34:04 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.7` - linux; s390x

```console
$ docker pull mariadb@sha256:78e3904a5d1367d61d4543a6eaf9484abe9b780100df5e5a3293f390f1f89cd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.8 MB (123822669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad1d81a0d9d30f27590ca96f6d6476d904c9f7b1ffebbe651c8d82ebeae73f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:51:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:04:47 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:04:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:05:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:05:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:05:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:05:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.7.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:05:14 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:05:14 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:05:14 GMT
ARG MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:05:15 GMT
ENV MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:05:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:05:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:05:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:05:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:05:54 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:05:54 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:05:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:05:55 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:05:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c5044aaae9e9803c63085684d6340fffb48767ac91fa592d662702d71aff1`  
		Last Modified: Tue, 25 Oct 2022 08:57:06 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e797e665b3dcac7015b2708bfc1e2a7e59440583bb0dc4ce190816045b7dc697`  
		Last Modified: Fri, 11 Nov 2022 03:10:38 GMT  
		Size: 6.6 MB (6609162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172ce120405e0ffc7c9898c55d47e408d08615b0d187e3dafb6c6e38feba596`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c642d0428e3f0c4261602b56e0e3979b27a7fc40c24dcbd64f947edf8a216`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f36b814486ae0e4e5492681125942dc9466b99a56cdcf60f6c7a5d7eac1162f`  
		Last Modified: Fri, 11 Nov 2022 03:10:49 GMT  
		Size: 90.2 MB (90184817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25ebb7dc2fef882c5b560839a1af91bc96ced3ddc37276e68fb54d7249a46f9`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fc9db2b8419255f6395d11377327295b351e5417ee5e38d63889c3e9a82973`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.7-focal`

```console
$ docker pull mariadb@sha256:b0ccd3ec2d98be87ac64a302b502316135d2592b3d67c9fd2ee0d314d436f6ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:cfb614d5a9c5befd2438d996fc50197ec6a8c3fd91a66f55e2baa79a477eb903
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125004791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41ed88878a8e3f0bf043eeb7480f859f83742b39c5929e53bda8dacaebce0bd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:11:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:52:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:52:19 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:52:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:52:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:52:47 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:52:47 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.7.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:52:47 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 01:52:47 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 01:52:47 GMT
ARG MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 01:52:47 GMT
ENV MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 01:52:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 01:52:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:53:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:54:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:54:00 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:54:00 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:54:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:54:00 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:54:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6f4832182b9d366cc9cf48f4786dbc0b688c5f2d0a819d5ed74f31bef53555`  
		Last Modified: Wed, 26 Oct 2022 16:20:02 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed3156c4156966693d0f4fbacae9b7b499afd7c6c674e6667c0cb8fda31a80`  
		Last Modified: Fri, 11 Nov 2022 01:59:11 GMT  
		Size: 7.1 MB (7058561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1adc5c9f5ec1426f7463c719d7680ab9fc690d0f91c348854cb16d24b879082`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f3842c61594161a6ca84cb0f7b12e885dbb45c556ddf4cbf1ce79fc70e779c`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ef296df01678ff544a14617156e7e555e8bf30a3a40c906509012f1e99fb73`  
		Last Modified: Fri, 11 Nov 2022 01:59:21 GMT  
		Size: 89.4 MB (89355727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b81fc14995cdef8ab793a00b3219bd7c062a9ee8aa2192d7e1906402f4afca`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f85c6b03d8a9c90ab88f7f0b9c5826ae1e571047821250d7a13d8434250d38`  
		Last Modified: Fri, 11 Nov 2022 01:59:08 GMT  
		Size: 7.0 KB (6953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.7-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a2f59d68a7c700c04dc976696304b4c35ddd4ea7c279ea5e9c708d0658f9f155
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135033560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2757454fe4728af602d6316e1c18f8aa768df9366e237e97e9b9dd7723642b5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:45:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:23:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:23:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:24:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:24:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:24:29 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:24:30 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.7.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:24:30 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:24:30 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:24:31 GMT
ARG MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:24:31 GMT
ENV MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:24:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:24:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:25:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:25:38 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:25:38 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:25:39 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:25:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:25:40 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:25:40 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da4aca0ded73831bac1900cce993de71ec5e346c23dedb306464348a16f0ff`  
		Last Modified: Tue, 25 Oct 2022 14:55:10 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01505719c678238c4a7043c3ca47ba17ea82bf2e139272dfb64aac20a1b7a56a`  
		Last Modified: Fri, 11 Nov 2022 03:34:08 GMT  
		Size: 7.8 MB (7765682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4574c0141a5685b7976c5db4a739dd6dc2410b75d63975db4204211070eb1c`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774d390910b2611b5609d6a87b55ecf21e8d8a94b0ccaa198de96da94e7f2f8f`  
		Last Modified: Fri, 11 Nov 2022 03:34:04 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48eacdaba1f21fc6dae043bada0482a0d0860c329d4f121a85b0be95747661c4`  
		Last Modified: Fri, 11 Nov 2022 03:34:29 GMT  
		Size: 94.0 MB (93954670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a52d11b9a201386b94074fd83d6cc3d16258e57d91bcbc2ae19d06cb81d5f32`  
		Last Modified: Fri, 11 Nov 2022 03:34:03 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8fb1b1cdec82551447442255718445788a5acf518dc3ee63cbfc297d357b444`  
		Last Modified: Fri, 11 Nov 2022 03:34:04 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:78e3904a5d1367d61d4543a6eaf9484abe9b780100df5e5a3293f390f1f89cd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.8 MB (123822669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad1d81a0d9d30f27590ca96f6d6476d904c9f7b1ffebbe651c8d82ebeae73f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:51:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:04:47 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:04:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:05:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:05:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:05:14 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:05:14 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:focal org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.7.7 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:05:14 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:05:14 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 11 Nov 2022 03:05:14 GMT
ARG MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:05:15 GMT
ENV MARIADB_VERSION=1:10.7.7+maria~ubu2004
# Fri, 11 Nov 2022 03:05:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
# Fri, 11 Nov 2022 03:05:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:05:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:05:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:05:54 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:05:54 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:05:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:05:55 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:05:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5c5044aaae9e9803c63085684d6340fffb48767ac91fa592d662702d71aff1`  
		Last Modified: Tue, 25 Oct 2022 08:57:06 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e797e665b3dcac7015b2708bfc1e2a7e59440583bb0dc4ce190816045b7dc697`  
		Last Modified: Fri, 11 Nov 2022 03:10:38 GMT  
		Size: 6.6 MB (6609162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172ce120405e0ffc7c9898c55d47e408d08615b0d187e3dafb6c6e38feba596`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c642d0428e3f0c4261602b56e0e3979b27a7fc40c24dcbd64f947edf8a216`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f36b814486ae0e4e5492681125942dc9466b99a56cdcf60f6c7a5d7eac1162f`  
		Last Modified: Fri, 11 Nov 2022 03:10:49 GMT  
		Size: 90.2 MB (90184817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25ebb7dc2fef882c5b560839a1af91bc96ced3ddc37276e68fb54d7249a46f9`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fc9db2b8419255f6395d11377327295b351e5417ee5e38d63889c3e9a82973`  
		Last Modified: Fri, 11 Nov 2022 03:10:36 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8`

```console
$ docker pull mariadb@sha256:9732f73e62e32c92513908990f09a55005d4762923be417d3fffbcb148033242
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8` - linux; amd64

```console
$ docker pull mariadb@sha256:d47a903023cae4ebab6c95a599f782d0e8c8dafdf9ad0c2717e4807f7b87dacf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121737861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c58efcb2d614137096fbd3417547e8132238b68e87b66fa6e65716ffa3abc88a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:51:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:51:39 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 01:51:39 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 01:51:39 GMT
ARG MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 01:51:39 GMT
ENV MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 01:51:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:51:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:52:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:52:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:52:11 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:52:11 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:52:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:52:12 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:52:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877c2d880362f31777c760a2d1948796a53c2635e67b5bf0fd6f79b53f322af3`  
		Last Modified: Fri, 11 Nov 2022 01:58:40 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5ba98b683265be4819670212b19e17535e23905e66e489112b6835a75bbe3`  
		Last Modified: Fri, 11 Nov 2022 01:58:52 GMT  
		Size: 85.8 MB (85770866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd72dca1315bd7f57b5a126213a37a0c7245319d62150d17e5e67128fba934d`  
		Last Modified: Fri, 11 Nov 2022 01:58:40 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1e28fc0e59ab6f523fa3d60e503a7ec2db653a80c76a93a37901dfae776336`  
		Last Modified: Fri, 11 Nov 2022 01:58:40 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0fb2878bc86064e2f6e3a23fb7c6b4000369966a515b60c171f411beabfc6bca
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118516515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80346687bfec3eaa67e3f424e9728c48f36592572dab6769e4232c408b5b632d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:07:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 20:07:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:35 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 20:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 20:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 20:07:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 20:08:59 GMT
ARG MARIADB_MAJOR=10.8
# Wed, 02 Nov 2022 20:08:59 GMT
ENV MARIADB_MAJOR=10.8
# Wed, 02 Nov 2022 20:08:59 GMT
ARG MARIADB_VERSION=1:10.8.5+maria~ubu2204
# Wed, 02 Nov 2022 20:08:59 GMT
ENV MARIADB_VERSION=1:10.8.5+maria~ubu2204
# Wed, 02 Nov 2022 20:08:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.5/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 20:09:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 20:09:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 20:09:19 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 20:09:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 20:09:19 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 20:09:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:09:20 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 20:09:20 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf568f815bdc2b755b642d6cad079d9e2e71dd364d2806bf4a9a3cb0fe3d18b7`  
		Last Modified: Wed, 02 Nov 2022 20:10:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a27635d8616b3a361adc11c7e5712c05d3edef95c0573370b2c92058ed582`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 3.7 MB (3737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce0b0cfd1e867e47d514f1de07a5da365d36bfb15513e7cf310802577ab13c`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 1.9 MB (1898793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd291b4a9d31c95c30d2580b470dd4ecbe4d2d10c11e47967a037f8b939146e`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505d811110d4c6311181f11307bd36ac49e38d1ab561c611e562b293b90a9ef`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 2.2 MB (2191982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf7ac4a18820861abff79a668773c9f881f45b6f47d10f21df0661e7190013b`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7f6dfb067d988f79d0ab038a1eca9d6a03131a6ca4eea8bf9ccd36e165b70`  
		Last Modified: Wed, 02 Nov 2022 20:11:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c14a98a30f182adcc4fdf5d93432421c616ee1cae7c56208e20ccecab70c19a`  
		Last Modified: Wed, 02 Nov 2022 20:11:24 GMT  
		Size: 82.3 MB (82290513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3489f5524a391d9156536b82a6f3cf4ff2e2c5d924cafedcdc1d28bda8e6d0e3`  
		Last Modified: Wed, 02 Nov 2022 20:11:13 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e52a7f78fc68eb4a754c260178976cc5046720f644b07bec438292e3b8b14ed`  
		Last Modified: Wed, 02 Nov 2022 20:11:13 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5cd96f86af7620fbf363de11524a936444d7d66381cb20eb6d113a6ec9bc8f99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130545980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01e1ecdf0fab536cbdbc11eca47b0476f1ad570ecfa41ce99a6febf640c99def`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:22:44 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:22:44 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:22:44 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:22:45 GMT
ARG MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:22:45 GMT
ENV MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:22:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:22:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:23:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:23:35 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:23:35 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:23:35 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:23:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:23:36 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:23:36 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5372729dbe2de8a9512ec5431764c111bc36656036324ce8708c6c7cc5d042`  
		Last Modified: Fri, 11 Nov 2022 03:33:17 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307917113c1a0257ca2e983d8e5b8796c9f1fdde1dd21350e039e4a43e0053ec`  
		Last Modified: Fri, 11 Nov 2022 03:33:40 GMT  
		Size: 88.9 MB (88870668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1b89a94a62aed757135ef1c331e73d77b5a686c5fb3bc0a39f792aae3eb97b`  
		Last Modified: Fri, 11 Nov 2022 03:33:17 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398d21e5947c286dafdb29c285eddf8da6da76b411286e39a06128731b3cf34`  
		Last Modified: Fri, 11 Nov 2022 03:33:17 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; s390x

```console
$ docker pull mariadb@sha256:7a78702f7ea9aab15e869d92e4ef620a369ca38655d70b6ca4ea8abc3617dc8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119432039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a588e02d6043614f8103299e736c7ca76d54233e6e514bfd6c0f95477df00cc6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:03:56 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:03:56 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:03:57 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:03:57 GMT
ARG MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:03:57 GMT
ENV MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:03:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:03:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:04:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:04:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:04:33 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:04:33 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:04:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:04:33 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:04:34 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266e3ddd08497ea645ba60d8bece75a38718dff1b57893f903dd1d56442c226`  
		Last Modified: Fri, 11 Nov 2022 03:10:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b1bcf43521eaae97e398c5411d3ba3ed2afd6c7714001e5225a4ecec20f413`  
		Last Modified: Fri, 11 Nov 2022 03:10:25 GMT  
		Size: 85.4 MB (85367954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449fbfc055402ec0fc39679b8314a0d144fe7667b6a97901ccfab32ea6fa7e3c`  
		Last Modified: Fri, 11 Nov 2022 03:10:14 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b3deb07ad0cf2c7cb8dc2c4a6f5766a8f9dd5f98adb2b2fc6caaf6f251a7a1`  
		Last Modified: Fri, 11 Nov 2022 03:10:14 GMT  
		Size: 7.0 KB (6952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8-jammy`

```console
$ docker pull mariadb@sha256:9732f73e62e32c92513908990f09a55005d4762923be417d3fffbcb148033242
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:d47a903023cae4ebab6c95a599f782d0e8c8dafdf9ad0c2717e4807f7b87dacf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121737861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c58efcb2d614137096fbd3417547e8132238b68e87b66fa6e65716ffa3abc88a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:51:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:51:39 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 01:51:39 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 01:51:39 GMT
ARG MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 01:51:39 GMT
ENV MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 01:51:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:51:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:52:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:52:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:52:11 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:52:11 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:52:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:52:12 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:52:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877c2d880362f31777c760a2d1948796a53c2635e67b5bf0fd6f79b53f322af3`  
		Last Modified: Fri, 11 Nov 2022 01:58:40 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5ba98b683265be4819670212b19e17535e23905e66e489112b6835a75bbe3`  
		Last Modified: Fri, 11 Nov 2022 01:58:52 GMT  
		Size: 85.8 MB (85770866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd72dca1315bd7f57b5a126213a37a0c7245319d62150d17e5e67128fba934d`  
		Last Modified: Fri, 11 Nov 2022 01:58:40 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1e28fc0e59ab6f523fa3d60e503a7ec2db653a80c76a93a37901dfae776336`  
		Last Modified: Fri, 11 Nov 2022 01:58:40 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0fb2878bc86064e2f6e3a23fb7c6b4000369966a515b60c171f411beabfc6bca
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118516515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80346687bfec3eaa67e3f424e9728c48f36592572dab6769e4232c408b5b632d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:07:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 20:07:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:35 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 20:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 20:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 20:07:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 20:08:59 GMT
ARG MARIADB_MAJOR=10.8
# Wed, 02 Nov 2022 20:08:59 GMT
ENV MARIADB_MAJOR=10.8
# Wed, 02 Nov 2022 20:08:59 GMT
ARG MARIADB_VERSION=1:10.8.5+maria~ubu2204
# Wed, 02 Nov 2022 20:08:59 GMT
ENV MARIADB_VERSION=1:10.8.5+maria~ubu2204
# Wed, 02 Nov 2022 20:08:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.5/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 20:09:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.5/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 20:09:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.5/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 20:09:19 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 20:09:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 20:09:19 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 20:09:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:09:20 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 20:09:20 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf568f815bdc2b755b642d6cad079d9e2e71dd364d2806bf4a9a3cb0fe3d18b7`  
		Last Modified: Wed, 02 Nov 2022 20:10:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a27635d8616b3a361adc11c7e5712c05d3edef95c0573370b2c92058ed582`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 3.7 MB (3737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce0b0cfd1e867e47d514f1de07a5da365d36bfb15513e7cf310802577ab13c`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 1.9 MB (1898793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd291b4a9d31c95c30d2580b470dd4ecbe4d2d10c11e47967a037f8b939146e`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505d811110d4c6311181f11307bd36ac49e38d1ab561c611e562b293b90a9ef`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 2.2 MB (2191982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf7ac4a18820861abff79a668773c9f881f45b6f47d10f21df0661e7190013b`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7f6dfb067d988f79d0ab038a1eca9d6a03131a6ca4eea8bf9ccd36e165b70`  
		Last Modified: Wed, 02 Nov 2022 20:11:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c14a98a30f182adcc4fdf5d93432421c616ee1cae7c56208e20ccecab70c19a`  
		Last Modified: Wed, 02 Nov 2022 20:11:24 GMT  
		Size: 82.3 MB (82290513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3489f5524a391d9156536b82a6f3cf4ff2e2c5d924cafedcdc1d28bda8e6d0e3`  
		Last Modified: Wed, 02 Nov 2022 20:11:13 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e52a7f78fc68eb4a754c260178976cc5046720f644b07bec438292e3b8b14ed`  
		Last Modified: Wed, 02 Nov 2022 20:11:13 GMT  
		Size: 7.0 KB (7047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5cd96f86af7620fbf363de11524a936444d7d66381cb20eb6d113a6ec9bc8f99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130545980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01e1ecdf0fab536cbdbc11eca47b0476f1ad570ecfa41ce99a6febf640c99def`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:22:44 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:22:44 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:22:44 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:22:45 GMT
ARG MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:22:45 GMT
ENV MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:22:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:22:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:23:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:23:35 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:23:35 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:23:35 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:23:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:23:36 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:23:36 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5372729dbe2de8a9512ec5431764c111bc36656036324ce8708c6c7cc5d042`  
		Last Modified: Fri, 11 Nov 2022 03:33:17 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307917113c1a0257ca2e983d8e5b8796c9f1fdde1dd21350e039e4a43e0053ec`  
		Last Modified: Fri, 11 Nov 2022 03:33:40 GMT  
		Size: 88.9 MB (88870668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1b89a94a62aed757135ef1c331e73d77b5a686c5fb3bc0a39f792aae3eb97b`  
		Last Modified: Fri, 11 Nov 2022 03:33:17 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398d21e5947c286dafdb29c285eddf8da6da76b411286e39a06128731b3cf34`  
		Last Modified: Fri, 11 Nov 2022 03:33:17 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:7a78702f7ea9aab15e869d92e4ef620a369ca38655d70b6ca4ea8abc3617dc8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119432039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a588e02d6043614f8103299e736c7ca76d54233e6e514bfd6c0f95477df00cc6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:03:56 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:03:56 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:03:57 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:03:57 GMT
ARG MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:03:57 GMT
ENV MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:03:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:03:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:04:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:04:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:04:33 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:04:33 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:04:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:04:33 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:04:34 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266e3ddd08497ea645ba60d8bece75a38718dff1b57893f903dd1d56442c226`  
		Last Modified: Fri, 11 Nov 2022 03:10:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b1bcf43521eaae97e398c5411d3ba3ed2afd6c7714001e5225a4ecec20f413`  
		Last Modified: Fri, 11 Nov 2022 03:10:25 GMT  
		Size: 85.4 MB (85367954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449fbfc055402ec0fc39679b8314a0d144fe7667b6a97901ccfab32ea6fa7e3c`  
		Last Modified: Fri, 11 Nov 2022 03:10:14 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b3deb07ad0cf2c7cb8dc2c4a6f5766a8f9dd5f98adb2b2fc6caaf6f251a7a1`  
		Last Modified: Fri, 11 Nov 2022 03:10:14 GMT  
		Size: 7.0 KB (6952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.6`

```console
$ docker pull mariadb@sha256:b4a1e9b1f43973648458e5f59177ceb75dbf1cfbb4a7bb4beec0d11d73803be1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8.6` - linux; amd64

```console
$ docker pull mariadb@sha256:d47a903023cae4ebab6c95a599f782d0e8c8dafdf9ad0c2717e4807f7b87dacf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121737861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c58efcb2d614137096fbd3417547e8132238b68e87b66fa6e65716ffa3abc88a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:51:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:51:39 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 01:51:39 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 01:51:39 GMT
ARG MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 01:51:39 GMT
ENV MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 01:51:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:51:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:52:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:52:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:52:11 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:52:11 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:52:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:52:12 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:52:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877c2d880362f31777c760a2d1948796a53c2635e67b5bf0fd6f79b53f322af3`  
		Last Modified: Fri, 11 Nov 2022 01:58:40 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5ba98b683265be4819670212b19e17535e23905e66e489112b6835a75bbe3`  
		Last Modified: Fri, 11 Nov 2022 01:58:52 GMT  
		Size: 85.8 MB (85770866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd72dca1315bd7f57b5a126213a37a0c7245319d62150d17e5e67128fba934d`  
		Last Modified: Fri, 11 Nov 2022 01:58:40 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1e28fc0e59ab6f523fa3d60e503a7ec2db653a80c76a93a37901dfae776336`  
		Last Modified: Fri, 11 Nov 2022 01:58:40 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5cd96f86af7620fbf363de11524a936444d7d66381cb20eb6d113a6ec9bc8f99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130545980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01e1ecdf0fab536cbdbc11eca47b0476f1ad570ecfa41ce99a6febf640c99def`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:22:44 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:22:44 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:22:44 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:22:45 GMT
ARG MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:22:45 GMT
ENV MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:22:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:22:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:23:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:23:35 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:23:35 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:23:35 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:23:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:23:36 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:23:36 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5372729dbe2de8a9512ec5431764c111bc36656036324ce8708c6c7cc5d042`  
		Last Modified: Fri, 11 Nov 2022 03:33:17 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307917113c1a0257ca2e983d8e5b8796c9f1fdde1dd21350e039e4a43e0053ec`  
		Last Modified: Fri, 11 Nov 2022 03:33:40 GMT  
		Size: 88.9 MB (88870668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1b89a94a62aed757135ef1c331e73d77b5a686c5fb3bc0a39f792aae3eb97b`  
		Last Modified: Fri, 11 Nov 2022 03:33:17 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398d21e5947c286dafdb29c285eddf8da6da76b411286e39a06128731b3cf34`  
		Last Modified: Fri, 11 Nov 2022 03:33:17 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.6` - linux; s390x

```console
$ docker pull mariadb@sha256:7a78702f7ea9aab15e869d92e4ef620a369ca38655d70b6ca4ea8abc3617dc8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119432039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a588e02d6043614f8103299e736c7ca76d54233e6e514bfd6c0f95477df00cc6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:03:56 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:03:56 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:03:57 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:03:57 GMT
ARG MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:03:57 GMT
ENV MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:03:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:03:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:04:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:04:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:04:33 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:04:33 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:04:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:04:33 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:04:34 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266e3ddd08497ea645ba60d8bece75a38718dff1b57893f903dd1d56442c226`  
		Last Modified: Fri, 11 Nov 2022 03:10:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b1bcf43521eaae97e398c5411d3ba3ed2afd6c7714001e5225a4ecec20f413`  
		Last Modified: Fri, 11 Nov 2022 03:10:25 GMT  
		Size: 85.4 MB (85367954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449fbfc055402ec0fc39679b8314a0d144fe7667b6a97901ccfab32ea6fa7e3c`  
		Last Modified: Fri, 11 Nov 2022 03:10:14 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b3deb07ad0cf2c7cb8dc2c4a6f5766a8f9dd5f98adb2b2fc6caaf6f251a7a1`  
		Last Modified: Fri, 11 Nov 2022 03:10:14 GMT  
		Size: 7.0 KB (6952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.6-jammy`

```console
$ docker pull mariadb@sha256:b4a1e9b1f43973648458e5f59177ceb75dbf1cfbb4a7bb4beec0d11d73803be1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8.6-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:d47a903023cae4ebab6c95a599f782d0e8c8dafdf9ad0c2717e4807f7b87dacf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121737861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c58efcb2d614137096fbd3417547e8132238b68e87b66fa6e65716ffa3abc88a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:51:39 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:51:39 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 01:51:39 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 01:51:39 GMT
ARG MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 01:51:39 GMT
ENV MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 01:51:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:51:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:52:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:52:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:52:11 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:52:11 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:52:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:52:12 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:52:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877c2d880362f31777c760a2d1948796a53c2635e67b5bf0fd6f79b53f322af3`  
		Last Modified: Fri, 11 Nov 2022 01:58:40 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d5ba98b683265be4819670212b19e17535e23905e66e489112b6835a75bbe3`  
		Last Modified: Fri, 11 Nov 2022 01:58:52 GMT  
		Size: 85.8 MB (85770866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd72dca1315bd7f57b5a126213a37a0c7245319d62150d17e5e67128fba934d`  
		Last Modified: Fri, 11 Nov 2022 01:58:40 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1e28fc0e59ab6f523fa3d60e503a7ec2db653a80c76a93a37901dfae776336`  
		Last Modified: Fri, 11 Nov 2022 01:58:40 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.6-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5cd96f86af7620fbf363de11524a936444d7d66381cb20eb6d113a6ec9bc8f99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130545980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01e1ecdf0fab536cbdbc11eca47b0476f1ad570ecfa41ce99a6febf640c99def`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:22:44 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:22:44 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:22:44 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:22:45 GMT
ARG MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:22:45 GMT
ENV MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:22:45 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:22:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:23:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:23:35 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:23:35 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:23:35 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:23:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:23:36 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:23:36 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5372729dbe2de8a9512ec5431764c111bc36656036324ce8708c6c7cc5d042`  
		Last Modified: Fri, 11 Nov 2022 03:33:17 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307917113c1a0257ca2e983d8e5b8796c9f1fdde1dd21350e039e4a43e0053ec`  
		Last Modified: Fri, 11 Nov 2022 03:33:40 GMT  
		Size: 88.9 MB (88870668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1b89a94a62aed757135ef1c331e73d77b5a686c5fb3bc0a39f792aae3eb97b`  
		Last Modified: Fri, 11 Nov 2022 03:33:17 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398d21e5947c286dafdb29c285eddf8da6da76b411286e39a06128731b3cf34`  
		Last Modified: Fri, 11 Nov 2022 03:33:17 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.6-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:7a78702f7ea9aab15e869d92e4ef620a369ca38655d70b6ca4ea8abc3617dc8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119432039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a588e02d6043614f8103299e736c7ca76d54233e6e514bfd6c0f95477df00cc6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:03:56 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.8.6 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:03:56 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:03:57 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 11 Nov 2022 03:03:57 GMT
ARG MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:03:57 GMT
ENV MARIADB_VERSION=1:10.8.6+maria~ubu2204
# Fri, 11 Nov 2022 03:03:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:03:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:04:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.6/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:04:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:04:33 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:04:33 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:04:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:04:33 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:04:34 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0266e3ddd08497ea645ba60d8bece75a38718dff1b57893f903dd1d56442c226`  
		Last Modified: Fri, 11 Nov 2022 03:10:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b1bcf43521eaae97e398c5411d3ba3ed2afd6c7714001e5225a4ecec20f413`  
		Last Modified: Fri, 11 Nov 2022 03:10:25 GMT  
		Size: 85.4 MB (85367954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449fbfc055402ec0fc39679b8314a0d144fe7667b6a97901ccfab32ea6fa7e3c`  
		Last Modified: Fri, 11 Nov 2022 03:10:14 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b3deb07ad0cf2c7cb8dc2c4a6f5766a8f9dd5f98adb2b2fc6caaf6f251a7a1`  
		Last Modified: Fri, 11 Nov 2022 03:10:14 GMT  
		Size: 7.0 KB (6952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9`

```console
$ docker pull mariadb@sha256:4d0d7e05cac3f285cb7b38226e8f61f406c6ea2527c317ec2b31a5f5270d7fb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.9` - linux; amd64

```console
$ docker pull mariadb@sha256:91323beb7c5c2fb134d13874504aea4e4608304370423019f277b1f70882f9ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121852276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825ad7e31db8cfc5ffa434e1171060e9f60db49279dd675fc562466da3bc0ea0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:50:58 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:50:59 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:50:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:51:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:51:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:51:33 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:51:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ea015f843833e7db49738387776c15cc20eafdf70ef5045dff63f0737b4f2`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c861410f2b3e963a06afa4ca24fda97e00c496b9dc2a3ced1f8affa8f94293f`  
		Last Modified: Fri, 11 Nov 2022 01:58:12 GMT  
		Size: 85.9 MB (85885285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46193445bc4f96aba11e38a4481b43380bee2c095422d3df722641dcad6bc477`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262eb9124c0aca8d6780dfa07f0a43ff16308aa84d6f2c84e5566a0d975bd9dd`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:31f677ba9b50beef8d48a3bbcab29485f5aa3a90677d1ebc44039bbc9bc8bde4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118604917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe889c390f208ce09bf8bfa7869b7d342d999c4279a8809e3a2d2a14332cf10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:07:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 20:07:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:35 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 20:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 20:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 20:07:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 20:08:36 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 20:08:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 20:08:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 20:08:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 20:08:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:08:55 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 20:08:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf568f815bdc2b755b642d6cad079d9e2e71dd364d2806bf4a9a3cb0fe3d18b7`  
		Last Modified: Wed, 02 Nov 2022 20:10:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a27635d8616b3a361adc11c7e5712c05d3edef95c0573370b2c92058ed582`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 3.7 MB (3737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce0b0cfd1e867e47d514f1de07a5da365d36bfb15513e7cf310802577ab13c`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 1.9 MB (1898793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd291b4a9d31c95c30d2580b470dd4ecbe4d2d10c11e47967a037f8b939146e`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505d811110d4c6311181f11307bd36ac49e38d1ab561c611e562b293b90a9ef`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 2.2 MB (2191982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf7ac4a18820861abff79a668773c9f881f45b6f47d10f21df0661e7190013b`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5452b6a0ce3706d857279cfa1cdaef7c8b6bc76d8d6a4b1c43367203b766cd2f`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2628f7ef3cedd084f9a47495aa153853592da56561a6e3231a78435d95ff9949`  
		Last Modified: Wed, 02 Nov 2022 20:10:44 GMT  
		Size: 82.4 MB (82378919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e903661ffaca59211d235a8061c23cc51afe2459c91999d6e191b263897d86d0`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ecec752f0246a09512597065787135cfb39650e56b627521d6b7a25b44bec`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0b3197dcaae25333f0f203038060ecdea256e57a3dbddac50f28647989b2710d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130653312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837797e389ef277d85639136b3254240872973d0626320986cfffbfb6a87f0b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:21:41 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:21:42 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:21:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:22:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:22:34 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:22:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:22:35 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:22:35 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74756e55e3348ae0fd95c532056ccfd545a53ef391306dc1e40c944f767b424`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87682e9f6b59527390239170077fb830688d0d3ecb3a00ec019774d672fb7c9a`  
		Last Modified: Fri, 11 Nov 2022 03:32:44 GMT  
		Size: 89.0 MB (88977999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e944b0bd7dc5e8a3abc0784d0bbca0b06bf94e01f94133c299086f0ab5db977b`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50240058fe79dd7c3e564cbe912654ac3d47ff0b4ec8cf8843727f57594b73bc`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9` - linux; s390x

```console
$ docker pull mariadb@sha256:79b920fffb62ce6a5a5d43710462a5ee875839d137278cd648e98e4888851a0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119532750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c1a22b2569dd6f45c61a2a09a52ee5ac7577df02b9e510c73e4ef5e0798155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:03:13 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:03:13 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:03:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:03:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:03:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:03:44 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:03:45 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:03:45 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:03:45 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272871ff5a39e7f724ba60200020bda369282194ceb0a7fbacace8a0c1a6bd3`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a8ba951405415f1411b29b725fc469af2374cb7c4f24018f4f0ff7802d236d`  
		Last Modified: Fri, 11 Nov 2022 03:09:54 GMT  
		Size: 85.5 MB (85468667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89a1761c7bc6b466cd2efb4d28b9a0fc4fb55be84ded124f3922236ecf7c3af`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4932db4ceb6992a81f9ab516f105280d520e93584dc1b3302f0fa0d9feb96e57`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 7.0 KB (6952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9-jammy`

```console
$ docker pull mariadb@sha256:4d0d7e05cac3f285cb7b38226e8f61f406c6ea2527c317ec2b31a5f5270d7fb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.9-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:91323beb7c5c2fb134d13874504aea4e4608304370423019f277b1f70882f9ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121852276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825ad7e31db8cfc5ffa434e1171060e9f60db49279dd675fc562466da3bc0ea0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:50:58 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:50:59 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:50:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:51:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:51:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:51:33 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:51:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ea015f843833e7db49738387776c15cc20eafdf70ef5045dff63f0737b4f2`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c861410f2b3e963a06afa4ca24fda97e00c496b9dc2a3ced1f8affa8f94293f`  
		Last Modified: Fri, 11 Nov 2022 01:58:12 GMT  
		Size: 85.9 MB (85885285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46193445bc4f96aba11e38a4481b43380bee2c095422d3df722641dcad6bc477`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262eb9124c0aca8d6780dfa07f0a43ff16308aa84d6f2c84e5566a0d975bd9dd`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:31f677ba9b50beef8d48a3bbcab29485f5aa3a90677d1ebc44039bbc9bc8bde4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118604917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe889c390f208ce09bf8bfa7869b7d342d999c4279a8809e3a2d2a14332cf10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:07:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 20:07:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:35 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 20:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 20:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 20:07:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 20:08:36 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 20:08:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 20:08:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 20:08:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 20:08:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:08:55 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 20:08:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf568f815bdc2b755b642d6cad079d9e2e71dd364d2806bf4a9a3cb0fe3d18b7`  
		Last Modified: Wed, 02 Nov 2022 20:10:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a27635d8616b3a361adc11c7e5712c05d3edef95c0573370b2c92058ed582`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 3.7 MB (3737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce0b0cfd1e867e47d514f1de07a5da365d36bfb15513e7cf310802577ab13c`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 1.9 MB (1898793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd291b4a9d31c95c30d2580b470dd4ecbe4d2d10c11e47967a037f8b939146e`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505d811110d4c6311181f11307bd36ac49e38d1ab561c611e562b293b90a9ef`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 2.2 MB (2191982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf7ac4a18820861abff79a668773c9f881f45b6f47d10f21df0661e7190013b`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5452b6a0ce3706d857279cfa1cdaef7c8b6bc76d8d6a4b1c43367203b766cd2f`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2628f7ef3cedd084f9a47495aa153853592da56561a6e3231a78435d95ff9949`  
		Last Modified: Wed, 02 Nov 2022 20:10:44 GMT  
		Size: 82.4 MB (82378919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e903661ffaca59211d235a8061c23cc51afe2459c91999d6e191b263897d86d0`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ecec752f0246a09512597065787135cfb39650e56b627521d6b7a25b44bec`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0b3197dcaae25333f0f203038060ecdea256e57a3dbddac50f28647989b2710d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130653312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837797e389ef277d85639136b3254240872973d0626320986cfffbfb6a87f0b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:21:41 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:21:42 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:21:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:22:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:22:34 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:22:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:22:35 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:22:35 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74756e55e3348ae0fd95c532056ccfd545a53ef391306dc1e40c944f767b424`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87682e9f6b59527390239170077fb830688d0d3ecb3a00ec019774d672fb7c9a`  
		Last Modified: Fri, 11 Nov 2022 03:32:44 GMT  
		Size: 89.0 MB (88977999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e944b0bd7dc5e8a3abc0784d0bbca0b06bf94e01f94133c299086f0ab5db977b`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50240058fe79dd7c3e564cbe912654ac3d47ff0b4ec8cf8843727f57594b73bc`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:79b920fffb62ce6a5a5d43710462a5ee875839d137278cd648e98e4888851a0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119532750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c1a22b2569dd6f45c61a2a09a52ee5ac7577df02b9e510c73e4ef5e0798155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:03:13 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:03:13 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:03:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:03:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:03:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:03:44 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:03:45 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:03:45 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:03:45 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272871ff5a39e7f724ba60200020bda369282194ceb0a7fbacace8a0c1a6bd3`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a8ba951405415f1411b29b725fc469af2374cb7c4f24018f4f0ff7802d236d`  
		Last Modified: Fri, 11 Nov 2022 03:09:54 GMT  
		Size: 85.5 MB (85468667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89a1761c7bc6b466cd2efb4d28b9a0fc4fb55be84ded124f3922236ecf7c3af`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4932db4ceb6992a81f9ab516f105280d520e93584dc1b3302f0fa0d9feb96e57`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 7.0 KB (6952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9.4`

```console
$ docker pull mariadb@sha256:49b6fc6b7aaa542d543fb731c411cbe5a58e5c2b9ecafdd3bc3699361f8d111e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.9.4` - linux; amd64

```console
$ docker pull mariadb@sha256:91323beb7c5c2fb134d13874504aea4e4608304370423019f277b1f70882f9ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121852276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825ad7e31db8cfc5ffa434e1171060e9f60db49279dd675fc562466da3bc0ea0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:50:58 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:50:59 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:50:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:51:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:51:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:51:33 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:51:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ea015f843833e7db49738387776c15cc20eafdf70ef5045dff63f0737b4f2`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c861410f2b3e963a06afa4ca24fda97e00c496b9dc2a3ced1f8affa8f94293f`  
		Last Modified: Fri, 11 Nov 2022 01:58:12 GMT  
		Size: 85.9 MB (85885285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46193445bc4f96aba11e38a4481b43380bee2c095422d3df722641dcad6bc477`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262eb9124c0aca8d6780dfa07f0a43ff16308aa84d6f2c84e5566a0d975bd9dd`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0b3197dcaae25333f0f203038060ecdea256e57a3dbddac50f28647989b2710d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130653312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837797e389ef277d85639136b3254240872973d0626320986cfffbfb6a87f0b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:21:41 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:21:42 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:21:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:22:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:22:34 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:22:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:22:35 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:22:35 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74756e55e3348ae0fd95c532056ccfd545a53ef391306dc1e40c944f767b424`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87682e9f6b59527390239170077fb830688d0d3ecb3a00ec019774d672fb7c9a`  
		Last Modified: Fri, 11 Nov 2022 03:32:44 GMT  
		Size: 89.0 MB (88977999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e944b0bd7dc5e8a3abc0784d0bbca0b06bf94e01f94133c299086f0ab5db977b`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50240058fe79dd7c3e564cbe912654ac3d47ff0b4ec8cf8843727f57594b73bc`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9.4` - linux; s390x

```console
$ docker pull mariadb@sha256:79b920fffb62ce6a5a5d43710462a5ee875839d137278cd648e98e4888851a0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119532750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c1a22b2569dd6f45c61a2a09a52ee5ac7577df02b9e510c73e4ef5e0798155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:03:13 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:03:13 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:03:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:03:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:03:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:03:44 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:03:45 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:03:45 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:03:45 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272871ff5a39e7f724ba60200020bda369282194ceb0a7fbacace8a0c1a6bd3`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a8ba951405415f1411b29b725fc469af2374cb7c4f24018f4f0ff7802d236d`  
		Last Modified: Fri, 11 Nov 2022 03:09:54 GMT  
		Size: 85.5 MB (85468667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89a1761c7bc6b466cd2efb4d28b9a0fc4fb55be84ded124f3922236ecf7c3af`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4932db4ceb6992a81f9ab516f105280d520e93584dc1b3302f0fa0d9feb96e57`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 7.0 KB (6952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9.4-jammy`

```console
$ docker pull mariadb@sha256:49b6fc6b7aaa542d543fb731c411cbe5a58e5c2b9ecafdd3bc3699361f8d111e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.9.4-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:91323beb7c5c2fb134d13874504aea4e4608304370423019f277b1f70882f9ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121852276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825ad7e31db8cfc5ffa434e1171060e9f60db49279dd675fc562466da3bc0ea0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:50:58 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:50:59 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:50:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:51:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:51:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:51:33 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:51:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ea015f843833e7db49738387776c15cc20eafdf70ef5045dff63f0737b4f2`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c861410f2b3e963a06afa4ca24fda97e00c496b9dc2a3ced1f8affa8f94293f`  
		Last Modified: Fri, 11 Nov 2022 01:58:12 GMT  
		Size: 85.9 MB (85885285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46193445bc4f96aba11e38a4481b43380bee2c095422d3df722641dcad6bc477`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262eb9124c0aca8d6780dfa07f0a43ff16308aa84d6f2c84e5566a0d975bd9dd`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9.4-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0b3197dcaae25333f0f203038060ecdea256e57a3dbddac50f28647989b2710d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130653312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837797e389ef277d85639136b3254240872973d0626320986cfffbfb6a87f0b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:21:41 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:21:42 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:21:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:22:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:22:34 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:22:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:22:35 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:22:35 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74756e55e3348ae0fd95c532056ccfd545a53ef391306dc1e40c944f767b424`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87682e9f6b59527390239170077fb830688d0d3ecb3a00ec019774d672fb7c9a`  
		Last Modified: Fri, 11 Nov 2022 03:32:44 GMT  
		Size: 89.0 MB (88977999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e944b0bd7dc5e8a3abc0784d0bbca0b06bf94e01f94133c299086f0ab5db977b`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50240058fe79dd7c3e564cbe912654ac3d47ff0b4ec8cf8843727f57594b73bc`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9.4-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:79b920fffb62ce6a5a5d43710462a5ee875839d137278cd648e98e4888851a0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119532750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c1a22b2569dd6f45c61a2a09a52ee5ac7577df02b9e510c73e4ef5e0798155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:03:13 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:03:13 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:03:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:03:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:03:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:03:44 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:03:45 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:03:45 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:03:45 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272871ff5a39e7f724ba60200020bda369282194ceb0a7fbacace8a0c1a6bd3`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a8ba951405415f1411b29b725fc469af2374cb7c4f24018f4f0ff7802d236d`  
		Last Modified: Fri, 11 Nov 2022 03:09:54 GMT  
		Size: 85.5 MB (85468667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89a1761c7bc6b466cd2efb4d28b9a0fc4fb55be84ded124f3922236ecf7c3af`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4932db4ceb6992a81f9ab516f105280d520e93584dc1b3302f0fa0d9feb96e57`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 7.0 KB (6952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:jammy`

```console
$ docker pull mariadb@sha256:4d0d7e05cac3f285cb7b38226e8f61f406c6ea2527c317ec2b31a5f5270d7fb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:91323beb7c5c2fb134d13874504aea4e4608304370423019f277b1f70882f9ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121852276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825ad7e31db8cfc5ffa434e1171060e9f60db49279dd675fc562466da3bc0ea0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:50:58 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:50:59 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:50:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:51:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:51:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:51:33 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:51:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ea015f843833e7db49738387776c15cc20eafdf70ef5045dff63f0737b4f2`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c861410f2b3e963a06afa4ca24fda97e00c496b9dc2a3ced1f8affa8f94293f`  
		Last Modified: Fri, 11 Nov 2022 01:58:12 GMT  
		Size: 85.9 MB (85885285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46193445bc4f96aba11e38a4481b43380bee2c095422d3df722641dcad6bc477`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262eb9124c0aca8d6780dfa07f0a43ff16308aa84d6f2c84e5566a0d975bd9dd`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:31f677ba9b50beef8d48a3bbcab29485f5aa3a90677d1ebc44039bbc9bc8bde4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118604917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe889c390f208ce09bf8bfa7869b7d342d999c4279a8809e3a2d2a14332cf10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:07:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 20:07:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:35 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 20:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 20:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 20:07:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 20:08:36 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 20:08:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 20:08:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 20:08:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 20:08:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:08:55 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 20:08:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf568f815bdc2b755b642d6cad079d9e2e71dd364d2806bf4a9a3cb0fe3d18b7`  
		Last Modified: Wed, 02 Nov 2022 20:10:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a27635d8616b3a361adc11c7e5712c05d3edef95c0573370b2c92058ed582`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 3.7 MB (3737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce0b0cfd1e867e47d514f1de07a5da365d36bfb15513e7cf310802577ab13c`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 1.9 MB (1898793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd291b4a9d31c95c30d2580b470dd4ecbe4d2d10c11e47967a037f8b939146e`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505d811110d4c6311181f11307bd36ac49e38d1ab561c611e562b293b90a9ef`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 2.2 MB (2191982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf7ac4a18820861abff79a668773c9f881f45b6f47d10f21df0661e7190013b`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5452b6a0ce3706d857279cfa1cdaef7c8b6bc76d8d6a4b1c43367203b766cd2f`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2628f7ef3cedd084f9a47495aa153853592da56561a6e3231a78435d95ff9949`  
		Last Modified: Wed, 02 Nov 2022 20:10:44 GMT  
		Size: 82.4 MB (82378919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e903661ffaca59211d235a8061c23cc51afe2459c91999d6e191b263897d86d0`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ecec752f0246a09512597065787135cfb39650e56b627521d6b7a25b44bec`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0b3197dcaae25333f0f203038060ecdea256e57a3dbddac50f28647989b2710d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130653312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837797e389ef277d85639136b3254240872973d0626320986cfffbfb6a87f0b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:21:41 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:21:42 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:21:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:22:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:22:34 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:22:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:22:35 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:22:35 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74756e55e3348ae0fd95c532056ccfd545a53ef391306dc1e40c944f767b424`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87682e9f6b59527390239170077fb830688d0d3ecb3a00ec019774d672fb7c9a`  
		Last Modified: Fri, 11 Nov 2022 03:32:44 GMT  
		Size: 89.0 MB (88977999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e944b0bd7dc5e8a3abc0784d0bbca0b06bf94e01f94133c299086f0ab5db977b`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50240058fe79dd7c3e564cbe912654ac3d47ff0b4ec8cf8843727f57594b73bc`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:79b920fffb62ce6a5a5d43710462a5ee875839d137278cd648e98e4888851a0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119532750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c1a22b2569dd6f45c61a2a09a52ee5ac7577df02b9e510c73e4ef5e0798155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:03:13 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:03:13 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:03:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:03:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:03:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:03:44 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:03:45 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:03:45 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:03:45 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272871ff5a39e7f724ba60200020bda369282194ceb0a7fbacace8a0c1a6bd3`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a8ba951405415f1411b29b725fc469af2374cb7c4f24018f4f0ff7802d236d`  
		Last Modified: Fri, 11 Nov 2022 03:09:54 GMT  
		Size: 85.5 MB (85468667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89a1761c7bc6b466cd2efb4d28b9a0fc4fb55be84ded124f3922236ecf7c3af`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4932db4ceb6992a81f9ab516f105280d520e93584dc1b3302f0fa0d9feb96e57`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 7.0 KB (6952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:4d0d7e05cac3f285cb7b38226e8f61f406c6ea2527c317ec2b31a5f5270d7fb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:91323beb7c5c2fb134d13874504aea4e4608304370423019f277b1f70882f9ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121852276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:825ad7e31db8cfc5ffa434e1171060e9f60db49279dd675fc562466da3bc0ea0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 01:47:50 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 01:47:50 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 01:48:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 01:48:17 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:50:58 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 01:50:59 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 01:50:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 01:50:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 01:51:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 01:51:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 01:51:33 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 01:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 01:51:33 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 01:51:33 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5c4b73b9256bb9ce55509f5e24eda1b080780ceff0db42ce80783cb99efa02`  
		Last Modified: Fri, 11 Nov 2022 01:57:33 GMT  
		Size: 5.5 MB (5528722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f870965a3fa10b9d6b698cec208936020049fc24c1171e5d6f6142fa0282467`  
		Last Modified: Fri, 11 Nov 2022 01:57:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ea015f843833e7db49738387776c15cc20eafdf70ef5045dff63f0737b4f2`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c861410f2b3e963a06afa4ca24fda97e00c496b9dc2a3ced1f8affa8f94293f`  
		Last Modified: Fri, 11 Nov 2022 01:58:12 GMT  
		Size: 85.9 MB (85885285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46193445bc4f96aba11e38a4481b43380bee2c095422d3df722641dcad6bc477`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262eb9124c0aca8d6780dfa07f0a43ff16308aa84d6f2c84e5566a0d975bd9dd`  
		Last Modified: Fri, 11 Nov 2022 01:57:59 GMT  
		Size: 7.0 KB (6950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:31f677ba9b50beef8d48a3bbcab29485f5aa3a90677d1ebc44039bbc9bc8bde4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118604917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe889c390f208ce09bf8bfa7869b7d342d999c4279a8809e3a2d2a14332cf10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:07:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 20:07:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:35 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 20:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 20:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 20:07:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 20:08:36 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 20:08:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 20:08:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 20:08:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 20:08:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:08:55 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 20:08:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf568f815bdc2b755b642d6cad079d9e2e71dd364d2806bf4a9a3cb0fe3d18b7`  
		Last Modified: Wed, 02 Nov 2022 20:10:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a27635d8616b3a361adc11c7e5712c05d3edef95c0573370b2c92058ed582`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 3.7 MB (3737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce0b0cfd1e867e47d514f1de07a5da365d36bfb15513e7cf310802577ab13c`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 1.9 MB (1898793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd291b4a9d31c95c30d2580b470dd4ecbe4d2d10c11e47967a037f8b939146e`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505d811110d4c6311181f11307bd36ac49e38d1ab561c611e562b293b90a9ef`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 2.2 MB (2191982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf7ac4a18820861abff79a668773c9f881f45b6f47d10f21df0661e7190013b`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5452b6a0ce3706d857279cfa1cdaef7c8b6bc76d8d6a4b1c43367203b766cd2f`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2628f7ef3cedd084f9a47495aa153853592da56561a6e3231a78435d95ff9949`  
		Last Modified: Wed, 02 Nov 2022 20:10:44 GMT  
		Size: 82.4 MB (82378919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e903661ffaca59211d235a8061c23cc51afe2459c91999d6e191b263897d86d0`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ecec752f0246a09512597065787135cfb39650e56b627521d6b7a25b44bec`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0b3197dcaae25333f0f203038060ecdea256e57a3dbddac50f28647989b2710d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130653312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837797e389ef277d85639136b3254240872973d0626320986cfffbfb6a87f0b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:19:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:19:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:20:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:20:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:20:28 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:21:41 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:21:42 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:21:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:21:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:22:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:22:34 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:22:34 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:22:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:22:35 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:22:35 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34261ccc1abc87e8bc2183f54100c3bf85fd037f4ebb5a2bc3c7cfbc92079a6`  
		Last Modified: Fri, 11 Nov 2022 03:31:46 GMT  
		Size: 6.0 MB (5955072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483c565231c97d3a42ef6aaa831fa70760df9c9d7588f86c46ec2f16d9d3c188`  
		Last Modified: Fri, 11 Nov 2022 03:31:42 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74756e55e3348ae0fd95c532056ccfd545a53ef391306dc1e40c944f767b424`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87682e9f6b59527390239170077fb830688d0d3ecb3a00ec019774d672fb7c9a`  
		Last Modified: Fri, 11 Nov 2022 03:32:44 GMT  
		Size: 89.0 MB (88977999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e944b0bd7dc5e8a3abc0784d0bbca0b06bf94e01f94133c299086f0ab5db977b`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50240058fe79dd7c3e564cbe912654ac3d47ff0b4ec8cf8843727f57594b73bc`  
		Last Modified: Fri, 11 Nov 2022 03:32:21 GMT  
		Size: 7.0 KB (6951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:79b920fffb62ce6a5a5d43710462a5ee875839d137278cd648e98e4888851a0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119532750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c1a22b2569dd6f45c61a2a09a52ee5ac7577df02b9e510c73e4ef5e0798155`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Nov 2022 03:01:54 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Nov 2022 03:01:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Nov 2022 03:02:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Nov 2022 03:02:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Nov 2022 03:02:19 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 03:03:13 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=10.9.4 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 11 Nov 2022 03:03:13 GMT
ARG MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ENV MARIADB_VERSION=1:10.9.4+maria~ubu2204
# Fri, 11 Nov 2022 03:03:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
# Fri, 11 Nov 2022 03:03:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Nov 2022 03:03:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 11 Nov 2022 03:03:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Nov 2022 03:03:44 GMT
COPY file:889339e755ad928a437caeaa979e26ba168ae42039fb519e6d5b31d29bcce082 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Nov 2022 03:03:45 GMT
COPY file:8ff49c407a76d8990281701d57bd3af69835977acdff7e2905ae6052323b3ebd in /usr/local/bin/ 
# Fri, 11 Nov 2022 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 03:03:45 GMT
EXPOSE 3306
# Fri, 11 Nov 2022 03:03:45 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1612a290ef38204b4266c92dcabfc38752b746b73054fee500efee65da3404db`  
		Last Modified: Fri, 11 Nov 2022 03:09:23 GMT  
		Size: 5.4 MB (5410665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8492b0a8fcac17f2fd068f41c231ca5f096ca7e588a9286168d7ed60cfcd4b`  
		Last Modified: Fri, 11 Nov 2022 03:09:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272871ff5a39e7f724ba60200020bda369282194ceb0a7fbacace8a0c1a6bd3`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a8ba951405415f1411b29b725fc469af2374cb7c4f24018f4f0ff7802d236d`  
		Last Modified: Fri, 11 Nov 2022 03:09:54 GMT  
		Size: 85.5 MB (85468667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89a1761c7bc6b466cd2efb4d28b9a0fc4fb55be84ded124f3922236ecf7c3af`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4932db4ceb6992a81f9ab516f105280d520e93584dc1b3302f0fa0d9feb96e57`  
		Last Modified: Fri, 11 Nov 2022 03:09:42 GMT  
		Size: 7.0 KB (6952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
