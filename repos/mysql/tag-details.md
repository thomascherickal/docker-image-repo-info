<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5-debian`](#mysql5-debian)
-	[`mysql:5-oracle`](#mysql5-oracle)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7-debian`](#mysql57-debian)
-	[`mysql:5.7-oracle`](#mysql57-oracle)
-	[`mysql:5.7.38`](#mysql5738)
-	[`mysql:5.7.38-debian`](#mysql5738-debian)
-	[`mysql:5.7.38-oracle`](#mysql5738-oracle)
-	[`mysql:8`](#mysql8)
-	[`mysql:8-debian`](#mysql8-debian)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0.29`](#mysql8029)
-	[`mysql:8.0.29-debian`](#mysql8029-debian)
-	[`mysql:8.0.29-oracle`](#mysql8029-oracle)
-	[`mysql:debian`](#mysqldebian)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)

## `mysql:5`

```console
$ docker pull mysql@sha256:8b4b41d530c40d77a3205c53f7ecf1026d735648d9a09777845f305953e5eff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:e73f0d1cb2e042d4b93fcd4a301c147cbc0a28e982c0e965901162a733991df6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162479495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa50097efbdef5884e5ebaba4da5899e79609b78cd4fe91b365d5d9d3205188`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:23:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 28 Jun 2022 00:23:07 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Tue, 28 Jun 2022 00:23:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:23:26 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:23:26 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:23:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:23:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:23:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:23:27 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:23:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09914736f6f7304f95bac6a69ac7c684924e69e590068525ba1e3bcf61c6202c`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c835958ed8cedc7d60d07e83078b5dfa1b9b573b8e18cdc693feec0d92b591`  
		Last Modified: Tue, 28 Jun 2022 00:25:40 GMT  
		Size: 115.7 MB (115676518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa6834c9208751015a2687822d5a5142bfd1b52ce353eb0030ed8c45bc25662`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3b0798493943a172317b25ea1bc22652422af88c2954947e1e3342edcac2d`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:8b4b41d530c40d77a3205c53f7ecf1026d735648d9a09777845f305953e5eff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:e73f0d1cb2e042d4b93fcd4a301c147cbc0a28e982c0e965901162a733991df6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162479495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa50097efbdef5884e5ebaba4da5899e79609b78cd4fe91b365d5d9d3205188`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:23:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 28 Jun 2022 00:23:07 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Tue, 28 Jun 2022 00:23:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:23:26 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:23:26 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:23:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:23:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:23:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:23:27 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:23:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09914736f6f7304f95bac6a69ac7c684924e69e590068525ba1e3bcf61c6202c`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c835958ed8cedc7d60d07e83078b5dfa1b9b573b8e18cdc693feec0d92b591`  
		Last Modified: Tue, 28 Jun 2022 00:25:40 GMT  
		Size: 115.7 MB (115676518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa6834c9208751015a2687822d5a5142bfd1b52ce353eb0030ed8c45bc25662`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3b0798493943a172317b25ea1bc22652422af88c2954947e1e3342edcac2d`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:64ef2a07763f7f7ec4e1acbac84d5dbdda5b4bf468194aaa5caa9bf4bf370a75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:8b70e11f0a1d0d3018bf6ca3846d872e4e68c699cdf2dc25b46049327386db1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127806404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5958a947375b1e5db8071ec2f5332b72526229a8a0699d64078c3f7baf60687b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Jun 2022 01:20:22 GMT
ADD file:5e615d6d49ec50cba937fa86f5fb7d6a4a7e680b2b4f5b659e879b95304c0417 in / 
# Thu, 16 Jun 2022 01:20:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Jun 2022 01:38:41 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 16 Jun 2022 01:38:41 GMT
ENV GOSU_VERSION=1.14
# Thu, 16 Jun 2022 01:38:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Jun 2022 00:22:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Tue, 28 Jun 2022 00:22:16 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:22:16 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 28 Jun 2022 00:22:16 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Tue, 28 Jun 2022 00:22:17 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 28 Jun 2022 00:22:34 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 28 Jun 2022 00:22:35 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 28 Jun 2022 00:22:35 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Tue, 28 Jun 2022 00:22:56 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 28 Jun 2022 00:22:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:22:56 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:22:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:22:57 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:22:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:63183c9b4598e16c4cef95f706d50ff6c928de41f391cd513495b27eaa27bf89`  
		Last Modified: Thu, 16 Jun 2022 01:21:08 GMT  
		Size: 48.8 MB (48757931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921fb508f1d1aecc5558b119c43c60ca99e2803d417ea98b5a55f94975ac5440`  
		Last Modified: Thu, 16 Jun 2022 01:40:10 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c722a284ecb6bbcc3803b2a9fb3df9e58ebd491e421507db7c73d8f4255cf0f4`  
		Last Modified: Thu, 16 Jun 2022 01:40:09 GMT  
		Size: 930.2 KB (930225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e2862fad6e07e82b31bcad70ede98d8fda30c834740a571945313fbb06c086`  
		Last Modified: Tue, 28 Jun 2022 00:25:07 GMT  
		Size: 4.5 MB (4545079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa0403847e0144a5edf870bb60a1c2ca163adcbec7f37754825f101361ed34b`  
		Last Modified: Tue, 28 Jun 2022 00:25:06 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e220d9807c0bd3630bf3d8257814277de6620028f9769b8a0936e8e41d9177`  
		Last Modified: Tue, 28 Jun 2022 00:25:03 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bf024001e30ab8d7eef404acdf647bd35eea8ba5dfc013f809f664595e3aeb`  
		Last Modified: Tue, 28 Jun 2022 00:25:07 GMT  
		Size: 25.5 MB (25481000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a565f071b7651737bb567cf6f527aa8d30e5acb1f050e1c1744bba9b5aa825`  
		Last Modified: Tue, 28 Jun 2022 00:25:04 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbcac0569bb6d8155444f4dd08484dd7ef1ed644e3f69d80c0fa9018d18ed0e`  
		Last Modified: Tue, 28 Jun 2022 00:25:12 GMT  
		Size: 48.1 MB (48082637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def88f6fdde385c164a91c0e22b6c4c4ef9d6c8d38ca8e53c39079e6b0915b38`  
		Last Modified: Tue, 28 Jun 2022 00:25:03 GMT  
		Size: 5.2 KB (5161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:8b4b41d530c40d77a3205c53f7ecf1026d735648d9a09777845f305953e5eff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:e73f0d1cb2e042d4b93fcd4a301c147cbc0a28e982c0e965901162a733991df6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162479495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa50097efbdef5884e5ebaba4da5899e79609b78cd4fe91b365d5d9d3205188`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:23:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 28 Jun 2022 00:23:07 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Tue, 28 Jun 2022 00:23:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:23:26 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:23:26 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:23:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:23:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:23:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:23:27 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:23:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09914736f6f7304f95bac6a69ac7c684924e69e590068525ba1e3bcf61c6202c`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c835958ed8cedc7d60d07e83078b5dfa1b9b573b8e18cdc693feec0d92b591`  
		Last Modified: Tue, 28 Jun 2022 00:25:40 GMT  
		Size: 115.7 MB (115676518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa6834c9208751015a2687822d5a5142bfd1b52ce353eb0030ed8c45bc25662`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3b0798493943a172317b25ea1bc22652422af88c2954947e1e3342edcac2d`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:8b4b41d530c40d77a3205c53f7ecf1026d735648d9a09777845f305953e5eff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:e73f0d1cb2e042d4b93fcd4a301c147cbc0a28e982c0e965901162a733991df6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162479495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa50097efbdef5884e5ebaba4da5899e79609b78cd4fe91b365d5d9d3205188`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:23:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 28 Jun 2022 00:23:07 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Tue, 28 Jun 2022 00:23:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:23:26 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:23:26 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:23:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:23:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:23:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:23:27 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:23:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09914736f6f7304f95bac6a69ac7c684924e69e590068525ba1e3bcf61c6202c`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c835958ed8cedc7d60d07e83078b5dfa1b9b573b8e18cdc693feec0d92b591`  
		Last Modified: Tue, 28 Jun 2022 00:25:40 GMT  
		Size: 115.7 MB (115676518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa6834c9208751015a2687822d5a5142bfd1b52ce353eb0030ed8c45bc25662`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3b0798493943a172317b25ea1bc22652422af88c2954947e1e3342edcac2d`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:64ef2a07763f7f7ec4e1acbac84d5dbdda5b4bf468194aaa5caa9bf4bf370a75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:8b70e11f0a1d0d3018bf6ca3846d872e4e68c699cdf2dc25b46049327386db1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127806404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5958a947375b1e5db8071ec2f5332b72526229a8a0699d64078c3f7baf60687b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Jun 2022 01:20:22 GMT
ADD file:5e615d6d49ec50cba937fa86f5fb7d6a4a7e680b2b4f5b659e879b95304c0417 in / 
# Thu, 16 Jun 2022 01:20:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Jun 2022 01:38:41 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 16 Jun 2022 01:38:41 GMT
ENV GOSU_VERSION=1.14
# Thu, 16 Jun 2022 01:38:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Jun 2022 00:22:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Tue, 28 Jun 2022 00:22:16 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:22:16 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 28 Jun 2022 00:22:16 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Tue, 28 Jun 2022 00:22:17 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 28 Jun 2022 00:22:34 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 28 Jun 2022 00:22:35 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 28 Jun 2022 00:22:35 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Tue, 28 Jun 2022 00:22:56 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 28 Jun 2022 00:22:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:22:56 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:22:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:22:57 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:22:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:63183c9b4598e16c4cef95f706d50ff6c928de41f391cd513495b27eaa27bf89`  
		Last Modified: Thu, 16 Jun 2022 01:21:08 GMT  
		Size: 48.8 MB (48757931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921fb508f1d1aecc5558b119c43c60ca99e2803d417ea98b5a55f94975ac5440`  
		Last Modified: Thu, 16 Jun 2022 01:40:10 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c722a284ecb6bbcc3803b2a9fb3df9e58ebd491e421507db7c73d8f4255cf0f4`  
		Last Modified: Thu, 16 Jun 2022 01:40:09 GMT  
		Size: 930.2 KB (930225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e2862fad6e07e82b31bcad70ede98d8fda30c834740a571945313fbb06c086`  
		Last Modified: Tue, 28 Jun 2022 00:25:07 GMT  
		Size: 4.5 MB (4545079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa0403847e0144a5edf870bb60a1c2ca163adcbec7f37754825f101361ed34b`  
		Last Modified: Tue, 28 Jun 2022 00:25:06 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e220d9807c0bd3630bf3d8257814277de6620028f9769b8a0936e8e41d9177`  
		Last Modified: Tue, 28 Jun 2022 00:25:03 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bf024001e30ab8d7eef404acdf647bd35eea8ba5dfc013f809f664595e3aeb`  
		Last Modified: Tue, 28 Jun 2022 00:25:07 GMT  
		Size: 25.5 MB (25481000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a565f071b7651737bb567cf6f527aa8d30e5acb1f050e1c1744bba9b5aa825`  
		Last Modified: Tue, 28 Jun 2022 00:25:04 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbcac0569bb6d8155444f4dd08484dd7ef1ed644e3f69d80c0fa9018d18ed0e`  
		Last Modified: Tue, 28 Jun 2022 00:25:12 GMT  
		Size: 48.1 MB (48082637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def88f6fdde385c164a91c0e22b6c4c4ef9d6c8d38ca8e53c39079e6b0915b38`  
		Last Modified: Tue, 28 Jun 2022 00:25:03 GMT  
		Size: 5.2 KB (5161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.38`

```console
$ docker pull mysql@sha256:8b4b41d530c40d77a3205c53f7ecf1026d735648d9a09777845f305953e5eff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.38` - linux; amd64

```console
$ docker pull mysql@sha256:e73f0d1cb2e042d4b93fcd4a301c147cbc0a28e982c0e965901162a733991df6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162479495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa50097efbdef5884e5ebaba4da5899e79609b78cd4fe91b365d5d9d3205188`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:23:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 28 Jun 2022 00:23:07 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Tue, 28 Jun 2022 00:23:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:23:26 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:23:26 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:23:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:23:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:23:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:23:27 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:23:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09914736f6f7304f95bac6a69ac7c684924e69e590068525ba1e3bcf61c6202c`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c835958ed8cedc7d60d07e83078b5dfa1b9b573b8e18cdc693feec0d92b591`  
		Last Modified: Tue, 28 Jun 2022 00:25:40 GMT  
		Size: 115.7 MB (115676518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa6834c9208751015a2687822d5a5142bfd1b52ce353eb0030ed8c45bc25662`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3b0798493943a172317b25ea1bc22652422af88c2954947e1e3342edcac2d`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.38-debian`

```console
$ docker pull mysql@sha256:8b4b41d530c40d77a3205c53f7ecf1026d735648d9a09777845f305953e5eff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.38-debian` - linux; amd64

```console
$ docker pull mysql@sha256:e73f0d1cb2e042d4b93fcd4a301c147cbc0a28e982c0e965901162a733991df6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162479495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efa50097efbdef5884e5ebaba4da5899e79609b78cd4fe91b365d5d9d3205188`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:23:07 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 28 Jun 2022 00:23:07 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Tue, 28 Jun 2022 00:23:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:23:26 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:23:26 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:23:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:23:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:23:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:23:27 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:23:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09914736f6f7304f95bac6a69ac7c684924e69e590068525ba1e3bcf61c6202c`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c835958ed8cedc7d60d07e83078b5dfa1b9b573b8e18cdc693feec0d92b591`  
		Last Modified: Tue, 28 Jun 2022 00:25:40 GMT  
		Size: 115.7 MB (115676518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa6834c9208751015a2687822d5a5142bfd1b52ce353eb0030ed8c45bc25662`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3b0798493943a172317b25ea1bc22652422af88c2954947e1e3342edcac2d`  
		Last Modified: Tue, 28 Jun 2022 00:25:25 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.38-oracle`

```console
$ docker pull mysql@sha256:64ef2a07763f7f7ec4e1acbac84d5dbdda5b4bf468194aaa5caa9bf4bf370a75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.38-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:8b70e11f0a1d0d3018bf6ca3846d872e4e68c699cdf2dc25b46049327386db1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127806404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5958a947375b1e5db8071ec2f5332b72526229a8a0699d64078c3f7baf60687b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Jun 2022 01:20:22 GMT
ADD file:5e615d6d49ec50cba937fa86f5fb7d6a4a7e680b2b4f5b659e879b95304c0417 in / 
# Thu, 16 Jun 2022 01:20:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Jun 2022 01:38:41 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 16 Jun 2022 01:38:41 GMT
ENV GOSU_VERSION=1.14
# Thu, 16 Jun 2022 01:38:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Jun 2022 00:22:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Tue, 28 Jun 2022 00:22:16 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:22:16 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 28 Jun 2022 00:22:16 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Tue, 28 Jun 2022 00:22:17 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 28 Jun 2022 00:22:34 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 28 Jun 2022 00:22:35 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 28 Jun 2022 00:22:35 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Tue, 28 Jun 2022 00:22:56 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 28 Jun 2022 00:22:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:22:56 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:22:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:22:57 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:22:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:63183c9b4598e16c4cef95f706d50ff6c928de41f391cd513495b27eaa27bf89`  
		Last Modified: Thu, 16 Jun 2022 01:21:08 GMT  
		Size: 48.8 MB (48757931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921fb508f1d1aecc5558b119c43c60ca99e2803d417ea98b5a55f94975ac5440`  
		Last Modified: Thu, 16 Jun 2022 01:40:10 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c722a284ecb6bbcc3803b2a9fb3df9e58ebd491e421507db7c73d8f4255cf0f4`  
		Last Modified: Thu, 16 Jun 2022 01:40:09 GMT  
		Size: 930.2 KB (930225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e2862fad6e07e82b31bcad70ede98d8fda30c834740a571945313fbb06c086`  
		Last Modified: Tue, 28 Jun 2022 00:25:07 GMT  
		Size: 4.5 MB (4545079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa0403847e0144a5edf870bb60a1c2ca163adcbec7f37754825f101361ed34b`  
		Last Modified: Tue, 28 Jun 2022 00:25:06 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e220d9807c0bd3630bf3d8257814277de6620028f9769b8a0936e8e41d9177`  
		Last Modified: Tue, 28 Jun 2022 00:25:03 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bf024001e30ab8d7eef404acdf647bd35eea8ba5dfc013f809f664595e3aeb`  
		Last Modified: Tue, 28 Jun 2022 00:25:07 GMT  
		Size: 25.5 MB (25481000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a565f071b7651737bb567cf6f527aa8d30e5acb1f050e1c1744bba9b5aa825`  
		Last Modified: Tue, 28 Jun 2022 00:25:04 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbcac0569bb6d8155444f4dd08484dd7ef1ed644e3f69d80c0fa9018d18ed0e`  
		Last Modified: Tue, 28 Jun 2022 00:25:12 GMT  
		Size: 48.1 MB (48082637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def88f6fdde385c164a91c0e22b6c4c4ef9d6c8d38ca8e53c39079e6b0915b38`  
		Last Modified: Tue, 28 Jun 2022 00:25:03 GMT  
		Size: 5.2 KB (5161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:a840244706a5fdc3c704b15a3700bfda39fdc069262d7753fa09de2d9faf5f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:b2d83fc6fbd16d59db1adc8d2e81a65663148b243bb36c6dc645f3c6468dc284
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155908369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef9083d9892db139e2b7c81fd133836e7aa32db2b5f1d5702e2593100fa1417`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Tue, 28 Jun 2022 00:21:38 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:21:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:21:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:21:53 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 28 Jun 2022 00:21:53 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:21:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:21:54 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:21:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6b647ddb19a4d8418c24e6de80b121ac50563fc8c2d90f0b59dbb619c9507`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09ca0f0cb24ca059efd9c31d1802ff067f77165a930b3ba53b1d3ff9833b18d`  
		Last Modified: Tue, 28 Jun 2022 00:24:35 GMT  
		Size: 109.1 MB (109104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e223e3cd2fdb62988d08fe4dfdc8a8a3ca0916a0c151f9ce2bb463a8033ce0a`  
		Last Modified: Tue, 28 Jun 2022 00:24:17 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b038d826c6572e26b8ef0a0bc128710feb4dd940bc174c570be426a67a57fff`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33ac6052fc913fd126296376ceeb69c617236fa33d820a02b8744148615f543`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:a840244706a5fdc3c704b15a3700bfda39fdc069262d7753fa09de2d9faf5f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:b2d83fc6fbd16d59db1adc8d2e81a65663148b243bb36c6dc645f3c6468dc284
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155908369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef9083d9892db139e2b7c81fd133836e7aa32db2b5f1d5702e2593100fa1417`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Tue, 28 Jun 2022 00:21:38 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:21:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:21:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:21:53 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 28 Jun 2022 00:21:53 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:21:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:21:54 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:21:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6b647ddb19a4d8418c24e6de80b121ac50563fc8c2d90f0b59dbb619c9507`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09ca0f0cb24ca059efd9c31d1802ff067f77165a930b3ba53b1d3ff9833b18d`  
		Last Modified: Tue, 28 Jun 2022 00:24:35 GMT  
		Size: 109.1 MB (109104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e223e3cd2fdb62988d08fe4dfdc8a8a3ca0916a0c151f9ce2bb463a8033ce0a`  
		Last Modified: Tue, 28 Jun 2022 00:24:17 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b038d826c6572e26b8ef0a0bc128710feb4dd940bc174c570be426a67a57fff`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33ac6052fc913fd126296376ceeb69c617236fa33d820a02b8744148615f543`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:a3db7b0ac138588506dbcb958bbfa4a3a71da227fb1410b6c8ba86e5a0632f88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:a695fb7643f3b28bb720670c8557e946fb0df0bed6f118cecb61b46ef353ce46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131788232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab8fad28a2df8c23829d482831a1a913823340b7de88e6452855ff042b662093`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:23:26 GMT
ADD file:837f6c6e7e20067b92edb72e78a8399e6cbbd72dab23db7b5b5a301c58d2a0de in / 
# Tue, 14 Jun 2022 18:23:26 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 18:39:39 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 18:39:39 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 18:39:43 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Jun 2022 00:20:13 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 28 Jun 2022 00:20:15 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:20:15 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 28 Jun 2022 00:20:15 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 28 Jun 2022 00:20:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 28 Jun 2022 00:20:42 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 28 Jun 2022 00:20:43 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 28 Jun 2022 00:20:43 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 28 Jun 2022 00:21:14 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 28 Jun 2022 00:21:14 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:21:14 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:21:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:21:15 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:21:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5f160c0f6cac587a73883b48a8857f5cce0930112792cef25c62510e256e93dc`  
		Last Modified: Tue, 14 Jun 2022 18:24:18 GMT  
		Size: 39.2 MB (39219730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86c3d841d1984f858257755bdf734554725af4f926f3b1d1b22f119cce8bda9`  
		Last Modified: Tue, 14 Jun 2022 18:41:49 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f026b3ec1ed102cfe531d812e2063669bad08ac3a0ac68a31e44083d9b9a5f5d`  
		Last Modified: Tue, 14 Jun 2022 18:41:47 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478636a5486e48bba38a3fa287f3b8ac0f9475d0a3fa2d12fa93b380345be6bf`  
		Last Modified: Tue, 28 Jun 2022 00:23:57 GMT  
		Size: 4.6 MB (4584099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b941aa3584d8a0c760fdd99040fee760b2847d93819a44dd2bfb396fd7c04d9`  
		Last Modified: Tue, 28 Jun 2022 00:23:57 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebddb2e985f2fd2f75055ad472eb725ae21b4c841e7fbc28384250ff79b1b15`  
		Last Modified: Tue, 28 Jun 2022 00:23:54 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a2abf961ad5794642b9911e32bfcc6a56c27ae26596ae3cb1ae8bafdc200f9`  
		Last Modified: Tue, 28 Jun 2022 00:24:02 GMT  
		Size: 47.3 MB (47257530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215106930b414b865a2703a23e7428c641bb28d7250b3d520938fca7e7daa217`  
		Last Modified: Tue, 28 Jun 2022 00:23:54 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0746f4080775920510cf00ee4853ff6c24db6c4707f4817f89af986192d99695`  
		Last Modified: Tue, 28 Jun 2022 00:24:02 GMT  
		Size: 39.8 MB (39788521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1195705edd352cba35d5fd3544b781c31a5081fa3bdece1936be2cea886506f6`  
		Last Modified: Tue, 28 Jun 2022 00:23:54 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:0418232b74414d7e223da6fc26f47d9498abd72b4ca3bb1cd826f8f05ea55374
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138660393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a0eef221ccdafeb4649e0af86a16d1bf826ed66807fd64248a212871c04c2a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:41:36 GMT
ADD file:4a6ee90ad73353bfb87b2f121e06bddaed6104536e485baa83fadbe7facc774c in / 
# Tue, 14 Jun 2022 18:41:37 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 19:17:17 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 19:17:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 19:17:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 27 Jun 2022 23:40:26 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Mon, 27 Jun 2022 23:40:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Mon, 27 Jun 2022 23:40:28 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 27 Jun 2022 23:40:29 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Mon, 27 Jun 2022 23:40:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 27 Jun 2022 23:40:56 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Mon, 27 Jun 2022 23:40:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 27 Jun 2022 23:40:57 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Mon, 27 Jun 2022 23:41:27 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 27 Jun 2022 23:41:27 GMT
VOLUME [/var/lib/mysql]
# Mon, 27 Jun 2022 23:41:29 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Mon, 27 Jun 2022 23:41:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Jun 2022 23:41:30 GMT
EXPOSE 3306 33060
# Mon, 27 Jun 2022 23:41:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2bbc1bf883bd601c0da5735b538963308bcc17f90d36525ecc93456ffad79064`  
		Last Modified: Tue, 14 Jun 2022 18:42:39 GMT  
		Size: 38.0 MB (38012371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428f9d18fc319262a774f75a5849d4819b5b44cbf07fbb5e3c262e5cf30c22d`  
		Last Modified: Tue, 14 Jun 2022 19:19:14 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cba94044003680a99c76f187ea817c71b843de38bb7f28faf8ca6508efd45e`  
		Last Modified: Tue, 14 Jun 2022 19:19:12 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac1107eaf64ada9002dc0dbf73e0a8b8c2a3e2dfe557a59ee79ae5296dd6d35`  
		Last Modified: Mon, 27 Jun 2022 23:41:57 GMT  
		Size: 4.4 MB (4400369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287b497aedf9bf453ca624e6f7b036489fa7091918b209ff279b763cecaff56e`  
		Last Modified: Mon, 27 Jun 2022 23:41:56 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95691dcdde5f2ee25bddc7d7b86e909e83b4afb1e4df5fad18d9522c3f510579`  
		Last Modified: Mon, 27 Jun 2022 23:41:54 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5782ffaaa3341fdec1b0c7406c0492d5cff1a9970a6bd418392b7174e60bea6f`  
		Last Modified: Mon, 27 Jun 2022 23:42:01 GMT  
		Size: 53.3 MB (53324071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01dd932f22732278b472cba5572dc1447697a6c2ef0d4ad0fb6f0d9ae009d07`  
		Last Modified: Mon, 27 Jun 2022 23:41:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d729e5c05f924689961a0ec3f59e39b68696747fe8e84592e0c7d3466f264bef`  
		Last Modified: Mon, 27 Jun 2022 23:42:01 GMT  
		Size: 42.1 MB (42056996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abe7fac72065516d8f16acb9fddfb5df729c103afd883ab5c353157a60ae4be`  
		Last Modified: Mon, 27 Jun 2022 23:41:53 GMT  
		Size: 5.2 KB (5161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:a840244706a5fdc3c704b15a3700bfda39fdc069262d7753fa09de2d9faf5f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:b2d83fc6fbd16d59db1adc8d2e81a65663148b243bb36c6dc645f3c6468dc284
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155908369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef9083d9892db139e2b7c81fd133836e7aa32db2b5f1d5702e2593100fa1417`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Tue, 28 Jun 2022 00:21:38 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:21:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:21:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:21:53 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 28 Jun 2022 00:21:53 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:21:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:21:54 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:21:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6b647ddb19a4d8418c24e6de80b121ac50563fc8c2d90f0b59dbb619c9507`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09ca0f0cb24ca059efd9c31d1802ff067f77165a930b3ba53b1d3ff9833b18d`  
		Last Modified: Tue, 28 Jun 2022 00:24:35 GMT  
		Size: 109.1 MB (109104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e223e3cd2fdb62988d08fe4dfdc8a8a3ca0916a0c151f9ce2bb463a8033ce0a`  
		Last Modified: Tue, 28 Jun 2022 00:24:17 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b038d826c6572e26b8ef0a0bc128710feb4dd940bc174c570be426a67a57fff`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33ac6052fc913fd126296376ceeb69c617236fa33d820a02b8744148615f543`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:a840244706a5fdc3c704b15a3700bfda39fdc069262d7753fa09de2d9faf5f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:b2d83fc6fbd16d59db1adc8d2e81a65663148b243bb36c6dc645f3c6468dc284
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155908369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef9083d9892db139e2b7c81fd133836e7aa32db2b5f1d5702e2593100fa1417`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Tue, 28 Jun 2022 00:21:38 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:21:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:21:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:21:53 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 28 Jun 2022 00:21:53 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:21:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:21:54 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:21:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6b647ddb19a4d8418c24e6de80b121ac50563fc8c2d90f0b59dbb619c9507`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09ca0f0cb24ca059efd9c31d1802ff067f77165a930b3ba53b1d3ff9833b18d`  
		Last Modified: Tue, 28 Jun 2022 00:24:35 GMT  
		Size: 109.1 MB (109104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e223e3cd2fdb62988d08fe4dfdc8a8a3ca0916a0c151f9ce2bb463a8033ce0a`  
		Last Modified: Tue, 28 Jun 2022 00:24:17 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b038d826c6572e26b8ef0a0bc128710feb4dd940bc174c570be426a67a57fff`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33ac6052fc913fd126296376ceeb69c617236fa33d820a02b8744148615f543`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:a3db7b0ac138588506dbcb958bbfa4a3a71da227fb1410b6c8ba86e5a0632f88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:a695fb7643f3b28bb720670c8557e946fb0df0bed6f118cecb61b46ef353ce46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131788232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab8fad28a2df8c23829d482831a1a913823340b7de88e6452855ff042b662093`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:23:26 GMT
ADD file:837f6c6e7e20067b92edb72e78a8399e6cbbd72dab23db7b5b5a301c58d2a0de in / 
# Tue, 14 Jun 2022 18:23:26 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 18:39:39 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 18:39:39 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 18:39:43 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Jun 2022 00:20:13 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 28 Jun 2022 00:20:15 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:20:15 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 28 Jun 2022 00:20:15 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 28 Jun 2022 00:20:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 28 Jun 2022 00:20:42 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 28 Jun 2022 00:20:43 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 28 Jun 2022 00:20:43 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 28 Jun 2022 00:21:14 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 28 Jun 2022 00:21:14 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:21:14 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:21:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:21:15 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:21:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5f160c0f6cac587a73883b48a8857f5cce0930112792cef25c62510e256e93dc`  
		Last Modified: Tue, 14 Jun 2022 18:24:18 GMT  
		Size: 39.2 MB (39219730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86c3d841d1984f858257755bdf734554725af4f926f3b1d1b22f119cce8bda9`  
		Last Modified: Tue, 14 Jun 2022 18:41:49 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f026b3ec1ed102cfe531d812e2063669bad08ac3a0ac68a31e44083d9b9a5f5d`  
		Last Modified: Tue, 14 Jun 2022 18:41:47 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478636a5486e48bba38a3fa287f3b8ac0f9475d0a3fa2d12fa93b380345be6bf`  
		Last Modified: Tue, 28 Jun 2022 00:23:57 GMT  
		Size: 4.6 MB (4584099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b941aa3584d8a0c760fdd99040fee760b2847d93819a44dd2bfb396fd7c04d9`  
		Last Modified: Tue, 28 Jun 2022 00:23:57 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebddb2e985f2fd2f75055ad472eb725ae21b4c841e7fbc28384250ff79b1b15`  
		Last Modified: Tue, 28 Jun 2022 00:23:54 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a2abf961ad5794642b9911e32bfcc6a56c27ae26596ae3cb1ae8bafdc200f9`  
		Last Modified: Tue, 28 Jun 2022 00:24:02 GMT  
		Size: 47.3 MB (47257530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215106930b414b865a2703a23e7428c641bb28d7250b3d520938fca7e7daa217`  
		Last Modified: Tue, 28 Jun 2022 00:23:54 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0746f4080775920510cf00ee4853ff6c24db6c4707f4817f89af986192d99695`  
		Last Modified: Tue, 28 Jun 2022 00:24:02 GMT  
		Size: 39.8 MB (39788521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1195705edd352cba35d5fd3544b781c31a5081fa3bdece1936be2cea886506f6`  
		Last Modified: Tue, 28 Jun 2022 00:23:54 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:0418232b74414d7e223da6fc26f47d9498abd72b4ca3bb1cd826f8f05ea55374
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138660393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a0eef221ccdafeb4649e0af86a16d1bf826ed66807fd64248a212871c04c2a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:41:36 GMT
ADD file:4a6ee90ad73353bfb87b2f121e06bddaed6104536e485baa83fadbe7facc774c in / 
# Tue, 14 Jun 2022 18:41:37 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 19:17:17 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 19:17:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 19:17:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 27 Jun 2022 23:40:26 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Mon, 27 Jun 2022 23:40:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Mon, 27 Jun 2022 23:40:28 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 27 Jun 2022 23:40:29 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Mon, 27 Jun 2022 23:40:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 27 Jun 2022 23:40:56 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Mon, 27 Jun 2022 23:40:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 27 Jun 2022 23:40:57 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Mon, 27 Jun 2022 23:41:27 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 27 Jun 2022 23:41:27 GMT
VOLUME [/var/lib/mysql]
# Mon, 27 Jun 2022 23:41:29 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Mon, 27 Jun 2022 23:41:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Jun 2022 23:41:30 GMT
EXPOSE 3306 33060
# Mon, 27 Jun 2022 23:41:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2bbc1bf883bd601c0da5735b538963308bcc17f90d36525ecc93456ffad79064`  
		Last Modified: Tue, 14 Jun 2022 18:42:39 GMT  
		Size: 38.0 MB (38012371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428f9d18fc319262a774f75a5849d4819b5b44cbf07fbb5e3c262e5cf30c22d`  
		Last Modified: Tue, 14 Jun 2022 19:19:14 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cba94044003680a99c76f187ea817c71b843de38bb7f28faf8ca6508efd45e`  
		Last Modified: Tue, 14 Jun 2022 19:19:12 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac1107eaf64ada9002dc0dbf73e0a8b8c2a3e2dfe557a59ee79ae5296dd6d35`  
		Last Modified: Mon, 27 Jun 2022 23:41:57 GMT  
		Size: 4.4 MB (4400369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287b497aedf9bf453ca624e6f7b036489fa7091918b209ff279b763cecaff56e`  
		Last Modified: Mon, 27 Jun 2022 23:41:56 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95691dcdde5f2ee25bddc7d7b86e909e83b4afb1e4df5fad18d9522c3f510579`  
		Last Modified: Mon, 27 Jun 2022 23:41:54 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5782ffaaa3341fdec1b0c7406c0492d5cff1a9970a6bd418392b7174e60bea6f`  
		Last Modified: Mon, 27 Jun 2022 23:42:01 GMT  
		Size: 53.3 MB (53324071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01dd932f22732278b472cba5572dc1447697a6c2ef0d4ad0fb6f0d9ae009d07`  
		Last Modified: Mon, 27 Jun 2022 23:41:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d729e5c05f924689961a0ec3f59e39b68696747fe8e84592e0c7d3466f264bef`  
		Last Modified: Mon, 27 Jun 2022 23:42:01 GMT  
		Size: 42.1 MB (42056996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abe7fac72065516d8f16acb9fddfb5df729c103afd883ab5c353157a60ae4be`  
		Last Modified: Mon, 27 Jun 2022 23:41:53 GMT  
		Size: 5.2 KB (5161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.29`

```console
$ docker pull mysql@sha256:a840244706a5fdc3c704b15a3700bfda39fdc069262d7753fa09de2d9faf5f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.29` - linux; amd64

```console
$ docker pull mysql@sha256:b2d83fc6fbd16d59db1adc8d2e81a65663148b243bb36c6dc645f3c6468dc284
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155908369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef9083d9892db139e2b7c81fd133836e7aa32db2b5f1d5702e2593100fa1417`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Tue, 28 Jun 2022 00:21:38 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:21:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:21:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:21:53 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 28 Jun 2022 00:21:53 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:21:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:21:54 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:21:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6b647ddb19a4d8418c24e6de80b121ac50563fc8c2d90f0b59dbb619c9507`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09ca0f0cb24ca059efd9c31d1802ff067f77165a930b3ba53b1d3ff9833b18d`  
		Last Modified: Tue, 28 Jun 2022 00:24:35 GMT  
		Size: 109.1 MB (109104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e223e3cd2fdb62988d08fe4dfdc8a8a3ca0916a0c151f9ce2bb463a8033ce0a`  
		Last Modified: Tue, 28 Jun 2022 00:24:17 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b038d826c6572e26b8ef0a0bc128710feb4dd940bc174c570be426a67a57fff`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33ac6052fc913fd126296376ceeb69c617236fa33d820a02b8744148615f543`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.29-debian`

```console
$ docker pull mysql@sha256:a840244706a5fdc3c704b15a3700bfda39fdc069262d7753fa09de2d9faf5f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.29-debian` - linux; amd64

```console
$ docker pull mysql@sha256:b2d83fc6fbd16d59db1adc8d2e81a65663148b243bb36c6dc645f3c6468dc284
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155908369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef9083d9892db139e2b7c81fd133836e7aa32db2b5f1d5702e2593100fa1417`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Tue, 28 Jun 2022 00:21:38 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:21:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:21:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:21:53 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 28 Jun 2022 00:21:53 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:21:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:21:54 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:21:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6b647ddb19a4d8418c24e6de80b121ac50563fc8c2d90f0b59dbb619c9507`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09ca0f0cb24ca059efd9c31d1802ff067f77165a930b3ba53b1d3ff9833b18d`  
		Last Modified: Tue, 28 Jun 2022 00:24:35 GMT  
		Size: 109.1 MB (109104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e223e3cd2fdb62988d08fe4dfdc8a8a3ca0916a0c151f9ce2bb463a8033ce0a`  
		Last Modified: Tue, 28 Jun 2022 00:24:17 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b038d826c6572e26b8ef0a0bc128710feb4dd940bc174c570be426a67a57fff`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33ac6052fc913fd126296376ceeb69c617236fa33d820a02b8744148615f543`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.29-oracle`

```console
$ docker pull mysql@sha256:a3db7b0ac138588506dbcb958bbfa4a3a71da227fb1410b6c8ba86e5a0632f88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.29-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:a695fb7643f3b28bb720670c8557e946fb0df0bed6f118cecb61b46ef353ce46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131788232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab8fad28a2df8c23829d482831a1a913823340b7de88e6452855ff042b662093`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:23:26 GMT
ADD file:837f6c6e7e20067b92edb72e78a8399e6cbbd72dab23db7b5b5a301c58d2a0de in / 
# Tue, 14 Jun 2022 18:23:26 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 18:39:39 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 18:39:39 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 18:39:43 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Jun 2022 00:20:13 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 28 Jun 2022 00:20:15 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:20:15 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 28 Jun 2022 00:20:15 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 28 Jun 2022 00:20:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 28 Jun 2022 00:20:42 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 28 Jun 2022 00:20:43 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 28 Jun 2022 00:20:43 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 28 Jun 2022 00:21:14 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 28 Jun 2022 00:21:14 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:21:14 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:21:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:21:15 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:21:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5f160c0f6cac587a73883b48a8857f5cce0930112792cef25c62510e256e93dc`  
		Last Modified: Tue, 14 Jun 2022 18:24:18 GMT  
		Size: 39.2 MB (39219730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86c3d841d1984f858257755bdf734554725af4f926f3b1d1b22f119cce8bda9`  
		Last Modified: Tue, 14 Jun 2022 18:41:49 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f026b3ec1ed102cfe531d812e2063669bad08ac3a0ac68a31e44083d9b9a5f5d`  
		Last Modified: Tue, 14 Jun 2022 18:41:47 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478636a5486e48bba38a3fa287f3b8ac0f9475d0a3fa2d12fa93b380345be6bf`  
		Last Modified: Tue, 28 Jun 2022 00:23:57 GMT  
		Size: 4.6 MB (4584099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b941aa3584d8a0c760fdd99040fee760b2847d93819a44dd2bfb396fd7c04d9`  
		Last Modified: Tue, 28 Jun 2022 00:23:57 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebddb2e985f2fd2f75055ad472eb725ae21b4c841e7fbc28384250ff79b1b15`  
		Last Modified: Tue, 28 Jun 2022 00:23:54 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a2abf961ad5794642b9911e32bfcc6a56c27ae26596ae3cb1ae8bafdc200f9`  
		Last Modified: Tue, 28 Jun 2022 00:24:02 GMT  
		Size: 47.3 MB (47257530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215106930b414b865a2703a23e7428c641bb28d7250b3d520938fca7e7daa217`  
		Last Modified: Tue, 28 Jun 2022 00:23:54 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0746f4080775920510cf00ee4853ff6c24db6c4707f4817f89af986192d99695`  
		Last Modified: Tue, 28 Jun 2022 00:24:02 GMT  
		Size: 39.8 MB (39788521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1195705edd352cba35d5fd3544b781c31a5081fa3bdece1936be2cea886506f6`  
		Last Modified: Tue, 28 Jun 2022 00:23:54 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.29-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:0418232b74414d7e223da6fc26f47d9498abd72b4ca3bb1cd826f8f05ea55374
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138660393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a0eef221ccdafeb4649e0af86a16d1bf826ed66807fd64248a212871c04c2a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:41:36 GMT
ADD file:4a6ee90ad73353bfb87b2f121e06bddaed6104536e485baa83fadbe7facc774c in / 
# Tue, 14 Jun 2022 18:41:37 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 19:17:17 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 19:17:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 19:17:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 27 Jun 2022 23:40:26 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Mon, 27 Jun 2022 23:40:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Mon, 27 Jun 2022 23:40:28 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 27 Jun 2022 23:40:29 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Mon, 27 Jun 2022 23:40:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 27 Jun 2022 23:40:56 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Mon, 27 Jun 2022 23:40:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 27 Jun 2022 23:40:57 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Mon, 27 Jun 2022 23:41:27 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 27 Jun 2022 23:41:27 GMT
VOLUME [/var/lib/mysql]
# Mon, 27 Jun 2022 23:41:29 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Mon, 27 Jun 2022 23:41:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Jun 2022 23:41:30 GMT
EXPOSE 3306 33060
# Mon, 27 Jun 2022 23:41:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2bbc1bf883bd601c0da5735b538963308bcc17f90d36525ecc93456ffad79064`  
		Last Modified: Tue, 14 Jun 2022 18:42:39 GMT  
		Size: 38.0 MB (38012371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428f9d18fc319262a774f75a5849d4819b5b44cbf07fbb5e3c262e5cf30c22d`  
		Last Modified: Tue, 14 Jun 2022 19:19:14 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cba94044003680a99c76f187ea817c71b843de38bb7f28faf8ca6508efd45e`  
		Last Modified: Tue, 14 Jun 2022 19:19:12 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac1107eaf64ada9002dc0dbf73e0a8b8c2a3e2dfe557a59ee79ae5296dd6d35`  
		Last Modified: Mon, 27 Jun 2022 23:41:57 GMT  
		Size: 4.4 MB (4400369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287b497aedf9bf453ca624e6f7b036489fa7091918b209ff279b763cecaff56e`  
		Last Modified: Mon, 27 Jun 2022 23:41:56 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95691dcdde5f2ee25bddc7d7b86e909e83b4afb1e4df5fad18d9522c3f510579`  
		Last Modified: Mon, 27 Jun 2022 23:41:54 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5782ffaaa3341fdec1b0c7406c0492d5cff1a9970a6bd418392b7174e60bea6f`  
		Last Modified: Mon, 27 Jun 2022 23:42:01 GMT  
		Size: 53.3 MB (53324071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01dd932f22732278b472cba5572dc1447697a6c2ef0d4ad0fb6f0d9ae009d07`  
		Last Modified: Mon, 27 Jun 2022 23:41:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d729e5c05f924689961a0ec3f59e39b68696747fe8e84592e0c7d3466f264bef`  
		Last Modified: Mon, 27 Jun 2022 23:42:01 GMT  
		Size: 42.1 MB (42056996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abe7fac72065516d8f16acb9fddfb5df729c103afd883ab5c353157a60ae4be`  
		Last Modified: Mon, 27 Jun 2022 23:41:53 GMT  
		Size: 5.2 KB (5161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:a840244706a5fdc3c704b15a3700bfda39fdc069262d7753fa09de2d9faf5f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:b2d83fc6fbd16d59db1adc8d2e81a65663148b243bb36c6dc645f3c6468dc284
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155908369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef9083d9892db139e2b7c81fd133836e7aa32db2b5f1d5702e2593100fa1417`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Tue, 28 Jun 2022 00:21:38 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:21:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:21:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:21:53 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 28 Jun 2022 00:21:53 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:21:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:21:54 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:21:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6b647ddb19a4d8418c24e6de80b121ac50563fc8c2d90f0b59dbb619c9507`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09ca0f0cb24ca059efd9c31d1802ff067f77165a930b3ba53b1d3ff9833b18d`  
		Last Modified: Tue, 28 Jun 2022 00:24:35 GMT  
		Size: 109.1 MB (109104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e223e3cd2fdb62988d08fe4dfdc8a8a3ca0916a0c151f9ce2bb463a8033ce0a`  
		Last Modified: Tue, 28 Jun 2022 00:24:17 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b038d826c6572e26b8ef0a0bc128710feb4dd940bc174c570be426a67a57fff`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33ac6052fc913fd126296376ceeb69c617236fa33d820a02b8744148615f543`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:a840244706a5fdc3c704b15a3700bfda39fdc069262d7753fa09de2d9faf5f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:b2d83fc6fbd16d59db1adc8d2e81a65663148b243bb36c6dc645f3c6468dc284
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155908369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef9083d9892db139e2b7c81fd133836e7aa32db2b5f1d5702e2593100fa1417`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:46 GMT
ADD file:0ae121f9805d31a4ad0ed63e1fc397167a23656a285572fe68bfc51ea91ecfdd in / 
# Thu, 23 Jun 2022 00:20:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:05:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Jun 2022 04:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:05:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 04:05:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 04:05:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Jun 2022 00:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Jun 2022 00:21:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 28 Jun 2022 00:21:38 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Tue, 28 Jun 2022 00:21:38 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 28 Jun 2022 00:21:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 28 Jun 2022 00:21:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:21:53 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 28 Jun 2022 00:21:53 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:21:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 28 Jun 2022 00:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:21:54 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:21:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:824b15f81d6568adc139263c39805e52d9880758b907f40144bbb1938ca59323`  
		Last Modified: Thu, 23 Jun 2022 00:26:03 GMT  
		Size: 27.1 MB (27140043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559dd1913db86c3984c4dfc3e07fccee1fecc810999b4b6aea8b5cde104d207`  
		Last Modified: Thu, 23 Jun 2022 04:07:11 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e201c19614e69f7e7040b951f02b91baf11428b0f83cab3516df27a8f4a79870`  
		Last Modified: Thu, 23 Jun 2022 04:07:12 GMT  
		Size: 4.2 MB (4179291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4247e8f61251b7262eb83877350fc1c641526969e1ce931ec6d78361cb9236c`  
		Last Modified: Thu, 23 Jun 2022 04:07:10 GMT  
		Size: 1.4 MB (1386689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9fefd8cfb55346940b7d843ac4d88addc2a66b38e85f7b1c0b94820ce698ca`  
		Last Modified: Thu, 23 Jun 2022 04:07:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3787edd16df30d4ca1f062e3becefcf1e1f5595517d4325c48006156f358ee`  
		Last Modified: Tue, 28 Jun 2022 00:24:23 GMT  
		Size: 14.1 MB (14086998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bb40f875d341e08634fbde0893016a25f4a8a6777248ef3ff6ecdd8b0f0a3d`  
		Last Modified: Tue, 28 Jun 2022 00:24:20 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f6b647ddb19a4d8418c24e6de80b121ac50563fc8c2d90f0b59dbb619c9507`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09ca0f0cb24ca059efd9c31d1802ff067f77165a930b3ba53b1d3ff9833b18d`  
		Last Modified: Tue, 28 Jun 2022 00:24:35 GMT  
		Size: 109.1 MB (109104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e223e3cd2fdb62988d08fe4dfdc8a8a3ca0916a0c151f9ce2bb463a8033ce0a`  
		Last Modified: Tue, 28 Jun 2022 00:24:17 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b038d826c6572e26b8ef0a0bc128710feb4dd940bc174c570be426a67a57fff`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33ac6052fc913fd126296376ceeb69c617236fa33d820a02b8744148615f543`  
		Last Modified: Tue, 28 Jun 2022 00:24:18 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:a3db7b0ac138588506dbcb958bbfa4a3a71da227fb1410b6c8ba86e5a0632f88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:a695fb7643f3b28bb720670c8557e946fb0df0bed6f118cecb61b46ef353ce46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131788232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab8fad28a2df8c23829d482831a1a913823340b7de88e6452855ff042b662093`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:23:26 GMT
ADD file:837f6c6e7e20067b92edb72e78a8399e6cbbd72dab23db7b5b5a301c58d2a0de in / 
# Tue, 14 Jun 2022 18:23:26 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 18:39:39 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 18:39:39 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 18:39:43 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Jun 2022 00:20:13 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 28 Jun 2022 00:20:15 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 28 Jun 2022 00:20:15 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 28 Jun 2022 00:20:15 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 28 Jun 2022 00:20:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 28 Jun 2022 00:20:42 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 28 Jun 2022 00:20:43 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 28 Jun 2022 00:20:43 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 28 Jun 2022 00:21:14 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 28 Jun 2022 00:21:14 GMT
VOLUME [/var/lib/mysql]
# Tue, 28 Jun 2022 00:21:14 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 28 Jun 2022 00:21:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jun 2022 00:21:15 GMT
EXPOSE 3306 33060
# Tue, 28 Jun 2022 00:21:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5f160c0f6cac587a73883b48a8857f5cce0930112792cef25c62510e256e93dc`  
		Last Modified: Tue, 14 Jun 2022 18:24:18 GMT  
		Size: 39.2 MB (39219730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86c3d841d1984f858257755bdf734554725af4f926f3b1d1b22f119cce8bda9`  
		Last Modified: Tue, 14 Jun 2022 18:41:49 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f026b3ec1ed102cfe531d812e2063669bad08ac3a0ac68a31e44083d9b9a5f5d`  
		Last Modified: Tue, 14 Jun 2022 18:41:47 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478636a5486e48bba38a3fa287f3b8ac0f9475d0a3fa2d12fa93b380345be6bf`  
		Last Modified: Tue, 28 Jun 2022 00:23:57 GMT  
		Size: 4.6 MB (4584099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b941aa3584d8a0c760fdd99040fee760b2847d93819a44dd2bfb396fd7c04d9`  
		Last Modified: Tue, 28 Jun 2022 00:23:57 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebddb2e985f2fd2f75055ad472eb725ae21b4c841e7fbc28384250ff79b1b15`  
		Last Modified: Tue, 28 Jun 2022 00:23:54 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a2abf961ad5794642b9911e32bfcc6a56c27ae26596ae3cb1ae8bafdc200f9`  
		Last Modified: Tue, 28 Jun 2022 00:24:02 GMT  
		Size: 47.3 MB (47257530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215106930b414b865a2703a23e7428c641bb28d7250b3d520938fca7e7daa217`  
		Last Modified: Tue, 28 Jun 2022 00:23:54 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0746f4080775920510cf00ee4853ff6c24db6c4707f4817f89af986192d99695`  
		Last Modified: Tue, 28 Jun 2022 00:24:02 GMT  
		Size: 39.8 MB (39788521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1195705edd352cba35d5fd3544b781c31a5081fa3bdece1936be2cea886506f6`  
		Last Modified: Tue, 28 Jun 2022 00:23:54 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:0418232b74414d7e223da6fc26f47d9498abd72b4ca3bb1cd826f8f05ea55374
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138660393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a0eef221ccdafeb4649e0af86a16d1bf826ed66807fd64248a212871c04c2a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 14 Jun 2022 18:41:36 GMT
ADD file:4a6ee90ad73353bfb87b2f121e06bddaed6104536e485baa83fadbe7facc774c in / 
# Tue, 14 Jun 2022 18:41:37 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 19:17:17 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 14 Jun 2022 19:17:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 14 Jun 2022 19:17:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 27 Jun 2022 23:40:26 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Mon, 27 Jun 2022 23:40:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Mon, 27 Jun 2022 23:40:28 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 27 Jun 2022 23:40:29 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Mon, 27 Jun 2022 23:40:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 27 Jun 2022 23:40:56 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Mon, 27 Jun 2022 23:40:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 27 Jun 2022 23:40:57 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Mon, 27 Jun 2022 23:41:27 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 27 Jun 2022 23:41:27 GMT
VOLUME [/var/lib/mysql]
# Mon, 27 Jun 2022 23:41:29 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Mon, 27 Jun 2022 23:41:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Jun 2022 23:41:30 GMT
EXPOSE 3306 33060
# Mon, 27 Jun 2022 23:41:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2bbc1bf883bd601c0da5735b538963308bcc17f90d36525ecc93456ffad79064`  
		Last Modified: Tue, 14 Jun 2022 18:42:39 GMT  
		Size: 38.0 MB (38012371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428f9d18fc319262a774f75a5849d4819b5b44cbf07fbb5e3c262e5cf30c22d`  
		Last Modified: Tue, 14 Jun 2022 19:19:14 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cba94044003680a99c76f187ea817c71b843de38bb7f28faf8ca6508efd45e`  
		Last Modified: Tue, 14 Jun 2022 19:19:12 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac1107eaf64ada9002dc0dbf73e0a8b8c2a3e2dfe557a59ee79ae5296dd6d35`  
		Last Modified: Mon, 27 Jun 2022 23:41:57 GMT  
		Size: 4.4 MB (4400369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287b497aedf9bf453ca624e6f7b036489fa7091918b209ff279b763cecaff56e`  
		Last Modified: Mon, 27 Jun 2022 23:41:56 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95691dcdde5f2ee25bddc7d7b86e909e83b4afb1e4df5fad18d9522c3f510579`  
		Last Modified: Mon, 27 Jun 2022 23:41:54 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5782ffaaa3341fdec1b0c7406c0492d5cff1a9970a6bd418392b7174e60bea6f`  
		Last Modified: Mon, 27 Jun 2022 23:42:01 GMT  
		Size: 53.3 MB (53324071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01dd932f22732278b472cba5572dc1447697a6c2ef0d4ad0fb6f0d9ae009d07`  
		Last Modified: Mon, 27 Jun 2022 23:41:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d729e5c05f924689961a0ec3f59e39b68696747fe8e84592e0c7d3466f264bef`  
		Last Modified: Mon, 27 Jun 2022 23:42:01 GMT  
		Size: 42.1 MB (42056996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abe7fac72065516d8f16acb9fddfb5df729c103afd883ab5c353157a60ae4be`  
		Last Modified: Mon, 27 Jun 2022 23:41:53 GMT  
		Size: 5.2 KB (5161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
