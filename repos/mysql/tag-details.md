<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5-debian`](#mysql5-debian)
-	[`mysql:5-oracle`](#mysql5-oracle)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7-debian`](#mysql57-debian)
-	[`mysql:5.7-oracle`](#mysql57-oracle)
-	[`mysql:5.7.37`](#mysql5737)
-	[`mysql:5.7.37-debian`](#mysql5737-debian)
-	[`mysql:5.7.37-oracle`](#mysql5737-oracle)
-	[`mysql:8`](#mysql8)
-	[`mysql:8-debian`](#mysql8-debian)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0.28`](#mysql8028)
-	[`mysql:8.0.28-debian`](#mysql8028-debian)
-	[`mysql:8.0.28-oracle`](#mysql8028-oracle)
-	[`mysql:debian`](#mysqldebian)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)

## `mysql:5`

```console
$ docker pull mysql@sha256:1a73b6a8f507639a8f91ed01ace28965f4f74bb62a9d9b9e7378d5f07fab79dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:f30790aa9f367de69a4c440c1f4bc17df588723036cac4191a31456e8c32aa66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155429115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f26e21ddd20df245d88410116241f3eef1ec49ce888856c95b85081a7250183d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:09:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 29 Mar 2022 18:09:07 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Tue, 29 Mar 2022 18:09:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:09:27 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:09:27 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:09:28 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:09:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:09:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:09:28 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:09:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba61822c65c2f08f4f96e39055c0df7bcc8a0be134483a651c61e6025540b462`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec59acdf78a928e150027aa5bca7d01c2e5f0a1b4cfdab216d90bb385c05c58`  
		Last Modified: Tue, 29 Mar 2022 18:10:57 GMT  
		Size: 108.6 MB (108637125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a05235a6981099aaad91858481f02ca69a8459bff87307676b72f2490908fd1`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87d621d691622f91858909d89946ed80b873449377f285a13f3d1d7ffdcb4f0`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:1a73b6a8f507639a8f91ed01ace28965f4f74bb62a9d9b9e7378d5f07fab79dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:f30790aa9f367de69a4c440c1f4bc17df588723036cac4191a31456e8c32aa66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155429115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f26e21ddd20df245d88410116241f3eef1ec49ce888856c95b85081a7250183d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:09:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 29 Mar 2022 18:09:07 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Tue, 29 Mar 2022 18:09:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:09:27 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:09:27 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:09:28 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:09:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:09:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:09:28 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:09:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba61822c65c2f08f4f96e39055c0df7bcc8a0be134483a651c61e6025540b462`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec59acdf78a928e150027aa5bca7d01c2e5f0a1b4cfdab216d90bb385c05c58`  
		Last Modified: Tue, 29 Mar 2022 18:10:57 GMT  
		Size: 108.6 MB (108637125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a05235a6981099aaad91858481f02ca69a8459bff87307676b72f2490908fd1`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87d621d691622f91858909d89946ed80b873449377f285a13f3d1d7ffdcb4f0`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:8962a5b45272d182f83f5740e88c518436a645d29b3de013680b5e4aff6d3de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:0fa6fe4d97d23662a23dca6350c388338767b7281a7e0be926fb62aa406d5d77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125179560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e1e4a93d3d4d84af0ffc4f12d29433575faf8a8d68cebf0fe55802e44d188f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 22:26:41 GMT
ADD file:c54c465abf0c60dc924ca0809a1a862121214379efe90dacb9c9947c81054213 in / 
# Thu, 24 Mar 2022 22:26:42 GMT
CMD ["/bin/bash"]
# Fri, 25 Mar 2022 01:14:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 25 Mar 2022 01:14:04 GMT
ENV GOSU_VERSION=1.14
# Fri, 25 Mar 2022 01:14:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Mar 2022 01:14:17 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 25 Mar 2022 01:14:18 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 25 Mar 2022 01:14:18 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 25 Mar 2022 01:14:18 GMT
ENV MYSQL_VERSION=5.7.37-1.el7
# Fri, 25 Mar 2022 01:14:18 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 25 Mar 2022 01:14:31 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Fri, 25 Mar 2022 01:14:32 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 25 Mar 2022 01:14:32 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el7
# Fri, 25 Mar 2022 01:14:48 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Fri, 25 Mar 2022 01:14:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Mar 2022 01:14:49 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 25 Mar 2022 01:14:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Mar 2022 01:14:49 GMT
EXPOSE 3306 33060
# Fri, 25 Mar 2022 01:14:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fda5369ef22868b2225eb458f776aabaf140371e2f8d709c4de99b69a02ae748`  
		Last Modified: Thu, 24 Mar 2022 22:28:00 GMT  
		Size: 48.7 MB (48749451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b58b3893c085f11af6e5ca6b087be43aec1893003a9e7b2556ce9e3bafef4`  
		Last Modified: Fri, 25 Mar 2022 01:15:47 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea650c51b90deed10e9f6099b31fb82607fb6d5cc72a3888cebb4fe6a72126`  
		Last Modified: Fri, 25 Mar 2022 01:15:45 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f1a9443c8eda03be6762f9b513cd9ebb7a67e7d5b7c8e01b1650b3e107ace0`  
		Last Modified: Fri, 25 Mar 2022 01:15:46 GMT  
		Size: 3.7 MB (3723980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2bb1a4c9a1619a3665f5b4debb10d34faf07eac811404f8adb23ced825a2d`  
		Last Modified: Fri, 25 Mar 2022 01:15:45 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c6c5585f2fd11140279e78a8e68b4d44f7521e9b98cad74515d663d01e87be`  
		Last Modified: Fri, 25 Mar 2022 01:15:42 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76392f3c32db20513b0e963d6475fd396ce1d89748939521dea2aca0ae8522e`  
		Last Modified: Fri, 25 Mar 2022 01:15:47 GMT  
		Size: 25.5 MB (25454525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1963192a3bfe0201fb85f40c06a4dbfe9d0831bf31a3a7256c958447bf0f939d`  
		Last Modified: Fri, 25 Mar 2022 01:15:43 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7676c869d791c0ef5e3f0db6713d2a02bb38d93e893a4c9eb785b898d306ae54`  
		Last Modified: Fri, 25 Mar 2022 01:15:51 GMT  
		Size: 46.3 MB (46311870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e4c1264e439d0e9d1095f0e9b9cefee52f27e443b0cf553442e4170f8b5a92`  
		Last Modified: Fri, 25 Mar 2022 01:15:43 GMT  
		Size: 5.1 KB (5141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:1a73b6a8f507639a8f91ed01ace28965f4f74bb62a9d9b9e7378d5f07fab79dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:f30790aa9f367de69a4c440c1f4bc17df588723036cac4191a31456e8c32aa66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155429115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f26e21ddd20df245d88410116241f3eef1ec49ce888856c95b85081a7250183d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:09:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 29 Mar 2022 18:09:07 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Tue, 29 Mar 2022 18:09:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:09:27 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:09:27 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:09:28 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:09:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:09:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:09:28 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:09:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba61822c65c2f08f4f96e39055c0df7bcc8a0be134483a651c61e6025540b462`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec59acdf78a928e150027aa5bca7d01c2e5f0a1b4cfdab216d90bb385c05c58`  
		Last Modified: Tue, 29 Mar 2022 18:10:57 GMT  
		Size: 108.6 MB (108637125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a05235a6981099aaad91858481f02ca69a8459bff87307676b72f2490908fd1`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87d621d691622f91858909d89946ed80b873449377f285a13f3d1d7ffdcb4f0`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:1a73b6a8f507639a8f91ed01ace28965f4f74bb62a9d9b9e7378d5f07fab79dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:f30790aa9f367de69a4c440c1f4bc17df588723036cac4191a31456e8c32aa66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155429115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f26e21ddd20df245d88410116241f3eef1ec49ce888856c95b85081a7250183d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:09:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 29 Mar 2022 18:09:07 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Tue, 29 Mar 2022 18:09:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:09:27 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:09:27 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:09:28 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:09:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:09:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:09:28 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:09:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba61822c65c2f08f4f96e39055c0df7bcc8a0be134483a651c61e6025540b462`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec59acdf78a928e150027aa5bca7d01c2e5f0a1b4cfdab216d90bb385c05c58`  
		Last Modified: Tue, 29 Mar 2022 18:10:57 GMT  
		Size: 108.6 MB (108637125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a05235a6981099aaad91858481f02ca69a8459bff87307676b72f2490908fd1`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87d621d691622f91858909d89946ed80b873449377f285a13f3d1d7ffdcb4f0`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:8962a5b45272d182f83f5740e88c518436a645d29b3de013680b5e4aff6d3de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:0fa6fe4d97d23662a23dca6350c388338767b7281a7e0be926fb62aa406d5d77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125179560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e1e4a93d3d4d84af0ffc4f12d29433575faf8a8d68cebf0fe55802e44d188f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 22:26:41 GMT
ADD file:c54c465abf0c60dc924ca0809a1a862121214379efe90dacb9c9947c81054213 in / 
# Thu, 24 Mar 2022 22:26:42 GMT
CMD ["/bin/bash"]
# Fri, 25 Mar 2022 01:14:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 25 Mar 2022 01:14:04 GMT
ENV GOSU_VERSION=1.14
# Fri, 25 Mar 2022 01:14:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Mar 2022 01:14:17 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 25 Mar 2022 01:14:18 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 25 Mar 2022 01:14:18 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 25 Mar 2022 01:14:18 GMT
ENV MYSQL_VERSION=5.7.37-1.el7
# Fri, 25 Mar 2022 01:14:18 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 25 Mar 2022 01:14:31 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Fri, 25 Mar 2022 01:14:32 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 25 Mar 2022 01:14:32 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el7
# Fri, 25 Mar 2022 01:14:48 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Fri, 25 Mar 2022 01:14:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Mar 2022 01:14:49 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 25 Mar 2022 01:14:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Mar 2022 01:14:49 GMT
EXPOSE 3306 33060
# Fri, 25 Mar 2022 01:14:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fda5369ef22868b2225eb458f776aabaf140371e2f8d709c4de99b69a02ae748`  
		Last Modified: Thu, 24 Mar 2022 22:28:00 GMT  
		Size: 48.7 MB (48749451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b58b3893c085f11af6e5ca6b087be43aec1893003a9e7b2556ce9e3bafef4`  
		Last Modified: Fri, 25 Mar 2022 01:15:47 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea650c51b90deed10e9f6099b31fb82607fb6d5cc72a3888cebb4fe6a72126`  
		Last Modified: Fri, 25 Mar 2022 01:15:45 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f1a9443c8eda03be6762f9b513cd9ebb7a67e7d5b7c8e01b1650b3e107ace0`  
		Last Modified: Fri, 25 Mar 2022 01:15:46 GMT  
		Size: 3.7 MB (3723980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2bb1a4c9a1619a3665f5b4debb10d34faf07eac811404f8adb23ced825a2d`  
		Last Modified: Fri, 25 Mar 2022 01:15:45 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c6c5585f2fd11140279e78a8e68b4d44f7521e9b98cad74515d663d01e87be`  
		Last Modified: Fri, 25 Mar 2022 01:15:42 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76392f3c32db20513b0e963d6475fd396ce1d89748939521dea2aca0ae8522e`  
		Last Modified: Fri, 25 Mar 2022 01:15:47 GMT  
		Size: 25.5 MB (25454525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1963192a3bfe0201fb85f40c06a4dbfe9d0831bf31a3a7256c958447bf0f939d`  
		Last Modified: Fri, 25 Mar 2022 01:15:43 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7676c869d791c0ef5e3f0db6713d2a02bb38d93e893a4c9eb785b898d306ae54`  
		Last Modified: Fri, 25 Mar 2022 01:15:51 GMT  
		Size: 46.3 MB (46311870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e4c1264e439d0e9d1095f0e9b9cefee52f27e443b0cf553442e4170f8b5a92`  
		Last Modified: Fri, 25 Mar 2022 01:15:43 GMT  
		Size: 5.1 KB (5141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.37`

```console
$ docker pull mysql@sha256:1a73b6a8f507639a8f91ed01ace28965f4f74bb62a9d9b9e7378d5f07fab79dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.37` - linux; amd64

```console
$ docker pull mysql@sha256:f30790aa9f367de69a4c440c1f4bc17df588723036cac4191a31456e8c32aa66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155429115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f26e21ddd20df245d88410116241f3eef1ec49ce888856c95b85081a7250183d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:09:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 29 Mar 2022 18:09:07 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Tue, 29 Mar 2022 18:09:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:09:27 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:09:27 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:09:28 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:09:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:09:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:09:28 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:09:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba61822c65c2f08f4f96e39055c0df7bcc8a0be134483a651c61e6025540b462`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec59acdf78a928e150027aa5bca7d01c2e5f0a1b4cfdab216d90bb385c05c58`  
		Last Modified: Tue, 29 Mar 2022 18:10:57 GMT  
		Size: 108.6 MB (108637125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a05235a6981099aaad91858481f02ca69a8459bff87307676b72f2490908fd1`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87d621d691622f91858909d89946ed80b873449377f285a13f3d1d7ffdcb4f0`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.37-debian`

```console
$ docker pull mysql@sha256:1a73b6a8f507639a8f91ed01ace28965f4f74bb62a9d9b9e7378d5f07fab79dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.37-debian` - linux; amd64

```console
$ docker pull mysql@sha256:f30790aa9f367de69a4c440c1f4bc17df588723036cac4191a31456e8c32aa66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155429115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f26e21ddd20df245d88410116241f3eef1ec49ce888856c95b85081a7250183d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:09:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 29 Mar 2022 18:09:07 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Tue, 29 Mar 2022 18:09:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:09:27 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:09:27 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:09:28 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:09:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:09:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:09:28 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:09:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba61822c65c2f08f4f96e39055c0df7bcc8a0be134483a651c61e6025540b462`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec59acdf78a928e150027aa5bca7d01c2e5f0a1b4cfdab216d90bb385c05c58`  
		Last Modified: Tue, 29 Mar 2022 18:10:57 GMT  
		Size: 108.6 MB (108637125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a05235a6981099aaad91858481f02ca69a8459bff87307676b72f2490908fd1`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87d621d691622f91858909d89946ed80b873449377f285a13f3d1d7ffdcb4f0`  
		Last Modified: Tue, 29 Mar 2022 18:10:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.37-oracle`

```console
$ docker pull mysql@sha256:8962a5b45272d182f83f5740e88c518436a645d29b3de013680b5e4aff6d3de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.37-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:0fa6fe4d97d23662a23dca6350c388338767b7281a7e0be926fb62aa406d5d77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125179560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e1e4a93d3d4d84af0ffc4f12d29433575faf8a8d68cebf0fe55802e44d188f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 22:26:41 GMT
ADD file:c54c465abf0c60dc924ca0809a1a862121214379efe90dacb9c9947c81054213 in / 
# Thu, 24 Mar 2022 22:26:42 GMT
CMD ["/bin/bash"]
# Fri, 25 Mar 2022 01:14:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 25 Mar 2022 01:14:04 GMT
ENV GOSU_VERSION=1.14
# Fri, 25 Mar 2022 01:14:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Mar 2022 01:14:17 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 25 Mar 2022 01:14:18 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 25 Mar 2022 01:14:18 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 25 Mar 2022 01:14:18 GMT
ENV MYSQL_VERSION=5.7.37-1.el7
# Fri, 25 Mar 2022 01:14:18 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 25 Mar 2022 01:14:31 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Fri, 25 Mar 2022 01:14:32 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 25 Mar 2022 01:14:32 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el7
# Fri, 25 Mar 2022 01:14:48 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Fri, 25 Mar 2022 01:14:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Mar 2022 01:14:49 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 25 Mar 2022 01:14:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Mar 2022 01:14:49 GMT
EXPOSE 3306 33060
# Fri, 25 Mar 2022 01:14:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fda5369ef22868b2225eb458f776aabaf140371e2f8d709c4de99b69a02ae748`  
		Last Modified: Thu, 24 Mar 2022 22:28:00 GMT  
		Size: 48.7 MB (48749451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b58b3893c085f11af6e5ca6b087be43aec1893003a9e7b2556ce9e3bafef4`  
		Last Modified: Fri, 25 Mar 2022 01:15:47 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea650c51b90deed10e9f6099b31fb82607fb6d5cc72a3888cebb4fe6a72126`  
		Last Modified: Fri, 25 Mar 2022 01:15:45 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f1a9443c8eda03be6762f9b513cd9ebb7a67e7d5b7c8e01b1650b3e107ace0`  
		Last Modified: Fri, 25 Mar 2022 01:15:46 GMT  
		Size: 3.7 MB (3723980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2bb1a4c9a1619a3665f5b4debb10d34faf07eac811404f8adb23ced825a2d`  
		Last Modified: Fri, 25 Mar 2022 01:15:45 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c6c5585f2fd11140279e78a8e68b4d44f7521e9b98cad74515d663d01e87be`  
		Last Modified: Fri, 25 Mar 2022 01:15:42 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76392f3c32db20513b0e963d6475fd396ce1d89748939521dea2aca0ae8522e`  
		Last Modified: Fri, 25 Mar 2022 01:15:47 GMT  
		Size: 25.5 MB (25454525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1963192a3bfe0201fb85f40c06a4dbfe9d0831bf31a3a7256c958447bf0f939d`  
		Last Modified: Fri, 25 Mar 2022 01:15:43 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7676c869d791c0ef5e3f0db6713d2a02bb38d93e893a4c9eb785b898d306ae54`  
		Last Modified: Fri, 25 Mar 2022 01:15:51 GMT  
		Size: 46.3 MB (46311870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e4c1264e439d0e9d1095f0e9b9cefee52f27e443b0cf553442e4170f8b5a92`  
		Last Modified: Fri, 25 Mar 2022 01:15:43 GMT  
		Size: 5.1 KB (5141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:1c75ba7716c6f73fc106dacedfdcf13f934ea8c161c8b3b3e4618bcd5fbcf195
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:8cdf596eb3fba84ae6d0ad683d330dcaf87ef8fb51e4d5dd9f1e289c5012e0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154597910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:667ee8fb158e365450fc3f09712208fe44e9f1364a9b130fed95f3f4862f8a63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Tue, 29 Mar 2022 18:08:41 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:08:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:08:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:08:56 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 29 Mar 2022 18:08:56 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:08:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:08:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:08:57 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:08:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6ea71d471d2d38ef59731ae2b31379ddd9163c4da92c1de543d8bd4f97fedf`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2920c795b25d6cd74b842f7329b94e1d7c5482885a3158589a6bc680c616fa4`  
		Last Modified: Tue, 29 Mar 2022 18:10:11 GMT  
		Size: 107.8 MB (107805075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c3bdf75ff5618cd6b7d60004bfb8cb8759026305eef07d986afa6e46454b15`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec1f1f78b0e9e0d09b58d1be3497429eb5c0f76f8dcf01371bcd6f9d019715d`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4607fa685ac65df86f44720e2b8a69e97f835483a5aa8fa139048e75e00f38ff`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:1c75ba7716c6f73fc106dacedfdcf13f934ea8c161c8b3b3e4618bcd5fbcf195
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:8cdf596eb3fba84ae6d0ad683d330dcaf87ef8fb51e4d5dd9f1e289c5012e0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154597910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:667ee8fb158e365450fc3f09712208fe44e9f1364a9b130fed95f3f4862f8a63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Tue, 29 Mar 2022 18:08:41 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:08:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:08:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:08:56 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 29 Mar 2022 18:08:56 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:08:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:08:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:08:57 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:08:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6ea71d471d2d38ef59731ae2b31379ddd9163c4da92c1de543d8bd4f97fedf`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2920c795b25d6cd74b842f7329b94e1d7c5482885a3158589a6bc680c616fa4`  
		Last Modified: Tue, 29 Mar 2022 18:10:11 GMT  
		Size: 107.8 MB (107805075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c3bdf75ff5618cd6b7d60004bfb8cb8759026305eef07d986afa6e46454b15`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec1f1f78b0e9e0d09b58d1be3497429eb5c0f76f8dcf01371bcd6f9d019715d`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4607fa685ac65df86f44720e2b8a69e97f835483a5aa8fa139048e75e00f38ff`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:32054d8d010726bee26052cd4ac1b8d76db55180f6ac976e5fc6279190e896cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:e1866c1d0f58b69de7fa0b5986564ae044784f0dd1c61c01bbf3ec1470784312
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133139496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce4b41e88ebc537d8fe49c51d193e0d69307c49886cdad58a83ab738afe3522`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 22:26:17 GMT
ADD file:ebb4986af4fcca0d00738e77d2c814e70536c01a0e02eef98c71e9e3a56c0abd in / 
# Thu, 24 Mar 2022 22:26:18 GMT
CMD ["/bin/bash"]
# Fri, 25 Mar 2022 01:12:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 25 Mar 2022 01:12:38 GMT
ENV GOSU_VERSION=1.14
# Fri, 25 Mar 2022 01:12:41 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Mar 2022 01:13:00 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 25 Mar 2022 01:13:02 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 25 Mar 2022 01:13:02 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 25 Mar 2022 01:13:02 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Fri, 25 Mar 2022 01:13:02 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 25 Mar 2022 01:13:26 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Fri, 25 Mar 2022 01:13:27 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 25 Mar 2022 01:13:27 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Fri, 25 Mar 2022 01:13:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 25 Mar 2022 01:13:55 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Mar 2022 01:13:55 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 25 Mar 2022 01:13:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Mar 2022 01:13:55 GMT
EXPOSE 3306 33060
# Fri, 25 Mar 2022 01:13:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1de6f411eccf5041d90362d2d035abf0e59cf91dce4eacbc37ef0aa52f5b5920`  
		Last Modified: Thu, 24 Mar 2022 22:27:23 GMT  
		Size: 42.1 MB (42111629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7750893065cbe5478b40ebf1b3f4a424e4bff391ecfcd9355140adc25715de`  
		Last Modified: Fri, 25 Mar 2022 01:15:20 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf1e489f4aae4498fc2f96f3dbd32459bf28b5500980eb189896fe0781bbd39`  
		Last Modified: Fri, 25 Mar 2022 01:15:18 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a64bfd09b448f5ebe279c4b42eb6a98d6cd9b2a203c84e1e1179cc40d554c65`  
		Last Modified: Fri, 25 Mar 2022 01:15:18 GMT  
		Size: 4.5 MB (4547133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439534ad10016b75ec2760171452fdc19f522fcd321f4d9559aa98e93d090245`  
		Last Modified: Fri, 25 Mar 2022 01:15:18 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ba31e211ec3bc3f21d9e79ba88961da072db9951a42bf34f7f75575c2f22a2`  
		Last Modified: Fri, 25 Mar 2022 01:15:15 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb32dad74239c798b8edc0734070af95cc5fc2400f6c23e43204deaf27198ab`  
		Last Modified: Fri, 25 Mar 2022 01:15:23 GMT  
		Size: 47.3 MB (47267324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d728d0b568cbe11d3ec4a20552a005f259ef4db49c7aac61e6141248904912`  
		Last Modified: Fri, 25 Mar 2022 01:15:15 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d30611313f049519c61520bb7b8653a63d87f18bbe13d9ba96af57ed90a717a`  
		Last Modified: Fri, 25 Mar 2022 01:15:23 GMT  
		Size: 38.3 MB (38275082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829b3d97de2a870cc6f6976d671eea1e7818931e14c6e792bfa8c705ab0949a7`  
		Last Modified: Fri, 25 Mar 2022 01:15:15 GMT  
		Size: 5.1 KB (5140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c31271d3ea18ed5d8c8b2d255e675a8599801d571d58fee7b293cececcf1d1fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141175486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf5b46dfe3694e200010e9e0574770af8b1a7d2d1ef9e6ae7b664578f048b10e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 22:21:09 GMT
ADD file:1eaca9dccdbe88c4fac0b484a625100443af30879cf6cba7b5615db77745b0c7 in / 
# Thu, 24 Mar 2022 22:21:10 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 23:11:19 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 24 Mar 2022 23:11:20 GMT
ENV GOSU_VERSION=1.14
# Thu, 24 Mar 2022 23:11:23 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 24 Mar 2022 23:11:43 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 24 Mar 2022 23:11:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 24 Mar 2022 23:11:46 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 24 Mar 2022 23:11:47 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 23:11:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 24 Mar 2022 23:12:12 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 24 Mar 2022 23:12:12 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 24 Mar 2022 23:12:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 23:12:37 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 24 Mar 2022 23:12:38 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Mar 2022 23:12:40 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Thu, 24 Mar 2022 23:12:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 23:12:41 GMT
EXPOSE 3306 33060
# Thu, 24 Mar 2022 23:12:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c11319b13f376dfb3fa1ee22d0047cfb7157eba4ba2786653cb29ac6defcb93c`  
		Last Modified: Thu, 24 Mar 2022 22:22:26 GMT  
		Size: 42.0 MB (42018948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba57e28a536434d0ba46750553b143b00eb996ef81ded45f4df4a30a5487c750`  
		Last Modified: Thu, 24 Mar 2022 23:13:17 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbb305818ad837064d616414049e197543cdffb0bc3c48046a7d3271b3e1b5e`  
		Last Modified: Thu, 24 Mar 2022 23:13:15 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6245bb06bb46ba0c35b7433234c72c1685ff5e9c938e0d498897b2c79951fd`  
		Last Modified: Thu, 24 Mar 2022 23:13:15 GMT  
		Size: 4.4 MB (4378824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b57640c9c7786162fe68c440e7fc35fa6a4f59dfc8b2c05ead4a85eb5a7e9f`  
		Last Modified: Thu, 24 Mar 2022 23:13:14 GMT  
		Size: 2.6 KB (2604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733dab4a1602b172f16690529dc18c051788f5403d52caff3703fae8c4ccdb37`  
		Last Modified: Thu, 24 Mar 2022 23:13:12 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb800e2c9b9dd594d7cc7e5b777e6b548a09d55234d2f3a547cf7a11f24ce2d`  
		Last Modified: Thu, 24 Mar 2022 23:13:19 GMT  
		Size: 53.4 MB (53429969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bf9d82ddd548e76ee83ba27fbbfd69d45f00aa73993e83f796c6b448d7f503`  
		Last Modified: Thu, 24 Mar 2022 23:13:12 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915025a8362d74e5f93a614dc592dc258a2dc0985cd6fb9d903a974ab0b823d1`  
		Last Modified: Thu, 24 Mar 2022 23:13:19 GMT  
		Size: 40.5 MB (40481181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9317ed1ad35f14a9b32b10227b398a129812dafd444475214d3ccf51c86d265d`  
		Last Modified: Thu, 24 Mar 2022 23:13:12 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:1c75ba7716c6f73fc106dacedfdcf13f934ea8c161c8b3b3e4618bcd5fbcf195
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:8cdf596eb3fba84ae6d0ad683d330dcaf87ef8fb51e4d5dd9f1e289c5012e0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154597910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:667ee8fb158e365450fc3f09712208fe44e9f1364a9b130fed95f3f4862f8a63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Tue, 29 Mar 2022 18:08:41 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:08:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:08:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:08:56 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 29 Mar 2022 18:08:56 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:08:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:08:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:08:57 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:08:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6ea71d471d2d38ef59731ae2b31379ddd9163c4da92c1de543d8bd4f97fedf`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2920c795b25d6cd74b842f7329b94e1d7c5482885a3158589a6bc680c616fa4`  
		Last Modified: Tue, 29 Mar 2022 18:10:11 GMT  
		Size: 107.8 MB (107805075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c3bdf75ff5618cd6b7d60004bfb8cb8759026305eef07d986afa6e46454b15`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec1f1f78b0e9e0d09b58d1be3497429eb5c0f76f8dcf01371bcd6f9d019715d`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4607fa685ac65df86f44720e2b8a69e97f835483a5aa8fa139048e75e00f38ff`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:1c75ba7716c6f73fc106dacedfdcf13f934ea8c161c8b3b3e4618bcd5fbcf195
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:8cdf596eb3fba84ae6d0ad683d330dcaf87ef8fb51e4d5dd9f1e289c5012e0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154597910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:667ee8fb158e365450fc3f09712208fe44e9f1364a9b130fed95f3f4862f8a63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Tue, 29 Mar 2022 18:08:41 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:08:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:08:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:08:56 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 29 Mar 2022 18:08:56 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:08:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:08:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:08:57 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:08:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6ea71d471d2d38ef59731ae2b31379ddd9163c4da92c1de543d8bd4f97fedf`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2920c795b25d6cd74b842f7329b94e1d7c5482885a3158589a6bc680c616fa4`  
		Last Modified: Tue, 29 Mar 2022 18:10:11 GMT  
		Size: 107.8 MB (107805075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c3bdf75ff5618cd6b7d60004bfb8cb8759026305eef07d986afa6e46454b15`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec1f1f78b0e9e0d09b58d1be3497429eb5c0f76f8dcf01371bcd6f9d019715d`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4607fa685ac65df86f44720e2b8a69e97f835483a5aa8fa139048e75e00f38ff`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:32054d8d010726bee26052cd4ac1b8d76db55180f6ac976e5fc6279190e896cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:e1866c1d0f58b69de7fa0b5986564ae044784f0dd1c61c01bbf3ec1470784312
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133139496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce4b41e88ebc537d8fe49c51d193e0d69307c49886cdad58a83ab738afe3522`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 22:26:17 GMT
ADD file:ebb4986af4fcca0d00738e77d2c814e70536c01a0e02eef98c71e9e3a56c0abd in / 
# Thu, 24 Mar 2022 22:26:18 GMT
CMD ["/bin/bash"]
# Fri, 25 Mar 2022 01:12:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 25 Mar 2022 01:12:38 GMT
ENV GOSU_VERSION=1.14
# Fri, 25 Mar 2022 01:12:41 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Mar 2022 01:13:00 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 25 Mar 2022 01:13:02 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 25 Mar 2022 01:13:02 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 25 Mar 2022 01:13:02 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Fri, 25 Mar 2022 01:13:02 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 25 Mar 2022 01:13:26 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Fri, 25 Mar 2022 01:13:27 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 25 Mar 2022 01:13:27 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Fri, 25 Mar 2022 01:13:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 25 Mar 2022 01:13:55 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Mar 2022 01:13:55 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 25 Mar 2022 01:13:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Mar 2022 01:13:55 GMT
EXPOSE 3306 33060
# Fri, 25 Mar 2022 01:13:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1de6f411eccf5041d90362d2d035abf0e59cf91dce4eacbc37ef0aa52f5b5920`  
		Last Modified: Thu, 24 Mar 2022 22:27:23 GMT  
		Size: 42.1 MB (42111629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7750893065cbe5478b40ebf1b3f4a424e4bff391ecfcd9355140adc25715de`  
		Last Modified: Fri, 25 Mar 2022 01:15:20 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf1e489f4aae4498fc2f96f3dbd32459bf28b5500980eb189896fe0781bbd39`  
		Last Modified: Fri, 25 Mar 2022 01:15:18 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a64bfd09b448f5ebe279c4b42eb6a98d6cd9b2a203c84e1e1179cc40d554c65`  
		Last Modified: Fri, 25 Mar 2022 01:15:18 GMT  
		Size: 4.5 MB (4547133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439534ad10016b75ec2760171452fdc19f522fcd321f4d9559aa98e93d090245`  
		Last Modified: Fri, 25 Mar 2022 01:15:18 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ba31e211ec3bc3f21d9e79ba88961da072db9951a42bf34f7f75575c2f22a2`  
		Last Modified: Fri, 25 Mar 2022 01:15:15 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb32dad74239c798b8edc0734070af95cc5fc2400f6c23e43204deaf27198ab`  
		Last Modified: Fri, 25 Mar 2022 01:15:23 GMT  
		Size: 47.3 MB (47267324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d728d0b568cbe11d3ec4a20552a005f259ef4db49c7aac61e6141248904912`  
		Last Modified: Fri, 25 Mar 2022 01:15:15 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d30611313f049519c61520bb7b8653a63d87f18bbe13d9ba96af57ed90a717a`  
		Last Modified: Fri, 25 Mar 2022 01:15:23 GMT  
		Size: 38.3 MB (38275082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829b3d97de2a870cc6f6976d671eea1e7818931e14c6e792bfa8c705ab0949a7`  
		Last Modified: Fri, 25 Mar 2022 01:15:15 GMT  
		Size: 5.1 KB (5140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c31271d3ea18ed5d8c8b2d255e675a8599801d571d58fee7b293cececcf1d1fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141175486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf5b46dfe3694e200010e9e0574770af8b1a7d2d1ef9e6ae7b664578f048b10e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 22:21:09 GMT
ADD file:1eaca9dccdbe88c4fac0b484a625100443af30879cf6cba7b5615db77745b0c7 in / 
# Thu, 24 Mar 2022 22:21:10 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 23:11:19 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 24 Mar 2022 23:11:20 GMT
ENV GOSU_VERSION=1.14
# Thu, 24 Mar 2022 23:11:23 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 24 Mar 2022 23:11:43 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 24 Mar 2022 23:11:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 24 Mar 2022 23:11:46 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 24 Mar 2022 23:11:47 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 23:11:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 24 Mar 2022 23:12:12 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 24 Mar 2022 23:12:12 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 24 Mar 2022 23:12:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 23:12:37 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 24 Mar 2022 23:12:38 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Mar 2022 23:12:40 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Thu, 24 Mar 2022 23:12:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 23:12:41 GMT
EXPOSE 3306 33060
# Thu, 24 Mar 2022 23:12:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c11319b13f376dfb3fa1ee22d0047cfb7157eba4ba2786653cb29ac6defcb93c`  
		Last Modified: Thu, 24 Mar 2022 22:22:26 GMT  
		Size: 42.0 MB (42018948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba57e28a536434d0ba46750553b143b00eb996ef81ded45f4df4a30a5487c750`  
		Last Modified: Thu, 24 Mar 2022 23:13:17 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbb305818ad837064d616414049e197543cdffb0bc3c48046a7d3271b3e1b5e`  
		Last Modified: Thu, 24 Mar 2022 23:13:15 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6245bb06bb46ba0c35b7433234c72c1685ff5e9c938e0d498897b2c79951fd`  
		Last Modified: Thu, 24 Mar 2022 23:13:15 GMT  
		Size: 4.4 MB (4378824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b57640c9c7786162fe68c440e7fc35fa6a4f59dfc8b2c05ead4a85eb5a7e9f`  
		Last Modified: Thu, 24 Mar 2022 23:13:14 GMT  
		Size: 2.6 KB (2604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733dab4a1602b172f16690529dc18c051788f5403d52caff3703fae8c4ccdb37`  
		Last Modified: Thu, 24 Mar 2022 23:13:12 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb800e2c9b9dd594d7cc7e5b777e6b548a09d55234d2f3a547cf7a11f24ce2d`  
		Last Modified: Thu, 24 Mar 2022 23:13:19 GMT  
		Size: 53.4 MB (53429969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bf9d82ddd548e76ee83ba27fbbfd69d45f00aa73993e83f796c6b448d7f503`  
		Last Modified: Thu, 24 Mar 2022 23:13:12 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915025a8362d74e5f93a614dc592dc258a2dc0985cd6fb9d903a974ab0b823d1`  
		Last Modified: Thu, 24 Mar 2022 23:13:19 GMT  
		Size: 40.5 MB (40481181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9317ed1ad35f14a9b32b10227b398a129812dafd444475214d3ccf51c86d265d`  
		Last Modified: Thu, 24 Mar 2022 23:13:12 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.28`

```console
$ docker pull mysql@sha256:1c75ba7716c6f73fc106dacedfdcf13f934ea8c161c8b3b3e4618bcd5fbcf195
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.28` - linux; amd64

```console
$ docker pull mysql@sha256:8cdf596eb3fba84ae6d0ad683d330dcaf87ef8fb51e4d5dd9f1e289c5012e0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154597910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:667ee8fb158e365450fc3f09712208fe44e9f1364a9b130fed95f3f4862f8a63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Tue, 29 Mar 2022 18:08:41 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:08:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:08:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:08:56 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 29 Mar 2022 18:08:56 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:08:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:08:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:08:57 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:08:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6ea71d471d2d38ef59731ae2b31379ddd9163c4da92c1de543d8bd4f97fedf`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2920c795b25d6cd74b842f7329b94e1d7c5482885a3158589a6bc680c616fa4`  
		Last Modified: Tue, 29 Mar 2022 18:10:11 GMT  
		Size: 107.8 MB (107805075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c3bdf75ff5618cd6b7d60004bfb8cb8759026305eef07d986afa6e46454b15`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec1f1f78b0e9e0d09b58d1be3497429eb5c0f76f8dcf01371bcd6f9d019715d`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4607fa685ac65df86f44720e2b8a69e97f835483a5aa8fa139048e75e00f38ff`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.28-debian`

```console
$ docker pull mysql@sha256:1c75ba7716c6f73fc106dacedfdcf13f934ea8c161c8b3b3e4618bcd5fbcf195
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.28-debian` - linux; amd64

```console
$ docker pull mysql@sha256:8cdf596eb3fba84ae6d0ad683d330dcaf87ef8fb51e4d5dd9f1e289c5012e0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154597910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:667ee8fb158e365450fc3f09712208fe44e9f1364a9b130fed95f3f4862f8a63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Tue, 29 Mar 2022 18:08:41 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:08:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:08:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:08:56 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 29 Mar 2022 18:08:56 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:08:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:08:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:08:57 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:08:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6ea71d471d2d38ef59731ae2b31379ddd9163c4da92c1de543d8bd4f97fedf`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2920c795b25d6cd74b842f7329b94e1d7c5482885a3158589a6bc680c616fa4`  
		Last Modified: Tue, 29 Mar 2022 18:10:11 GMT  
		Size: 107.8 MB (107805075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c3bdf75ff5618cd6b7d60004bfb8cb8759026305eef07d986afa6e46454b15`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec1f1f78b0e9e0d09b58d1be3497429eb5c0f76f8dcf01371bcd6f9d019715d`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4607fa685ac65df86f44720e2b8a69e97f835483a5aa8fa139048e75e00f38ff`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.28-oracle`

```console
$ docker pull mysql@sha256:32054d8d010726bee26052cd4ac1b8d76db55180f6ac976e5fc6279190e896cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.28-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:e1866c1d0f58b69de7fa0b5986564ae044784f0dd1c61c01bbf3ec1470784312
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133139496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce4b41e88ebc537d8fe49c51d193e0d69307c49886cdad58a83ab738afe3522`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 22:26:17 GMT
ADD file:ebb4986af4fcca0d00738e77d2c814e70536c01a0e02eef98c71e9e3a56c0abd in / 
# Thu, 24 Mar 2022 22:26:18 GMT
CMD ["/bin/bash"]
# Fri, 25 Mar 2022 01:12:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 25 Mar 2022 01:12:38 GMT
ENV GOSU_VERSION=1.14
# Fri, 25 Mar 2022 01:12:41 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Mar 2022 01:13:00 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 25 Mar 2022 01:13:02 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 25 Mar 2022 01:13:02 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 25 Mar 2022 01:13:02 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Fri, 25 Mar 2022 01:13:02 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 25 Mar 2022 01:13:26 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Fri, 25 Mar 2022 01:13:27 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 25 Mar 2022 01:13:27 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Fri, 25 Mar 2022 01:13:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 25 Mar 2022 01:13:55 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Mar 2022 01:13:55 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 25 Mar 2022 01:13:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Mar 2022 01:13:55 GMT
EXPOSE 3306 33060
# Fri, 25 Mar 2022 01:13:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1de6f411eccf5041d90362d2d035abf0e59cf91dce4eacbc37ef0aa52f5b5920`  
		Last Modified: Thu, 24 Mar 2022 22:27:23 GMT  
		Size: 42.1 MB (42111629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7750893065cbe5478b40ebf1b3f4a424e4bff391ecfcd9355140adc25715de`  
		Last Modified: Fri, 25 Mar 2022 01:15:20 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf1e489f4aae4498fc2f96f3dbd32459bf28b5500980eb189896fe0781bbd39`  
		Last Modified: Fri, 25 Mar 2022 01:15:18 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a64bfd09b448f5ebe279c4b42eb6a98d6cd9b2a203c84e1e1179cc40d554c65`  
		Last Modified: Fri, 25 Mar 2022 01:15:18 GMT  
		Size: 4.5 MB (4547133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439534ad10016b75ec2760171452fdc19f522fcd321f4d9559aa98e93d090245`  
		Last Modified: Fri, 25 Mar 2022 01:15:18 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ba31e211ec3bc3f21d9e79ba88961da072db9951a42bf34f7f75575c2f22a2`  
		Last Modified: Fri, 25 Mar 2022 01:15:15 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb32dad74239c798b8edc0734070af95cc5fc2400f6c23e43204deaf27198ab`  
		Last Modified: Fri, 25 Mar 2022 01:15:23 GMT  
		Size: 47.3 MB (47267324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d728d0b568cbe11d3ec4a20552a005f259ef4db49c7aac61e6141248904912`  
		Last Modified: Fri, 25 Mar 2022 01:15:15 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d30611313f049519c61520bb7b8653a63d87f18bbe13d9ba96af57ed90a717a`  
		Last Modified: Fri, 25 Mar 2022 01:15:23 GMT  
		Size: 38.3 MB (38275082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829b3d97de2a870cc6f6976d671eea1e7818931e14c6e792bfa8c705ab0949a7`  
		Last Modified: Fri, 25 Mar 2022 01:15:15 GMT  
		Size: 5.1 KB (5140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.28-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c31271d3ea18ed5d8c8b2d255e675a8599801d571d58fee7b293cececcf1d1fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141175486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf5b46dfe3694e200010e9e0574770af8b1a7d2d1ef9e6ae7b664578f048b10e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 22:21:09 GMT
ADD file:1eaca9dccdbe88c4fac0b484a625100443af30879cf6cba7b5615db77745b0c7 in / 
# Thu, 24 Mar 2022 22:21:10 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 23:11:19 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 24 Mar 2022 23:11:20 GMT
ENV GOSU_VERSION=1.14
# Thu, 24 Mar 2022 23:11:23 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 24 Mar 2022 23:11:43 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 24 Mar 2022 23:11:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 24 Mar 2022 23:11:46 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 24 Mar 2022 23:11:47 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 23:11:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 24 Mar 2022 23:12:12 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 24 Mar 2022 23:12:12 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 24 Mar 2022 23:12:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 23:12:37 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 24 Mar 2022 23:12:38 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Mar 2022 23:12:40 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Thu, 24 Mar 2022 23:12:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 23:12:41 GMT
EXPOSE 3306 33060
# Thu, 24 Mar 2022 23:12:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c11319b13f376dfb3fa1ee22d0047cfb7157eba4ba2786653cb29ac6defcb93c`  
		Last Modified: Thu, 24 Mar 2022 22:22:26 GMT  
		Size: 42.0 MB (42018948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba57e28a536434d0ba46750553b143b00eb996ef81ded45f4df4a30a5487c750`  
		Last Modified: Thu, 24 Mar 2022 23:13:17 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbb305818ad837064d616414049e197543cdffb0bc3c48046a7d3271b3e1b5e`  
		Last Modified: Thu, 24 Mar 2022 23:13:15 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6245bb06bb46ba0c35b7433234c72c1685ff5e9c938e0d498897b2c79951fd`  
		Last Modified: Thu, 24 Mar 2022 23:13:15 GMT  
		Size: 4.4 MB (4378824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b57640c9c7786162fe68c440e7fc35fa6a4f59dfc8b2c05ead4a85eb5a7e9f`  
		Last Modified: Thu, 24 Mar 2022 23:13:14 GMT  
		Size: 2.6 KB (2604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733dab4a1602b172f16690529dc18c051788f5403d52caff3703fae8c4ccdb37`  
		Last Modified: Thu, 24 Mar 2022 23:13:12 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb800e2c9b9dd594d7cc7e5b777e6b548a09d55234d2f3a547cf7a11f24ce2d`  
		Last Modified: Thu, 24 Mar 2022 23:13:19 GMT  
		Size: 53.4 MB (53429969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bf9d82ddd548e76ee83ba27fbbfd69d45f00aa73993e83f796c6b448d7f503`  
		Last Modified: Thu, 24 Mar 2022 23:13:12 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915025a8362d74e5f93a614dc592dc258a2dc0985cd6fb9d903a974ab0b823d1`  
		Last Modified: Thu, 24 Mar 2022 23:13:19 GMT  
		Size: 40.5 MB (40481181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9317ed1ad35f14a9b32b10227b398a129812dafd444475214d3ccf51c86d265d`  
		Last Modified: Thu, 24 Mar 2022 23:13:12 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:1c75ba7716c6f73fc106dacedfdcf13f934ea8c161c8b3b3e4618bcd5fbcf195
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:8cdf596eb3fba84ae6d0ad683d330dcaf87ef8fb51e4d5dd9f1e289c5012e0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154597910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:667ee8fb158e365450fc3f09712208fe44e9f1364a9b130fed95f3f4862f8a63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Tue, 29 Mar 2022 18:08:41 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:08:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:08:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:08:56 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 29 Mar 2022 18:08:56 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:08:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:08:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:08:57 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:08:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6ea71d471d2d38ef59731ae2b31379ddd9163c4da92c1de543d8bd4f97fedf`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2920c795b25d6cd74b842f7329b94e1d7c5482885a3158589a6bc680c616fa4`  
		Last Modified: Tue, 29 Mar 2022 18:10:11 GMT  
		Size: 107.8 MB (107805075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c3bdf75ff5618cd6b7d60004bfb8cb8759026305eef07d986afa6e46454b15`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec1f1f78b0e9e0d09b58d1be3497429eb5c0f76f8dcf01371bcd6f9d019715d`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4607fa685ac65df86f44720e2b8a69e97f835483a5aa8fa139048e75e00f38ff`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:1c75ba7716c6f73fc106dacedfdcf13f934ea8c161c8b3b3e4618bcd5fbcf195
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:8cdf596eb3fba84ae6d0ad683d330dcaf87ef8fb51e4d5dd9f1e289c5012e0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154597910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:667ee8fb158e365450fc3f09712208fe44e9f1364a9b130fed95f3f4862f8a63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:08:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 29 Mar 2022 18:08:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:23 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 18:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 18:08:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 18:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:08:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 29 Mar 2022 18:08:41 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Tue, 29 Mar 2022 18:08:41 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 29 Mar 2022 18:08:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 29 Mar 2022 18:08:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 29 Mar 2022 18:08:56 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 29 Mar 2022 18:08:56 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 29 Mar 2022 18:08:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 29 Mar 2022 18:08:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 18:08:57 GMT
EXPOSE 3306 33060
# Tue, 29 Mar 2022 18:08:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d94f01a09f657ba243e4c8f06dbcbe240baef4b02efa609d46fdf756f72cf9`  
		Last Modified: Tue, 29 Mar 2022 18:09:59 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d78aaa607875868b6ee3f3dac65bd3a1ced4a7a729e4fbe4a34c7a81b0d7fd`  
		Last Modified: Tue, 29 Mar 2022 18:10:01 GMT  
		Size: 4.2 MB (4179292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f91ffbdf6994a684bb27d6176dfed4065bccada5fe7aab65b4c2acf929d920`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 1.4 MB (1386619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee9e07e12fda8ed0999986a1cefb4ed81a233efb1120482400725fa3ca8953`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d82978082c5d3754f3becf6f7c5aae231ec9363c614e8aaab16480f2f0ea44`  
		Last Modified: Tue, 29 Mar 2022 18:10:00 GMT  
		Size: 14.1 MB (14064167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f46ebb971aaebfddac2122217ba259071b776b9637eecce63a6965bf1cbcf5`  
		Last Modified: Tue, 29 Mar 2022 18:09:57 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6ea71d471d2d38ef59731ae2b31379ddd9163c4da92c1de543d8bd4f97fedf`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2920c795b25d6cd74b842f7329b94e1d7c5482885a3158589a6bc680c616fa4`  
		Last Modified: Tue, 29 Mar 2022 18:10:11 GMT  
		Size: 107.8 MB (107805075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c3bdf75ff5618cd6b7d60004bfb8cb8759026305eef07d986afa6e46454b15`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec1f1f78b0e9e0d09b58d1be3497429eb5c0f76f8dcf01371bcd6f9d019715d`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 5.1 KB (5136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4607fa685ac65df86f44720e2b8a69e97f835483a5aa8fa139048e75e00f38ff`  
		Last Modified: Tue, 29 Mar 2022 18:09:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:32054d8d010726bee26052cd4ac1b8d76db55180f6ac976e5fc6279190e896cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:e1866c1d0f58b69de7fa0b5986564ae044784f0dd1c61c01bbf3ec1470784312
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133139496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce4b41e88ebc537d8fe49c51d193e0d69307c49886cdad58a83ab738afe3522`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 22:26:17 GMT
ADD file:ebb4986af4fcca0d00738e77d2c814e70536c01a0e02eef98c71e9e3a56c0abd in / 
# Thu, 24 Mar 2022 22:26:18 GMT
CMD ["/bin/bash"]
# Fri, 25 Mar 2022 01:12:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 25 Mar 2022 01:12:38 GMT
ENV GOSU_VERSION=1.14
# Fri, 25 Mar 2022 01:12:41 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Mar 2022 01:13:00 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 25 Mar 2022 01:13:02 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 25 Mar 2022 01:13:02 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 25 Mar 2022 01:13:02 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Fri, 25 Mar 2022 01:13:02 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 25 Mar 2022 01:13:26 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Fri, 25 Mar 2022 01:13:27 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 25 Mar 2022 01:13:27 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Fri, 25 Mar 2022 01:13:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 25 Mar 2022 01:13:55 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Mar 2022 01:13:55 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 25 Mar 2022 01:13:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Mar 2022 01:13:55 GMT
EXPOSE 3306 33060
# Fri, 25 Mar 2022 01:13:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1de6f411eccf5041d90362d2d035abf0e59cf91dce4eacbc37ef0aa52f5b5920`  
		Last Modified: Thu, 24 Mar 2022 22:27:23 GMT  
		Size: 42.1 MB (42111629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7750893065cbe5478b40ebf1b3f4a424e4bff391ecfcd9355140adc25715de`  
		Last Modified: Fri, 25 Mar 2022 01:15:20 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf1e489f4aae4498fc2f96f3dbd32459bf28b5500980eb189896fe0781bbd39`  
		Last Modified: Fri, 25 Mar 2022 01:15:18 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a64bfd09b448f5ebe279c4b42eb6a98d6cd9b2a203c84e1e1179cc40d554c65`  
		Last Modified: Fri, 25 Mar 2022 01:15:18 GMT  
		Size: 4.5 MB (4547133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439534ad10016b75ec2760171452fdc19f522fcd321f4d9559aa98e93d090245`  
		Last Modified: Fri, 25 Mar 2022 01:15:18 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ba31e211ec3bc3f21d9e79ba88961da072db9951a42bf34f7f75575c2f22a2`  
		Last Modified: Fri, 25 Mar 2022 01:15:15 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb32dad74239c798b8edc0734070af95cc5fc2400f6c23e43204deaf27198ab`  
		Last Modified: Fri, 25 Mar 2022 01:15:23 GMT  
		Size: 47.3 MB (47267324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d728d0b568cbe11d3ec4a20552a005f259ef4db49c7aac61e6141248904912`  
		Last Modified: Fri, 25 Mar 2022 01:15:15 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d30611313f049519c61520bb7b8653a63d87f18bbe13d9ba96af57ed90a717a`  
		Last Modified: Fri, 25 Mar 2022 01:15:23 GMT  
		Size: 38.3 MB (38275082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829b3d97de2a870cc6f6976d671eea1e7818931e14c6e792bfa8c705ab0949a7`  
		Last Modified: Fri, 25 Mar 2022 01:15:15 GMT  
		Size: 5.1 KB (5140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c31271d3ea18ed5d8c8b2d255e675a8599801d571d58fee7b293cececcf1d1fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141175486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf5b46dfe3694e200010e9e0574770af8b1a7d2d1ef9e6ae7b664578f048b10e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 22:21:09 GMT
ADD file:1eaca9dccdbe88c4fac0b484a625100443af30879cf6cba7b5615db77745b0c7 in / 
# Thu, 24 Mar 2022 22:21:10 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 23:11:19 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 24 Mar 2022 23:11:20 GMT
ENV GOSU_VERSION=1.14
# Thu, 24 Mar 2022 23:11:23 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 24 Mar 2022 23:11:43 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 24 Mar 2022 23:11:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 24 Mar 2022 23:11:46 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 24 Mar 2022 23:11:47 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 23:11:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 24 Mar 2022 23:12:12 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 24 Mar 2022 23:12:12 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 24 Mar 2022 23:12:13 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 23:12:37 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 24 Mar 2022 23:12:38 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Mar 2022 23:12:40 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Thu, 24 Mar 2022 23:12:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 23:12:41 GMT
EXPOSE 3306 33060
# Thu, 24 Mar 2022 23:12:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c11319b13f376dfb3fa1ee22d0047cfb7157eba4ba2786653cb29ac6defcb93c`  
		Last Modified: Thu, 24 Mar 2022 22:22:26 GMT  
		Size: 42.0 MB (42018948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba57e28a536434d0ba46750553b143b00eb996ef81ded45f4df4a30a5487c750`  
		Last Modified: Thu, 24 Mar 2022 23:13:17 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbb305818ad837064d616414049e197543cdffb0bc3c48046a7d3271b3e1b5e`  
		Last Modified: Thu, 24 Mar 2022 23:13:15 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6245bb06bb46ba0c35b7433234c72c1685ff5e9c938e0d498897b2c79951fd`  
		Last Modified: Thu, 24 Mar 2022 23:13:15 GMT  
		Size: 4.4 MB (4378824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b57640c9c7786162fe68c440e7fc35fa6a4f59dfc8b2c05ead4a85eb5a7e9f`  
		Last Modified: Thu, 24 Mar 2022 23:13:14 GMT  
		Size: 2.6 KB (2604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733dab4a1602b172f16690529dc18c051788f5403d52caff3703fae8c4ccdb37`  
		Last Modified: Thu, 24 Mar 2022 23:13:12 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb800e2c9b9dd594d7cc7e5b777e6b548a09d55234d2f3a547cf7a11f24ce2d`  
		Last Modified: Thu, 24 Mar 2022 23:13:19 GMT  
		Size: 53.4 MB (53429969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bf9d82ddd548e76ee83ba27fbbfd69d45f00aa73993e83f796c6b448d7f503`  
		Last Modified: Thu, 24 Mar 2022 23:13:12 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915025a8362d74e5f93a614dc592dc258a2dc0985cd6fb9d903a974ab0b823d1`  
		Last Modified: Thu, 24 Mar 2022 23:13:19 GMT  
		Size: 40.5 MB (40481181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9317ed1ad35f14a9b32b10227b398a129812dafd444475214d3ccf51c86d265d`  
		Last Modified: Thu, 24 Mar 2022 23:13:12 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
