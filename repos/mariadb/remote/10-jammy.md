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
