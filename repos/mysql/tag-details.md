<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5-debian`](#mysql5-debian)
-	[`mysql:5-oracle`](#mysql5-oracle)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7-debian`](#mysql57-debian)
-	[`mysql:5.7-oracle`](#mysql57-oracle)
-	[`mysql:5.7.41`](#mysql5741)
-	[`mysql:5.7.41-debian`](#mysql5741-debian)
-	[`mysql:5.7.41-oracle`](#mysql5741-oracle)
-	[`mysql:8`](#mysql8)
-	[`mysql:8-debian`](#mysql8-debian)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0.32`](#mysql8032)
-	[`mysql:8.0.32-debian`](#mysql8032-debian)
-	[`mysql:8.0.32-oracle`](#mysql8032-oracle)
-	[`mysql:debian`](#mysqldebian)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)

## `mysql:5`

```console
$ docker pull mysql@sha256:1780318bdabc0edd36907bf91b47632eb912e8ea91258eca3590f8aca6f54836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:59391c720d279e070440dabc9b39e478ffb310d80759ad18fa7ad61dd2ec9b7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130037432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6ee2207ee7a9ed4f5c718a507fd00dace311300153b99f6830ce34741f2f093`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Mar 2023 19:26:42 GMT
ADD file:c2562ae661b3cd914b2c0dd27aba7ee36bffbeb92415b7b80c111a5d563d07ed in / 
# Tue, 21 Mar 2023 19:26:43 GMT
CMD ["/bin/bash"]
# Tue, 21 Mar 2023 20:51:10 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 21 Mar 2023 20:51:10 GMT
ENV GOSU_VERSION=1.16
# Tue, 21 Mar 2023 20:51:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Mar 2023 20:51:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Tue, 21 Mar 2023 20:51:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 21 Mar 2023 20:51:32 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 21 Mar 2023 20:51:32 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Tue, 21 Mar 2023 20:51:32 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 21 Mar 2023 20:51:51 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 21 Mar 2023 20:51:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 21 Mar 2023 20:51:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Tue, 21 Mar 2023 20:52:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 21 Mar 2023 20:52:16 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Mar 2023 20:52:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 21 Mar 2023 20:52:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Mar 2023 20:52:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Mar 2023 20:52:17 GMT
EXPOSE 3306 33060
# Tue, 21 Mar 2023 20:52:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ec521688c56b41126476e7ab1f7ab7305384f5b5326e80a8ba52b8d4deead22`  
		Last Modified: Tue, 21 Mar 2023 19:27:26 GMT  
		Size: 50.5 MB (50471128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f911f9b90db6be6d326471ffa9acef77985640199aca2f765be1efa82037a3d1`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38eb4fe7ed26a84c3c1f6a17d0fc831f0b7e5c43fb1ed355ff3240a813dcad61`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 983.7 KB (983706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f772a6b25f5bbd71a55ff1d40333ea8494f8281c8f386b58432036fcc96444`  
		Last Modified: Tue, 21 Mar 2023 20:52:51 GMT  
		Size: 4.6 MB (4591670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499456357ebfbc78d9408a5599908b7ded3b1d422fddf5865cdb8c8ae0fa8629`  
		Last Modified: Tue, 21 Mar 2023 20:52:50 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274f3ad0dcecde2bd838ef7f34562cbe017da4dae64469f53b48af068390d06a`  
		Last Modified: Tue, 21 Mar 2023 20:52:50 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a5b12e1de159ec628987eeb584030eb2acc6cb8025177a2a10f77e556fcc1`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 25.5 MB (25532897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0c5c82dbbc3a0e7e37dde0dd947d4401201452f147dd8f7982f6c026f3d41b`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bd281f46007c1698e833f1f602b126ba9a74db11dd4b158d61130d0edb2bcd`  
		Last Modified: Tue, 21 Mar 2023 20:52:57 GMT  
		Size: 48.4 MB (48448352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3289c4277a830488286360c722a87a8b9153b68aa6893a87fe1faf1e4018c15e`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b66f10a11fa382cf7bf501cb958d64ca12f4e236ba5f03d95028fa06421e33a`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:849a8e87076f75717e1f98102ed1545396faab1cb2c99c768bf2b5b430571604
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:2bbef75b058643f5a747c13661a88ee3301df9e25f0eaeb358587cc37da86afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162693934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88338e85f040d97b75f2d43518736f4af9e52fa4c4c577cd34b134273a079266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:50 GMT
ADD file:52316aa7d631242cd16337be337e57187ef07d3965e6284321fbdcd5b4f92b64 in / 
# Thu, 23 Mar 2023 01:30:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 11:00:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Mar 2023 11:00:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:00:28 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 11:00:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 11:00:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 11:00:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:00:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 11:00:45 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 23 Mar 2023 11:00:45 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Thu, 23 Mar 2023 11:00:46 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Mar 2023 11:01:03 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Thu, 23 Mar 2023 11:01:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 11:01:04 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 11:01:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 11:01:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:01:05 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 11:01:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3689b8de819b48387712c6d4d62d26a52a04c9e88afc68fb9d1dbe48bfa9e21d`  
		Last Modified: Thu, 23 Mar 2023 01:35:01 GMT  
		Size: 27.1 MB (27139869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ac63a14e4479941312ab4b314bbd36b8eed13e848b7446b33d62d1cf387c14`  
		Last Modified: Thu, 23 Mar 2023 11:01:59 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a94b43bbfe3822fc0a3c87da156138a81cec71bf1b9a2e00f3acc1b9819eca`  
		Last Modified: Thu, 23 Mar 2023 11:01:58 GMT  
		Size: 4.2 MB (4182339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38763e84573623aeb1cff67387112f2d0b31e5ed0b899e3b3a126770e46d8b94`  
		Last Modified: Thu, 23 Mar 2023 11:01:58 GMT  
		Size: 1.4 MB (1441745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcbc7fd4a2d7d18a737618196f4d75de0a316eaf5c125b2d4d35a7eb037426d`  
		Last Modified: Thu, 23 Mar 2023 11:01:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19764d7bd70a9eea88bec2db9d035ffe9224b9dcd7c0613e42f63b775f8f75d3`  
		Last Modified: Thu, 23 Mar 2023 11:02:00 GMT  
		Size: 14.1 MB (14086905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a2769597f7f726053839c80035384b62ea02c2f3dafa473e5200c96236b67c`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55969b3a4225bf2037f3ccfc7930ed5b0cfed7aeee036deb0d7aee144dfbc425`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4898aaf83c5d2f75aa7c90e3936fb2faf0f565889f5973fb820f1330cff028`  
		Last Modified: Thu, 23 Mar 2023 11:02:10 GMT  
		Size: 115.8 MB (115832889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9972a98a4d99007516b2303bc1ca8e06d9696adff985ac28b4f52bbb086738`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b8313553fddc90f14c25b3007f8f77459244ac46fbcd5580f9f3c31ba6a0d1`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:1780318bdabc0edd36907bf91b47632eb912e8ea91258eca3590f8aca6f54836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:59391c720d279e070440dabc9b39e478ffb310d80759ad18fa7ad61dd2ec9b7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130037432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6ee2207ee7a9ed4f5c718a507fd00dace311300153b99f6830ce34741f2f093`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Mar 2023 19:26:42 GMT
ADD file:c2562ae661b3cd914b2c0dd27aba7ee36bffbeb92415b7b80c111a5d563d07ed in / 
# Tue, 21 Mar 2023 19:26:43 GMT
CMD ["/bin/bash"]
# Tue, 21 Mar 2023 20:51:10 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 21 Mar 2023 20:51:10 GMT
ENV GOSU_VERSION=1.16
# Tue, 21 Mar 2023 20:51:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Mar 2023 20:51:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Tue, 21 Mar 2023 20:51:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 21 Mar 2023 20:51:32 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 21 Mar 2023 20:51:32 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Tue, 21 Mar 2023 20:51:32 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 21 Mar 2023 20:51:51 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 21 Mar 2023 20:51:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 21 Mar 2023 20:51:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Tue, 21 Mar 2023 20:52:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 21 Mar 2023 20:52:16 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Mar 2023 20:52:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 21 Mar 2023 20:52:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Mar 2023 20:52:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Mar 2023 20:52:17 GMT
EXPOSE 3306 33060
# Tue, 21 Mar 2023 20:52:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ec521688c56b41126476e7ab1f7ab7305384f5b5326e80a8ba52b8d4deead22`  
		Last Modified: Tue, 21 Mar 2023 19:27:26 GMT  
		Size: 50.5 MB (50471128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f911f9b90db6be6d326471ffa9acef77985640199aca2f765be1efa82037a3d1`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38eb4fe7ed26a84c3c1f6a17d0fc831f0b7e5c43fb1ed355ff3240a813dcad61`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 983.7 KB (983706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f772a6b25f5bbd71a55ff1d40333ea8494f8281c8f386b58432036fcc96444`  
		Last Modified: Tue, 21 Mar 2023 20:52:51 GMT  
		Size: 4.6 MB (4591670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499456357ebfbc78d9408a5599908b7ded3b1d422fddf5865cdb8c8ae0fa8629`  
		Last Modified: Tue, 21 Mar 2023 20:52:50 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274f3ad0dcecde2bd838ef7f34562cbe017da4dae64469f53b48af068390d06a`  
		Last Modified: Tue, 21 Mar 2023 20:52:50 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a5b12e1de159ec628987eeb584030eb2acc6cb8025177a2a10f77e556fcc1`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 25.5 MB (25532897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0c5c82dbbc3a0e7e37dde0dd947d4401201452f147dd8f7982f6c026f3d41b`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bd281f46007c1698e833f1f602b126ba9a74db11dd4b158d61130d0edb2bcd`  
		Last Modified: Tue, 21 Mar 2023 20:52:57 GMT  
		Size: 48.4 MB (48448352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3289c4277a830488286360c722a87a8b9153b68aa6893a87fe1faf1e4018c15e`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b66f10a11fa382cf7bf501cb958d64ca12f4e236ba5f03d95028fa06421e33a`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:1780318bdabc0edd36907bf91b47632eb912e8ea91258eca3590f8aca6f54836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:59391c720d279e070440dabc9b39e478ffb310d80759ad18fa7ad61dd2ec9b7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130037432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6ee2207ee7a9ed4f5c718a507fd00dace311300153b99f6830ce34741f2f093`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Mar 2023 19:26:42 GMT
ADD file:c2562ae661b3cd914b2c0dd27aba7ee36bffbeb92415b7b80c111a5d563d07ed in / 
# Tue, 21 Mar 2023 19:26:43 GMT
CMD ["/bin/bash"]
# Tue, 21 Mar 2023 20:51:10 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 21 Mar 2023 20:51:10 GMT
ENV GOSU_VERSION=1.16
# Tue, 21 Mar 2023 20:51:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Mar 2023 20:51:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Tue, 21 Mar 2023 20:51:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 21 Mar 2023 20:51:32 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 21 Mar 2023 20:51:32 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Tue, 21 Mar 2023 20:51:32 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 21 Mar 2023 20:51:51 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 21 Mar 2023 20:51:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 21 Mar 2023 20:51:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Tue, 21 Mar 2023 20:52:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 21 Mar 2023 20:52:16 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Mar 2023 20:52:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 21 Mar 2023 20:52:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Mar 2023 20:52:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Mar 2023 20:52:17 GMT
EXPOSE 3306 33060
# Tue, 21 Mar 2023 20:52:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ec521688c56b41126476e7ab1f7ab7305384f5b5326e80a8ba52b8d4deead22`  
		Last Modified: Tue, 21 Mar 2023 19:27:26 GMT  
		Size: 50.5 MB (50471128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f911f9b90db6be6d326471ffa9acef77985640199aca2f765be1efa82037a3d1`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38eb4fe7ed26a84c3c1f6a17d0fc831f0b7e5c43fb1ed355ff3240a813dcad61`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 983.7 KB (983706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f772a6b25f5bbd71a55ff1d40333ea8494f8281c8f386b58432036fcc96444`  
		Last Modified: Tue, 21 Mar 2023 20:52:51 GMT  
		Size: 4.6 MB (4591670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499456357ebfbc78d9408a5599908b7ded3b1d422fddf5865cdb8c8ae0fa8629`  
		Last Modified: Tue, 21 Mar 2023 20:52:50 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274f3ad0dcecde2bd838ef7f34562cbe017da4dae64469f53b48af068390d06a`  
		Last Modified: Tue, 21 Mar 2023 20:52:50 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a5b12e1de159ec628987eeb584030eb2acc6cb8025177a2a10f77e556fcc1`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 25.5 MB (25532897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0c5c82dbbc3a0e7e37dde0dd947d4401201452f147dd8f7982f6c026f3d41b`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bd281f46007c1698e833f1f602b126ba9a74db11dd4b158d61130d0edb2bcd`  
		Last Modified: Tue, 21 Mar 2023 20:52:57 GMT  
		Size: 48.4 MB (48448352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3289c4277a830488286360c722a87a8b9153b68aa6893a87fe1faf1e4018c15e`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b66f10a11fa382cf7bf501cb958d64ca12f4e236ba5f03d95028fa06421e33a`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:849a8e87076f75717e1f98102ed1545396faab1cb2c99c768bf2b5b430571604
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:2bbef75b058643f5a747c13661a88ee3301df9e25f0eaeb358587cc37da86afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162693934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88338e85f040d97b75f2d43518736f4af9e52fa4c4c577cd34b134273a079266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:50 GMT
ADD file:52316aa7d631242cd16337be337e57187ef07d3965e6284321fbdcd5b4f92b64 in / 
# Thu, 23 Mar 2023 01:30:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 11:00:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Mar 2023 11:00:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:00:28 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 11:00:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 11:00:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 11:00:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:00:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 11:00:45 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 23 Mar 2023 11:00:45 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Thu, 23 Mar 2023 11:00:46 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Mar 2023 11:01:03 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Thu, 23 Mar 2023 11:01:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 11:01:04 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 11:01:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 11:01:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:01:05 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 11:01:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3689b8de819b48387712c6d4d62d26a52a04c9e88afc68fb9d1dbe48bfa9e21d`  
		Last Modified: Thu, 23 Mar 2023 01:35:01 GMT  
		Size: 27.1 MB (27139869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ac63a14e4479941312ab4b314bbd36b8eed13e848b7446b33d62d1cf387c14`  
		Last Modified: Thu, 23 Mar 2023 11:01:59 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a94b43bbfe3822fc0a3c87da156138a81cec71bf1b9a2e00f3acc1b9819eca`  
		Last Modified: Thu, 23 Mar 2023 11:01:58 GMT  
		Size: 4.2 MB (4182339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38763e84573623aeb1cff67387112f2d0b31e5ed0b899e3b3a126770e46d8b94`  
		Last Modified: Thu, 23 Mar 2023 11:01:58 GMT  
		Size: 1.4 MB (1441745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcbc7fd4a2d7d18a737618196f4d75de0a316eaf5c125b2d4d35a7eb037426d`  
		Last Modified: Thu, 23 Mar 2023 11:01:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19764d7bd70a9eea88bec2db9d035ffe9224b9dcd7c0613e42f63b775f8f75d3`  
		Last Modified: Thu, 23 Mar 2023 11:02:00 GMT  
		Size: 14.1 MB (14086905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a2769597f7f726053839c80035384b62ea02c2f3dafa473e5200c96236b67c`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55969b3a4225bf2037f3ccfc7930ed5b0cfed7aeee036deb0d7aee144dfbc425`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4898aaf83c5d2f75aa7c90e3936fb2faf0f565889f5973fb820f1330cff028`  
		Last Modified: Thu, 23 Mar 2023 11:02:10 GMT  
		Size: 115.8 MB (115832889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9972a98a4d99007516b2303bc1ca8e06d9696adff985ac28b4f52bbb086738`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b8313553fddc90f14c25b3007f8f77459244ac46fbcd5580f9f3c31ba6a0d1`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:1780318bdabc0edd36907bf91b47632eb912e8ea91258eca3590f8aca6f54836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:59391c720d279e070440dabc9b39e478ffb310d80759ad18fa7ad61dd2ec9b7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130037432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6ee2207ee7a9ed4f5c718a507fd00dace311300153b99f6830ce34741f2f093`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Mar 2023 19:26:42 GMT
ADD file:c2562ae661b3cd914b2c0dd27aba7ee36bffbeb92415b7b80c111a5d563d07ed in / 
# Tue, 21 Mar 2023 19:26:43 GMT
CMD ["/bin/bash"]
# Tue, 21 Mar 2023 20:51:10 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 21 Mar 2023 20:51:10 GMT
ENV GOSU_VERSION=1.16
# Tue, 21 Mar 2023 20:51:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Mar 2023 20:51:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Tue, 21 Mar 2023 20:51:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 21 Mar 2023 20:51:32 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 21 Mar 2023 20:51:32 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Tue, 21 Mar 2023 20:51:32 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 21 Mar 2023 20:51:51 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 21 Mar 2023 20:51:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 21 Mar 2023 20:51:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Tue, 21 Mar 2023 20:52:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 21 Mar 2023 20:52:16 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Mar 2023 20:52:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 21 Mar 2023 20:52:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Mar 2023 20:52:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Mar 2023 20:52:17 GMT
EXPOSE 3306 33060
# Tue, 21 Mar 2023 20:52:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ec521688c56b41126476e7ab1f7ab7305384f5b5326e80a8ba52b8d4deead22`  
		Last Modified: Tue, 21 Mar 2023 19:27:26 GMT  
		Size: 50.5 MB (50471128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f911f9b90db6be6d326471ffa9acef77985640199aca2f765be1efa82037a3d1`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38eb4fe7ed26a84c3c1f6a17d0fc831f0b7e5c43fb1ed355ff3240a813dcad61`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 983.7 KB (983706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f772a6b25f5bbd71a55ff1d40333ea8494f8281c8f386b58432036fcc96444`  
		Last Modified: Tue, 21 Mar 2023 20:52:51 GMT  
		Size: 4.6 MB (4591670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499456357ebfbc78d9408a5599908b7ded3b1d422fddf5865cdb8c8ae0fa8629`  
		Last Modified: Tue, 21 Mar 2023 20:52:50 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274f3ad0dcecde2bd838ef7f34562cbe017da4dae64469f53b48af068390d06a`  
		Last Modified: Tue, 21 Mar 2023 20:52:50 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a5b12e1de159ec628987eeb584030eb2acc6cb8025177a2a10f77e556fcc1`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 25.5 MB (25532897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0c5c82dbbc3a0e7e37dde0dd947d4401201452f147dd8f7982f6c026f3d41b`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bd281f46007c1698e833f1f602b126ba9a74db11dd4b158d61130d0edb2bcd`  
		Last Modified: Tue, 21 Mar 2023 20:52:57 GMT  
		Size: 48.4 MB (48448352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3289c4277a830488286360c722a87a8b9153b68aa6893a87fe1faf1e4018c15e`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b66f10a11fa382cf7bf501cb958d64ca12f4e236ba5f03d95028fa06421e33a`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.41`

```console
$ docker pull mysql@sha256:1780318bdabc0edd36907bf91b47632eb912e8ea91258eca3590f8aca6f54836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.41` - linux; amd64

```console
$ docker pull mysql@sha256:59391c720d279e070440dabc9b39e478ffb310d80759ad18fa7ad61dd2ec9b7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130037432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6ee2207ee7a9ed4f5c718a507fd00dace311300153b99f6830ce34741f2f093`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Mar 2023 19:26:42 GMT
ADD file:c2562ae661b3cd914b2c0dd27aba7ee36bffbeb92415b7b80c111a5d563d07ed in / 
# Tue, 21 Mar 2023 19:26:43 GMT
CMD ["/bin/bash"]
# Tue, 21 Mar 2023 20:51:10 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 21 Mar 2023 20:51:10 GMT
ENV GOSU_VERSION=1.16
# Tue, 21 Mar 2023 20:51:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Mar 2023 20:51:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Tue, 21 Mar 2023 20:51:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 21 Mar 2023 20:51:32 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 21 Mar 2023 20:51:32 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Tue, 21 Mar 2023 20:51:32 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 21 Mar 2023 20:51:51 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 21 Mar 2023 20:51:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 21 Mar 2023 20:51:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Tue, 21 Mar 2023 20:52:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 21 Mar 2023 20:52:16 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Mar 2023 20:52:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 21 Mar 2023 20:52:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Mar 2023 20:52:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Mar 2023 20:52:17 GMT
EXPOSE 3306 33060
# Tue, 21 Mar 2023 20:52:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ec521688c56b41126476e7ab1f7ab7305384f5b5326e80a8ba52b8d4deead22`  
		Last Modified: Tue, 21 Mar 2023 19:27:26 GMT  
		Size: 50.5 MB (50471128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f911f9b90db6be6d326471ffa9acef77985640199aca2f765be1efa82037a3d1`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38eb4fe7ed26a84c3c1f6a17d0fc831f0b7e5c43fb1ed355ff3240a813dcad61`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 983.7 KB (983706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f772a6b25f5bbd71a55ff1d40333ea8494f8281c8f386b58432036fcc96444`  
		Last Modified: Tue, 21 Mar 2023 20:52:51 GMT  
		Size: 4.6 MB (4591670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499456357ebfbc78d9408a5599908b7ded3b1d422fddf5865cdb8c8ae0fa8629`  
		Last Modified: Tue, 21 Mar 2023 20:52:50 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274f3ad0dcecde2bd838ef7f34562cbe017da4dae64469f53b48af068390d06a`  
		Last Modified: Tue, 21 Mar 2023 20:52:50 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a5b12e1de159ec628987eeb584030eb2acc6cb8025177a2a10f77e556fcc1`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 25.5 MB (25532897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0c5c82dbbc3a0e7e37dde0dd947d4401201452f147dd8f7982f6c026f3d41b`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bd281f46007c1698e833f1f602b126ba9a74db11dd4b158d61130d0edb2bcd`  
		Last Modified: Tue, 21 Mar 2023 20:52:57 GMT  
		Size: 48.4 MB (48448352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3289c4277a830488286360c722a87a8b9153b68aa6893a87fe1faf1e4018c15e`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b66f10a11fa382cf7bf501cb958d64ca12f4e236ba5f03d95028fa06421e33a`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.41-debian`

```console
$ docker pull mysql@sha256:849a8e87076f75717e1f98102ed1545396faab1cb2c99c768bf2b5b430571604
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.41-debian` - linux; amd64

```console
$ docker pull mysql@sha256:2bbef75b058643f5a747c13661a88ee3301df9e25f0eaeb358587cc37da86afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162693934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88338e85f040d97b75f2d43518736f4af9e52fa4c4c577cd34b134273a079266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:50 GMT
ADD file:52316aa7d631242cd16337be337e57187ef07d3965e6284321fbdcd5b4f92b64 in / 
# Thu, 23 Mar 2023 01:30:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 11:00:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Mar 2023 11:00:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:00:28 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 11:00:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 11:00:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 11:00:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:00:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 11:00:45 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 23 Mar 2023 11:00:45 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Thu, 23 Mar 2023 11:00:46 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Mar 2023 11:01:03 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Thu, 23 Mar 2023 11:01:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 11:01:04 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 11:01:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 11:01:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:01:05 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 11:01:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3689b8de819b48387712c6d4d62d26a52a04c9e88afc68fb9d1dbe48bfa9e21d`  
		Last Modified: Thu, 23 Mar 2023 01:35:01 GMT  
		Size: 27.1 MB (27139869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ac63a14e4479941312ab4b314bbd36b8eed13e848b7446b33d62d1cf387c14`  
		Last Modified: Thu, 23 Mar 2023 11:01:59 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a94b43bbfe3822fc0a3c87da156138a81cec71bf1b9a2e00f3acc1b9819eca`  
		Last Modified: Thu, 23 Mar 2023 11:01:58 GMT  
		Size: 4.2 MB (4182339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38763e84573623aeb1cff67387112f2d0b31e5ed0b899e3b3a126770e46d8b94`  
		Last Modified: Thu, 23 Mar 2023 11:01:58 GMT  
		Size: 1.4 MB (1441745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcbc7fd4a2d7d18a737618196f4d75de0a316eaf5c125b2d4d35a7eb037426d`  
		Last Modified: Thu, 23 Mar 2023 11:01:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19764d7bd70a9eea88bec2db9d035ffe9224b9dcd7c0613e42f63b775f8f75d3`  
		Last Modified: Thu, 23 Mar 2023 11:02:00 GMT  
		Size: 14.1 MB (14086905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a2769597f7f726053839c80035384b62ea02c2f3dafa473e5200c96236b67c`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55969b3a4225bf2037f3ccfc7930ed5b0cfed7aeee036deb0d7aee144dfbc425`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4898aaf83c5d2f75aa7c90e3936fb2faf0f565889f5973fb820f1330cff028`  
		Last Modified: Thu, 23 Mar 2023 11:02:10 GMT  
		Size: 115.8 MB (115832889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9972a98a4d99007516b2303bc1ca8e06d9696adff985ac28b4f52bbb086738`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b8313553fddc90f14c25b3007f8f77459244ac46fbcd5580f9f3c31ba6a0d1`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.41-oracle`

```console
$ docker pull mysql@sha256:1780318bdabc0edd36907bf91b47632eb912e8ea91258eca3590f8aca6f54836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.41-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:59391c720d279e070440dabc9b39e478ffb310d80759ad18fa7ad61dd2ec9b7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130037432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6ee2207ee7a9ed4f5c718a507fd00dace311300153b99f6830ce34741f2f093`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Mar 2023 19:26:42 GMT
ADD file:c2562ae661b3cd914b2c0dd27aba7ee36bffbeb92415b7b80c111a5d563d07ed in / 
# Tue, 21 Mar 2023 19:26:43 GMT
CMD ["/bin/bash"]
# Tue, 21 Mar 2023 20:51:10 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 21 Mar 2023 20:51:10 GMT
ENV GOSU_VERSION=1.16
# Tue, 21 Mar 2023 20:51:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Mar 2023 20:51:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Tue, 21 Mar 2023 20:51:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 21 Mar 2023 20:51:32 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 21 Mar 2023 20:51:32 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Tue, 21 Mar 2023 20:51:32 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 21 Mar 2023 20:51:51 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 21 Mar 2023 20:51:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 21 Mar 2023 20:51:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Tue, 21 Mar 2023 20:52:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 21 Mar 2023 20:52:16 GMT
VOLUME [/var/lib/mysql]
# Tue, 21 Mar 2023 20:52:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 21 Mar 2023 20:52:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 21 Mar 2023 20:52:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Mar 2023 20:52:17 GMT
EXPOSE 3306 33060
# Tue, 21 Mar 2023 20:52:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ec521688c56b41126476e7ab1f7ab7305384f5b5326e80a8ba52b8d4deead22`  
		Last Modified: Tue, 21 Mar 2023 19:27:26 GMT  
		Size: 50.5 MB (50471128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f911f9b90db6be6d326471ffa9acef77985640199aca2f765be1efa82037a3d1`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38eb4fe7ed26a84c3c1f6a17d0fc831f0b7e5c43fb1ed355ff3240a813dcad61`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 983.7 KB (983706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f772a6b25f5bbd71a55ff1d40333ea8494f8281c8f386b58432036fcc96444`  
		Last Modified: Tue, 21 Mar 2023 20:52:51 GMT  
		Size: 4.6 MB (4591670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499456357ebfbc78d9408a5599908b7ded3b1d422fddf5865cdb8c8ae0fa8629`  
		Last Modified: Tue, 21 Mar 2023 20:52:50 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274f3ad0dcecde2bd838ef7f34562cbe017da4dae64469f53b48af068390d06a`  
		Last Modified: Tue, 21 Mar 2023 20:52:50 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a5b12e1de159ec628987eeb584030eb2acc6cb8025177a2a10f77e556fcc1`  
		Last Modified: Tue, 21 Mar 2023 20:52:52 GMT  
		Size: 25.5 MB (25532897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0c5c82dbbc3a0e7e37dde0dd947d4401201452f147dd8f7982f6c026f3d41b`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bd281f46007c1698e833f1f602b126ba9a74db11dd4b158d61130d0edb2bcd`  
		Last Modified: Tue, 21 Mar 2023 20:52:57 GMT  
		Size: 48.4 MB (48448352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3289c4277a830488286360c722a87a8b9153b68aa6893a87fe1faf1e4018c15e`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b66f10a11fa382cf7bf501cb958d64ca12f4e236ba5f03d95028fa06421e33a`  
		Last Modified: Tue, 21 Mar 2023 20:52:48 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:ca114710bb35b862062fd51733a7dba1ba3e93be33e4eede442b0ce15c77b718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:1b5c4f72bfc2f2cc8c8fea93b277e871acac9bc421f4587ae499a074a4fefacd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156576131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a8bc460a9b517dd0230cc3d475ce0a9b9e1744e7959bb538f5572ec88139f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:20 GMT
ADD file:1a06059b1a097ecc61cb02965fc90e00183a8653d9ae009965823226559c5be9 in / 
# Wed, 22 Mar 2023 23:55:20 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:17:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:17:18 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:17:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:17:46 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:17:47 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:17:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:18:18 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:18:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:18:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:18:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:18:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:18:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:18:55 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:18:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab8798141d463c224f18fa5dd1d249b554dda61be24da7aa516e4e2de324db76`  
		Last Modified: Wed, 22 Mar 2023 23:56:08 GMT  
		Size: 44.6 MB (44563376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75508f0dccd76c48588532e73fcc39ecd235b6f8349c658ba4e10c863a95c076`  
		Last Modified: Thu, 23 Mar 2023 00:19:30 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1f5f86172459ac9f263a8f049036d17a9f59f8762f2222a0c0ba7d7e7e348`  
		Last Modified: Thu, 23 Mar 2023 00:19:31 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccc774632f39a5557e6005f85d9b32ad162c0a91eb4f0eb6b78c1b52a1a131d`  
		Last Modified: Thu, 23 Mar 2023 00:19:29 GMT  
		Size: 4.6 MB (4612146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7d864905655742ad222a835ff4edaaa87c0995bef926a3596448dd3c66bac0`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32480f1416f753cf219ff7c80cdeb4b0b5ae742e52c160d74ed4f13ebda5c807`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b89229d2472b456f860ad13a7aebade35883a35acb83e049382895768a103a9`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 56.2 MB (56223601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229bb5ff022d1021b28bf0f791baba9c05b2f635576dcd7c0d2da25431fd972b`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972d41dd67e3a7011a276a60717261d023296077f39afe611dead60c4445ffd`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 50.2 MB (50184513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8283d390a92ef33392ce41d164da7cfb4b36e714d72d81548f5ca5be222eba7`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddba158ba54022083e4b58c97b21cbd5580ba227e949f25a492efedd098321b9`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:657baef4941da52684daf5c048e1a12fb67966b0f78b24ece03f176f2ecee634
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155443156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996fa9077f757f6a87943dd5d5fff378cb0448baad30e625d7bdb4b8ce71df77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:59:36 GMT
ADD file:b4a46acde2a8ffdb8874f11aadcfc90177b15422278a1b8fa87e7ed9c97cf2a4 in / 
# Wed, 22 Mar 2023 23:59:36 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:20:19 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:20:19 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:20:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:20:45 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:20:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:20:47 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:21:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:21:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:21:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:21:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:21:47 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:21:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:21:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:21:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:21:47 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:21:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:40ffb7074955cd4f083dfcadee0a1ef1e12dbe031bdf2325c8bae38711b1f70f`  
		Last Modified: Thu, 23 Mar 2023 00:00:22 GMT  
		Size: 43.5 MB (43460037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2447ceb7b2b15bbd81959c0472744d693ef3bd26dc3fcd72bc4feae2981c674`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90547588960ca61c5b858a871ec898e2132d3e726e02927788839ac44f7e8b2`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989c2ac214cf31e965acd6a00e4861ba362bdad21503fadb60edf497db4f3e98`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 4.5 MB (4468367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaccc20c24ae65eeabb4e5b8131ab3cbd9f6ddb85787b14adf4281ea6d51bb2`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18556b046cb247ac0c905f09cc10ab904a995c40af90e027592ed97b3247479e`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05489c77c7a7d715a7fc0003c17ba0eb1c6cec38d5db1e82dd8fc82b626ae2b`  
		Last Modified: Thu, 23 Mar 2023 00:22:10 GMT  
		Size: 55.6 MB (55602642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98130d34badf6c2c91c251c423385532971d92717c0213e03919d7398ceb8db5`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd0424f0a2cde2a4d2f36980987bb8a699c2baf12ce7fdac586f7b13c3f79e4`  
		Last Modified: Thu, 23 Mar 2023 00:22:11 GMT  
		Size: 51.0 MB (50989444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77021328e41962d496870a28b8bf00d6877368c5338ed48fbc35f7cf828f8780`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3590288009eb3bfc73b08757208574ee742d8b4b1f8a6fb1083584c036caf`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:01003f288c58133dad270905e2768e6a1d399d709a4a1375bc4f982f747252c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:38d6c177f28baa3b93350a59f0aae2c032418f05e2efd979c9da22d0a27d6223
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177766595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e8288d09e99593d17141361840c289947140d8e35f633ddeba0fab989abe3eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 10:59:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Mar 2023 10:59:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:59:38 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 10:59:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 10:59:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 10:59:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:59:55 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 10:59:55 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 10:59:55 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Thu, 23 Mar 2023 10:59:55 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Mar 2023 11:00:09 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Thu, 23 Mar 2023 11:00:10 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 11:00:10 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Thu, 23 Mar 2023 11:00:10 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 11:00:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 11:00:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:00:11 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 11:00:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6521829aee0429164fc3f7c547e84502400c78acde7a204473309a69c42de3`  
		Last Modified: Thu, 23 Mar 2023 11:01:26 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9f91eb302bb05cb9afddd1700b2642fd6618c437d04f4185f607b6328a96b4`  
		Last Modified: Thu, 23 Mar 2023 11:01:27 GMT  
		Size: 4.4 MB (4414934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13030349449a434afe037605a64bb8d3a329f038982cfc259d41614e5e07f9e6`  
		Last Modified: Thu, 23 Mar 2023 11:01:24 GMT  
		Size: 1.5 MB (1471385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c2b6b8463df89c8f2a6360c2f660aeaecfc6af04623b90c8672633b45508cf`  
		Last Modified: Thu, 23 Mar 2023 11:01:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c28230983db4101bc642c49ad9db328e79021f759b015452312fee84088bfd`  
		Last Modified: Thu, 23 Mar 2023 11:01:26 GMT  
		Size: 12.7 MB (12661950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d22d367ac2dbd2c3b82ae8b262419d0f4c0d52a347e70aec590b2ea0e3706d5`  
		Last Modified: Thu, 23 Mar 2023 11:01:24 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2bb5025fa157b775e71b1d4f2cdecd14b2d34b980f991ae86b50d0774057da`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e14277cdd802f47544aaa9a804c183ddef124757546b539b7c0f09379805728`  
		Last Modified: Thu, 23 Mar 2023 11:01:40 GMT  
		Size: 127.8 MB (127795886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a14127bf2fafa4308b78730e859d21a1d282b9508753a915c77fb970028891f`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed869d4966e891b12c705ddc7bb0f1f6cdb851ae2fc9106a46778f4c5f568ec7`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40298f9476557edea1f63b547f12e3a6814b8b110333bc90760d9363f86d8383`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:ca114710bb35b862062fd51733a7dba1ba3e93be33e4eede442b0ce15c77b718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1b5c4f72bfc2f2cc8c8fea93b277e871acac9bc421f4587ae499a074a4fefacd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156576131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a8bc460a9b517dd0230cc3d475ce0a9b9e1744e7959bb538f5572ec88139f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:20 GMT
ADD file:1a06059b1a097ecc61cb02965fc90e00183a8653d9ae009965823226559c5be9 in / 
# Wed, 22 Mar 2023 23:55:20 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:17:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:17:18 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:17:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:17:46 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:17:47 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:17:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:18:18 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:18:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:18:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:18:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:18:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:18:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:18:55 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:18:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab8798141d463c224f18fa5dd1d249b554dda61be24da7aa516e4e2de324db76`  
		Last Modified: Wed, 22 Mar 2023 23:56:08 GMT  
		Size: 44.6 MB (44563376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75508f0dccd76c48588532e73fcc39ecd235b6f8349c658ba4e10c863a95c076`  
		Last Modified: Thu, 23 Mar 2023 00:19:30 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1f5f86172459ac9f263a8f049036d17a9f59f8762f2222a0c0ba7d7e7e348`  
		Last Modified: Thu, 23 Mar 2023 00:19:31 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccc774632f39a5557e6005f85d9b32ad162c0a91eb4f0eb6b78c1b52a1a131d`  
		Last Modified: Thu, 23 Mar 2023 00:19:29 GMT  
		Size: 4.6 MB (4612146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7d864905655742ad222a835ff4edaaa87c0995bef926a3596448dd3c66bac0`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32480f1416f753cf219ff7c80cdeb4b0b5ae742e52c160d74ed4f13ebda5c807`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b89229d2472b456f860ad13a7aebade35883a35acb83e049382895768a103a9`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 56.2 MB (56223601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229bb5ff022d1021b28bf0f791baba9c05b2f635576dcd7c0d2da25431fd972b`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972d41dd67e3a7011a276a60717261d023296077f39afe611dead60c4445ffd`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 50.2 MB (50184513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8283d390a92ef33392ce41d164da7cfb4b36e714d72d81548f5ca5be222eba7`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddba158ba54022083e4b58c97b21cbd5580ba227e949f25a492efedd098321b9`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:657baef4941da52684daf5c048e1a12fb67966b0f78b24ece03f176f2ecee634
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155443156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996fa9077f757f6a87943dd5d5fff378cb0448baad30e625d7bdb4b8ce71df77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:59:36 GMT
ADD file:b4a46acde2a8ffdb8874f11aadcfc90177b15422278a1b8fa87e7ed9c97cf2a4 in / 
# Wed, 22 Mar 2023 23:59:36 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:20:19 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:20:19 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:20:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:20:45 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:20:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:20:47 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:21:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:21:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:21:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:21:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:21:47 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:21:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:21:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:21:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:21:47 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:21:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:40ffb7074955cd4f083dfcadee0a1ef1e12dbe031bdf2325c8bae38711b1f70f`  
		Last Modified: Thu, 23 Mar 2023 00:00:22 GMT  
		Size: 43.5 MB (43460037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2447ceb7b2b15bbd81959c0472744d693ef3bd26dc3fcd72bc4feae2981c674`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90547588960ca61c5b858a871ec898e2132d3e726e02927788839ac44f7e8b2`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989c2ac214cf31e965acd6a00e4861ba362bdad21503fadb60edf497db4f3e98`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 4.5 MB (4468367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaccc20c24ae65eeabb4e5b8131ab3cbd9f6ddb85787b14adf4281ea6d51bb2`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18556b046cb247ac0c905f09cc10ab904a995c40af90e027592ed97b3247479e`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05489c77c7a7d715a7fc0003c17ba0eb1c6cec38d5db1e82dd8fc82b626ae2b`  
		Last Modified: Thu, 23 Mar 2023 00:22:10 GMT  
		Size: 55.6 MB (55602642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98130d34badf6c2c91c251c423385532971d92717c0213e03919d7398ceb8db5`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd0424f0a2cde2a4d2f36980987bb8a699c2baf12ce7fdac586f7b13c3f79e4`  
		Last Modified: Thu, 23 Mar 2023 00:22:11 GMT  
		Size: 51.0 MB (50989444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77021328e41962d496870a28b8bf00d6877368c5338ed48fbc35f7cf828f8780`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3590288009eb3bfc73b08757208574ee742d8b4b1f8a6fb1083584c036caf`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:ca114710bb35b862062fd51733a7dba1ba3e93be33e4eede442b0ce15c77b718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:1b5c4f72bfc2f2cc8c8fea93b277e871acac9bc421f4587ae499a074a4fefacd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156576131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a8bc460a9b517dd0230cc3d475ce0a9b9e1744e7959bb538f5572ec88139f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:20 GMT
ADD file:1a06059b1a097ecc61cb02965fc90e00183a8653d9ae009965823226559c5be9 in / 
# Wed, 22 Mar 2023 23:55:20 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:17:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:17:18 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:17:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:17:46 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:17:47 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:17:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:18:18 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:18:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:18:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:18:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:18:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:18:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:18:55 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:18:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab8798141d463c224f18fa5dd1d249b554dda61be24da7aa516e4e2de324db76`  
		Last Modified: Wed, 22 Mar 2023 23:56:08 GMT  
		Size: 44.6 MB (44563376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75508f0dccd76c48588532e73fcc39ecd235b6f8349c658ba4e10c863a95c076`  
		Last Modified: Thu, 23 Mar 2023 00:19:30 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1f5f86172459ac9f263a8f049036d17a9f59f8762f2222a0c0ba7d7e7e348`  
		Last Modified: Thu, 23 Mar 2023 00:19:31 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccc774632f39a5557e6005f85d9b32ad162c0a91eb4f0eb6b78c1b52a1a131d`  
		Last Modified: Thu, 23 Mar 2023 00:19:29 GMT  
		Size: 4.6 MB (4612146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7d864905655742ad222a835ff4edaaa87c0995bef926a3596448dd3c66bac0`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32480f1416f753cf219ff7c80cdeb4b0b5ae742e52c160d74ed4f13ebda5c807`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b89229d2472b456f860ad13a7aebade35883a35acb83e049382895768a103a9`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 56.2 MB (56223601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229bb5ff022d1021b28bf0f791baba9c05b2f635576dcd7c0d2da25431fd972b`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972d41dd67e3a7011a276a60717261d023296077f39afe611dead60c4445ffd`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 50.2 MB (50184513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8283d390a92ef33392ce41d164da7cfb4b36e714d72d81548f5ca5be222eba7`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddba158ba54022083e4b58c97b21cbd5580ba227e949f25a492efedd098321b9`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:657baef4941da52684daf5c048e1a12fb67966b0f78b24ece03f176f2ecee634
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155443156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996fa9077f757f6a87943dd5d5fff378cb0448baad30e625d7bdb4b8ce71df77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:59:36 GMT
ADD file:b4a46acde2a8ffdb8874f11aadcfc90177b15422278a1b8fa87e7ed9c97cf2a4 in / 
# Wed, 22 Mar 2023 23:59:36 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:20:19 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:20:19 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:20:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:20:45 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:20:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:20:47 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:21:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:21:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:21:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:21:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:21:47 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:21:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:21:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:21:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:21:47 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:21:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:40ffb7074955cd4f083dfcadee0a1ef1e12dbe031bdf2325c8bae38711b1f70f`  
		Last Modified: Thu, 23 Mar 2023 00:00:22 GMT  
		Size: 43.5 MB (43460037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2447ceb7b2b15bbd81959c0472744d693ef3bd26dc3fcd72bc4feae2981c674`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90547588960ca61c5b858a871ec898e2132d3e726e02927788839ac44f7e8b2`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989c2ac214cf31e965acd6a00e4861ba362bdad21503fadb60edf497db4f3e98`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 4.5 MB (4468367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaccc20c24ae65eeabb4e5b8131ab3cbd9f6ddb85787b14adf4281ea6d51bb2`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18556b046cb247ac0c905f09cc10ab904a995c40af90e027592ed97b3247479e`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05489c77c7a7d715a7fc0003c17ba0eb1c6cec38d5db1e82dd8fc82b626ae2b`  
		Last Modified: Thu, 23 Mar 2023 00:22:10 GMT  
		Size: 55.6 MB (55602642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98130d34badf6c2c91c251c423385532971d92717c0213e03919d7398ceb8db5`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd0424f0a2cde2a4d2f36980987bb8a699c2baf12ce7fdac586f7b13c3f79e4`  
		Last Modified: Thu, 23 Mar 2023 00:22:11 GMT  
		Size: 51.0 MB (50989444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77021328e41962d496870a28b8bf00d6877368c5338ed48fbc35f7cf828f8780`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3590288009eb3bfc73b08757208574ee742d8b4b1f8a6fb1083584c036caf`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:01003f288c58133dad270905e2768e6a1d399d709a4a1375bc4f982f747252c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:38d6c177f28baa3b93350a59f0aae2c032418f05e2efd979c9da22d0a27d6223
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177766595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e8288d09e99593d17141361840c289947140d8e35f633ddeba0fab989abe3eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 10:59:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Mar 2023 10:59:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:59:38 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 10:59:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 10:59:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 10:59:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:59:55 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 10:59:55 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 10:59:55 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Thu, 23 Mar 2023 10:59:55 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Mar 2023 11:00:09 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Thu, 23 Mar 2023 11:00:10 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 11:00:10 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Thu, 23 Mar 2023 11:00:10 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 11:00:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 11:00:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:00:11 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 11:00:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6521829aee0429164fc3f7c547e84502400c78acde7a204473309a69c42de3`  
		Last Modified: Thu, 23 Mar 2023 11:01:26 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9f91eb302bb05cb9afddd1700b2642fd6618c437d04f4185f607b6328a96b4`  
		Last Modified: Thu, 23 Mar 2023 11:01:27 GMT  
		Size: 4.4 MB (4414934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13030349449a434afe037605a64bb8d3a329f038982cfc259d41614e5e07f9e6`  
		Last Modified: Thu, 23 Mar 2023 11:01:24 GMT  
		Size: 1.5 MB (1471385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c2b6b8463df89c8f2a6360c2f660aeaecfc6af04623b90c8672633b45508cf`  
		Last Modified: Thu, 23 Mar 2023 11:01:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c28230983db4101bc642c49ad9db328e79021f759b015452312fee84088bfd`  
		Last Modified: Thu, 23 Mar 2023 11:01:26 GMT  
		Size: 12.7 MB (12661950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d22d367ac2dbd2c3b82ae8b262419d0f4c0d52a347e70aec590b2ea0e3706d5`  
		Last Modified: Thu, 23 Mar 2023 11:01:24 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2bb5025fa157b775e71b1d4f2cdecd14b2d34b980f991ae86b50d0774057da`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e14277cdd802f47544aaa9a804c183ddef124757546b539b7c0f09379805728`  
		Last Modified: Thu, 23 Mar 2023 11:01:40 GMT  
		Size: 127.8 MB (127795886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a14127bf2fafa4308b78730e859d21a1d282b9508753a915c77fb970028891f`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed869d4966e891b12c705ddc7bb0f1f6cdb851ae2fc9106a46778f4c5f568ec7`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40298f9476557edea1f63b547f12e3a6814b8b110333bc90760d9363f86d8383`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:ca114710bb35b862062fd51733a7dba1ba3e93be33e4eede442b0ce15c77b718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1b5c4f72bfc2f2cc8c8fea93b277e871acac9bc421f4587ae499a074a4fefacd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156576131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a8bc460a9b517dd0230cc3d475ce0a9b9e1744e7959bb538f5572ec88139f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:20 GMT
ADD file:1a06059b1a097ecc61cb02965fc90e00183a8653d9ae009965823226559c5be9 in / 
# Wed, 22 Mar 2023 23:55:20 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:17:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:17:18 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:17:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:17:46 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:17:47 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:17:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:18:18 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:18:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:18:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:18:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:18:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:18:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:18:55 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:18:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab8798141d463c224f18fa5dd1d249b554dda61be24da7aa516e4e2de324db76`  
		Last Modified: Wed, 22 Mar 2023 23:56:08 GMT  
		Size: 44.6 MB (44563376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75508f0dccd76c48588532e73fcc39ecd235b6f8349c658ba4e10c863a95c076`  
		Last Modified: Thu, 23 Mar 2023 00:19:30 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1f5f86172459ac9f263a8f049036d17a9f59f8762f2222a0c0ba7d7e7e348`  
		Last Modified: Thu, 23 Mar 2023 00:19:31 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccc774632f39a5557e6005f85d9b32ad162c0a91eb4f0eb6b78c1b52a1a131d`  
		Last Modified: Thu, 23 Mar 2023 00:19:29 GMT  
		Size: 4.6 MB (4612146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7d864905655742ad222a835ff4edaaa87c0995bef926a3596448dd3c66bac0`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32480f1416f753cf219ff7c80cdeb4b0b5ae742e52c160d74ed4f13ebda5c807`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b89229d2472b456f860ad13a7aebade35883a35acb83e049382895768a103a9`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 56.2 MB (56223601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229bb5ff022d1021b28bf0f791baba9c05b2f635576dcd7c0d2da25431fd972b`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972d41dd67e3a7011a276a60717261d023296077f39afe611dead60c4445ffd`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 50.2 MB (50184513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8283d390a92ef33392ce41d164da7cfb4b36e714d72d81548f5ca5be222eba7`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddba158ba54022083e4b58c97b21cbd5580ba227e949f25a492efedd098321b9`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:657baef4941da52684daf5c048e1a12fb67966b0f78b24ece03f176f2ecee634
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155443156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996fa9077f757f6a87943dd5d5fff378cb0448baad30e625d7bdb4b8ce71df77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:59:36 GMT
ADD file:b4a46acde2a8ffdb8874f11aadcfc90177b15422278a1b8fa87e7ed9c97cf2a4 in / 
# Wed, 22 Mar 2023 23:59:36 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:20:19 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:20:19 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:20:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:20:45 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:20:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:20:47 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:21:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:21:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:21:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:21:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:21:47 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:21:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:21:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:21:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:21:47 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:21:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:40ffb7074955cd4f083dfcadee0a1ef1e12dbe031bdf2325c8bae38711b1f70f`  
		Last Modified: Thu, 23 Mar 2023 00:00:22 GMT  
		Size: 43.5 MB (43460037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2447ceb7b2b15bbd81959c0472744d693ef3bd26dc3fcd72bc4feae2981c674`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90547588960ca61c5b858a871ec898e2132d3e726e02927788839ac44f7e8b2`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989c2ac214cf31e965acd6a00e4861ba362bdad21503fadb60edf497db4f3e98`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 4.5 MB (4468367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaccc20c24ae65eeabb4e5b8131ab3cbd9f6ddb85787b14adf4281ea6d51bb2`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18556b046cb247ac0c905f09cc10ab904a995c40af90e027592ed97b3247479e`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05489c77c7a7d715a7fc0003c17ba0eb1c6cec38d5db1e82dd8fc82b626ae2b`  
		Last Modified: Thu, 23 Mar 2023 00:22:10 GMT  
		Size: 55.6 MB (55602642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98130d34badf6c2c91c251c423385532971d92717c0213e03919d7398ceb8db5`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd0424f0a2cde2a4d2f36980987bb8a699c2baf12ce7fdac586f7b13c3f79e4`  
		Last Modified: Thu, 23 Mar 2023 00:22:11 GMT  
		Size: 51.0 MB (50989444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77021328e41962d496870a28b8bf00d6877368c5338ed48fbc35f7cf828f8780`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3590288009eb3bfc73b08757208574ee742d8b4b1f8a6fb1083584c036caf`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.32`

```console
$ docker pull mysql@sha256:ca114710bb35b862062fd51733a7dba1ba3e93be33e4eede442b0ce15c77b718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.32` - linux; amd64

```console
$ docker pull mysql@sha256:1b5c4f72bfc2f2cc8c8fea93b277e871acac9bc421f4587ae499a074a4fefacd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156576131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a8bc460a9b517dd0230cc3d475ce0a9b9e1744e7959bb538f5572ec88139f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:20 GMT
ADD file:1a06059b1a097ecc61cb02965fc90e00183a8653d9ae009965823226559c5be9 in / 
# Wed, 22 Mar 2023 23:55:20 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:17:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:17:18 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:17:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:17:46 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:17:47 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:17:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:18:18 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:18:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:18:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:18:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:18:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:18:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:18:55 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:18:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab8798141d463c224f18fa5dd1d249b554dda61be24da7aa516e4e2de324db76`  
		Last Modified: Wed, 22 Mar 2023 23:56:08 GMT  
		Size: 44.6 MB (44563376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75508f0dccd76c48588532e73fcc39ecd235b6f8349c658ba4e10c863a95c076`  
		Last Modified: Thu, 23 Mar 2023 00:19:30 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1f5f86172459ac9f263a8f049036d17a9f59f8762f2222a0c0ba7d7e7e348`  
		Last Modified: Thu, 23 Mar 2023 00:19:31 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccc774632f39a5557e6005f85d9b32ad162c0a91eb4f0eb6b78c1b52a1a131d`  
		Last Modified: Thu, 23 Mar 2023 00:19:29 GMT  
		Size: 4.6 MB (4612146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7d864905655742ad222a835ff4edaaa87c0995bef926a3596448dd3c66bac0`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32480f1416f753cf219ff7c80cdeb4b0b5ae742e52c160d74ed4f13ebda5c807`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b89229d2472b456f860ad13a7aebade35883a35acb83e049382895768a103a9`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 56.2 MB (56223601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229bb5ff022d1021b28bf0f791baba9c05b2f635576dcd7c0d2da25431fd972b`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972d41dd67e3a7011a276a60717261d023296077f39afe611dead60c4445ffd`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 50.2 MB (50184513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8283d390a92ef33392ce41d164da7cfb4b36e714d72d81548f5ca5be222eba7`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddba158ba54022083e4b58c97b21cbd5580ba227e949f25a492efedd098321b9`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.32` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:657baef4941da52684daf5c048e1a12fb67966b0f78b24ece03f176f2ecee634
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155443156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996fa9077f757f6a87943dd5d5fff378cb0448baad30e625d7bdb4b8ce71df77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:59:36 GMT
ADD file:b4a46acde2a8ffdb8874f11aadcfc90177b15422278a1b8fa87e7ed9c97cf2a4 in / 
# Wed, 22 Mar 2023 23:59:36 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:20:19 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:20:19 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:20:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:20:45 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:20:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:20:47 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:21:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:21:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:21:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:21:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:21:47 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:21:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:21:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:21:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:21:47 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:21:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:40ffb7074955cd4f083dfcadee0a1ef1e12dbe031bdf2325c8bae38711b1f70f`  
		Last Modified: Thu, 23 Mar 2023 00:00:22 GMT  
		Size: 43.5 MB (43460037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2447ceb7b2b15bbd81959c0472744d693ef3bd26dc3fcd72bc4feae2981c674`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90547588960ca61c5b858a871ec898e2132d3e726e02927788839ac44f7e8b2`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989c2ac214cf31e965acd6a00e4861ba362bdad21503fadb60edf497db4f3e98`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 4.5 MB (4468367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaccc20c24ae65eeabb4e5b8131ab3cbd9f6ddb85787b14adf4281ea6d51bb2`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18556b046cb247ac0c905f09cc10ab904a995c40af90e027592ed97b3247479e`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05489c77c7a7d715a7fc0003c17ba0eb1c6cec38d5db1e82dd8fc82b626ae2b`  
		Last Modified: Thu, 23 Mar 2023 00:22:10 GMT  
		Size: 55.6 MB (55602642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98130d34badf6c2c91c251c423385532971d92717c0213e03919d7398ceb8db5`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd0424f0a2cde2a4d2f36980987bb8a699c2baf12ce7fdac586f7b13c3f79e4`  
		Last Modified: Thu, 23 Mar 2023 00:22:11 GMT  
		Size: 51.0 MB (50989444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77021328e41962d496870a28b8bf00d6877368c5338ed48fbc35f7cf828f8780`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3590288009eb3bfc73b08757208574ee742d8b4b1f8a6fb1083584c036caf`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.32-debian`

```console
$ docker pull mysql@sha256:01003f288c58133dad270905e2768e6a1d399d709a4a1375bc4f982f747252c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.32-debian` - linux; amd64

```console
$ docker pull mysql@sha256:38d6c177f28baa3b93350a59f0aae2c032418f05e2efd979c9da22d0a27d6223
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177766595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e8288d09e99593d17141361840c289947140d8e35f633ddeba0fab989abe3eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 10:59:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Mar 2023 10:59:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:59:38 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 10:59:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 10:59:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 10:59:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:59:55 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 10:59:55 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 10:59:55 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Thu, 23 Mar 2023 10:59:55 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Mar 2023 11:00:09 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Thu, 23 Mar 2023 11:00:10 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 11:00:10 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Thu, 23 Mar 2023 11:00:10 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 11:00:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 11:00:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:00:11 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 11:00:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6521829aee0429164fc3f7c547e84502400c78acde7a204473309a69c42de3`  
		Last Modified: Thu, 23 Mar 2023 11:01:26 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9f91eb302bb05cb9afddd1700b2642fd6618c437d04f4185f607b6328a96b4`  
		Last Modified: Thu, 23 Mar 2023 11:01:27 GMT  
		Size: 4.4 MB (4414934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13030349449a434afe037605a64bb8d3a329f038982cfc259d41614e5e07f9e6`  
		Last Modified: Thu, 23 Mar 2023 11:01:24 GMT  
		Size: 1.5 MB (1471385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c2b6b8463df89c8f2a6360c2f660aeaecfc6af04623b90c8672633b45508cf`  
		Last Modified: Thu, 23 Mar 2023 11:01:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c28230983db4101bc642c49ad9db328e79021f759b015452312fee84088bfd`  
		Last Modified: Thu, 23 Mar 2023 11:01:26 GMT  
		Size: 12.7 MB (12661950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d22d367ac2dbd2c3b82ae8b262419d0f4c0d52a347e70aec590b2ea0e3706d5`  
		Last Modified: Thu, 23 Mar 2023 11:01:24 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2bb5025fa157b775e71b1d4f2cdecd14b2d34b980f991ae86b50d0774057da`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e14277cdd802f47544aaa9a804c183ddef124757546b539b7c0f09379805728`  
		Last Modified: Thu, 23 Mar 2023 11:01:40 GMT  
		Size: 127.8 MB (127795886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a14127bf2fafa4308b78730e859d21a1d282b9508753a915c77fb970028891f`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed869d4966e891b12c705ddc7bb0f1f6cdb851ae2fc9106a46778f4c5f568ec7`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40298f9476557edea1f63b547f12e3a6814b8b110333bc90760d9363f86d8383`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.32-oracle`

```console
$ docker pull mysql@sha256:ca114710bb35b862062fd51733a7dba1ba3e93be33e4eede442b0ce15c77b718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.32-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1b5c4f72bfc2f2cc8c8fea93b277e871acac9bc421f4587ae499a074a4fefacd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156576131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a8bc460a9b517dd0230cc3d475ce0a9b9e1744e7959bb538f5572ec88139f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:20 GMT
ADD file:1a06059b1a097ecc61cb02965fc90e00183a8653d9ae009965823226559c5be9 in / 
# Wed, 22 Mar 2023 23:55:20 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:17:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:17:18 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:17:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:17:46 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:17:47 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:17:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:18:18 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:18:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:18:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:18:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:18:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:18:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:18:55 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:18:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab8798141d463c224f18fa5dd1d249b554dda61be24da7aa516e4e2de324db76`  
		Last Modified: Wed, 22 Mar 2023 23:56:08 GMT  
		Size: 44.6 MB (44563376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75508f0dccd76c48588532e73fcc39ecd235b6f8349c658ba4e10c863a95c076`  
		Last Modified: Thu, 23 Mar 2023 00:19:30 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1f5f86172459ac9f263a8f049036d17a9f59f8762f2222a0c0ba7d7e7e348`  
		Last Modified: Thu, 23 Mar 2023 00:19:31 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccc774632f39a5557e6005f85d9b32ad162c0a91eb4f0eb6b78c1b52a1a131d`  
		Last Modified: Thu, 23 Mar 2023 00:19:29 GMT  
		Size: 4.6 MB (4612146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7d864905655742ad222a835ff4edaaa87c0995bef926a3596448dd3c66bac0`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32480f1416f753cf219ff7c80cdeb4b0b5ae742e52c160d74ed4f13ebda5c807`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b89229d2472b456f860ad13a7aebade35883a35acb83e049382895768a103a9`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 56.2 MB (56223601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229bb5ff022d1021b28bf0f791baba9c05b2f635576dcd7c0d2da25431fd972b`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972d41dd67e3a7011a276a60717261d023296077f39afe611dead60c4445ffd`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 50.2 MB (50184513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8283d390a92ef33392ce41d164da7cfb4b36e714d72d81548f5ca5be222eba7`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddba158ba54022083e4b58c97b21cbd5580ba227e949f25a492efedd098321b9`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.32-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:657baef4941da52684daf5c048e1a12fb67966b0f78b24ece03f176f2ecee634
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155443156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996fa9077f757f6a87943dd5d5fff378cb0448baad30e625d7bdb4b8ce71df77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:59:36 GMT
ADD file:b4a46acde2a8ffdb8874f11aadcfc90177b15422278a1b8fa87e7ed9c97cf2a4 in / 
# Wed, 22 Mar 2023 23:59:36 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:20:19 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:20:19 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:20:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:20:45 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:20:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:20:47 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:21:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:21:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:21:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:21:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:21:47 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:21:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:21:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:21:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:21:47 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:21:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:40ffb7074955cd4f083dfcadee0a1ef1e12dbe031bdf2325c8bae38711b1f70f`  
		Last Modified: Thu, 23 Mar 2023 00:00:22 GMT  
		Size: 43.5 MB (43460037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2447ceb7b2b15bbd81959c0472744d693ef3bd26dc3fcd72bc4feae2981c674`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90547588960ca61c5b858a871ec898e2132d3e726e02927788839ac44f7e8b2`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989c2ac214cf31e965acd6a00e4861ba362bdad21503fadb60edf497db4f3e98`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 4.5 MB (4468367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaccc20c24ae65eeabb4e5b8131ab3cbd9f6ddb85787b14adf4281ea6d51bb2`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18556b046cb247ac0c905f09cc10ab904a995c40af90e027592ed97b3247479e`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05489c77c7a7d715a7fc0003c17ba0eb1c6cec38d5db1e82dd8fc82b626ae2b`  
		Last Modified: Thu, 23 Mar 2023 00:22:10 GMT  
		Size: 55.6 MB (55602642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98130d34badf6c2c91c251c423385532971d92717c0213e03919d7398ceb8db5`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd0424f0a2cde2a4d2f36980987bb8a699c2baf12ce7fdac586f7b13c3f79e4`  
		Last Modified: Thu, 23 Mar 2023 00:22:11 GMT  
		Size: 51.0 MB (50989444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77021328e41962d496870a28b8bf00d6877368c5338ed48fbc35f7cf828f8780`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3590288009eb3bfc73b08757208574ee742d8b4b1f8a6fb1083584c036caf`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:01003f288c58133dad270905e2768e6a1d399d709a4a1375bc4f982f747252c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:38d6c177f28baa3b93350a59f0aae2c032418f05e2efd979c9da22d0a27d6223
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177766595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e8288d09e99593d17141361840c289947140d8e35f633ddeba0fab989abe3eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 10:59:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Mar 2023 10:59:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:59:38 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 10:59:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 10:59:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 10:59:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:59:55 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 10:59:55 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 10:59:55 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Thu, 23 Mar 2023 10:59:55 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Mar 2023 11:00:09 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Thu, 23 Mar 2023 11:00:10 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 11:00:10 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Thu, 23 Mar 2023 11:00:10 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 11:00:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 11:00:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:00:11 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 11:00:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6521829aee0429164fc3f7c547e84502400c78acde7a204473309a69c42de3`  
		Last Modified: Thu, 23 Mar 2023 11:01:26 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9f91eb302bb05cb9afddd1700b2642fd6618c437d04f4185f607b6328a96b4`  
		Last Modified: Thu, 23 Mar 2023 11:01:27 GMT  
		Size: 4.4 MB (4414934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13030349449a434afe037605a64bb8d3a329f038982cfc259d41614e5e07f9e6`  
		Last Modified: Thu, 23 Mar 2023 11:01:24 GMT  
		Size: 1.5 MB (1471385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c2b6b8463df89c8f2a6360c2f660aeaecfc6af04623b90c8672633b45508cf`  
		Last Modified: Thu, 23 Mar 2023 11:01:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c28230983db4101bc642c49ad9db328e79021f759b015452312fee84088bfd`  
		Last Modified: Thu, 23 Mar 2023 11:01:26 GMT  
		Size: 12.7 MB (12661950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d22d367ac2dbd2c3b82ae8b262419d0f4c0d52a347e70aec590b2ea0e3706d5`  
		Last Modified: Thu, 23 Mar 2023 11:01:24 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2bb5025fa157b775e71b1d4f2cdecd14b2d34b980f991ae86b50d0774057da`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e14277cdd802f47544aaa9a804c183ddef124757546b539b7c0f09379805728`  
		Last Modified: Thu, 23 Mar 2023 11:01:40 GMT  
		Size: 127.8 MB (127795886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a14127bf2fafa4308b78730e859d21a1d282b9508753a915c77fb970028891f`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed869d4966e891b12c705ddc7bb0f1f6cdb851ae2fc9106a46778f4c5f568ec7`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40298f9476557edea1f63b547f12e3a6814b8b110333bc90760d9363f86d8383`  
		Last Modified: Thu, 23 Mar 2023 11:01:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:ca114710bb35b862062fd51733a7dba1ba3e93be33e4eede442b0ce15c77b718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:1b5c4f72bfc2f2cc8c8fea93b277e871acac9bc421f4587ae499a074a4fefacd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156576131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a8bc460a9b517dd0230cc3d475ce0a9b9e1744e7959bb538f5572ec88139f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:20 GMT
ADD file:1a06059b1a097ecc61cb02965fc90e00183a8653d9ae009965823226559c5be9 in / 
# Wed, 22 Mar 2023 23:55:20 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:17:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:17:18 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:17:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:17:46 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:17:47 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:17:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:18:18 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:18:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:18:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:18:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:18:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:18:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:18:55 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:18:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab8798141d463c224f18fa5dd1d249b554dda61be24da7aa516e4e2de324db76`  
		Last Modified: Wed, 22 Mar 2023 23:56:08 GMT  
		Size: 44.6 MB (44563376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75508f0dccd76c48588532e73fcc39ecd235b6f8349c658ba4e10c863a95c076`  
		Last Modified: Thu, 23 Mar 2023 00:19:30 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1f5f86172459ac9f263a8f049036d17a9f59f8762f2222a0c0ba7d7e7e348`  
		Last Modified: Thu, 23 Mar 2023 00:19:31 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccc774632f39a5557e6005f85d9b32ad162c0a91eb4f0eb6b78c1b52a1a131d`  
		Last Modified: Thu, 23 Mar 2023 00:19:29 GMT  
		Size: 4.6 MB (4612146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7d864905655742ad222a835ff4edaaa87c0995bef926a3596448dd3c66bac0`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32480f1416f753cf219ff7c80cdeb4b0b5ae742e52c160d74ed4f13ebda5c807`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b89229d2472b456f860ad13a7aebade35883a35acb83e049382895768a103a9`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 56.2 MB (56223601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229bb5ff022d1021b28bf0f791baba9c05b2f635576dcd7c0d2da25431fd972b`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972d41dd67e3a7011a276a60717261d023296077f39afe611dead60c4445ffd`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 50.2 MB (50184513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8283d390a92ef33392ce41d164da7cfb4b36e714d72d81548f5ca5be222eba7`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddba158ba54022083e4b58c97b21cbd5580ba227e949f25a492efedd098321b9`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:657baef4941da52684daf5c048e1a12fb67966b0f78b24ece03f176f2ecee634
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155443156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996fa9077f757f6a87943dd5d5fff378cb0448baad30e625d7bdb4b8ce71df77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:59:36 GMT
ADD file:b4a46acde2a8ffdb8874f11aadcfc90177b15422278a1b8fa87e7ed9c97cf2a4 in / 
# Wed, 22 Mar 2023 23:59:36 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:20:19 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:20:19 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:20:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:20:45 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:20:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:20:47 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:21:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:21:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:21:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:21:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:21:47 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:21:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:21:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:21:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:21:47 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:21:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:40ffb7074955cd4f083dfcadee0a1ef1e12dbe031bdf2325c8bae38711b1f70f`  
		Last Modified: Thu, 23 Mar 2023 00:00:22 GMT  
		Size: 43.5 MB (43460037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2447ceb7b2b15bbd81959c0472744d693ef3bd26dc3fcd72bc4feae2981c674`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90547588960ca61c5b858a871ec898e2132d3e726e02927788839ac44f7e8b2`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989c2ac214cf31e965acd6a00e4861ba362bdad21503fadb60edf497db4f3e98`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 4.5 MB (4468367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaccc20c24ae65eeabb4e5b8131ab3cbd9f6ddb85787b14adf4281ea6d51bb2`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18556b046cb247ac0c905f09cc10ab904a995c40af90e027592ed97b3247479e`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05489c77c7a7d715a7fc0003c17ba0eb1c6cec38d5db1e82dd8fc82b626ae2b`  
		Last Modified: Thu, 23 Mar 2023 00:22:10 GMT  
		Size: 55.6 MB (55602642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98130d34badf6c2c91c251c423385532971d92717c0213e03919d7398ceb8db5`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd0424f0a2cde2a4d2f36980987bb8a699c2baf12ce7fdac586f7b13c3f79e4`  
		Last Modified: Thu, 23 Mar 2023 00:22:11 GMT  
		Size: 51.0 MB (50989444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77021328e41962d496870a28b8bf00d6877368c5338ed48fbc35f7cf828f8780`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3590288009eb3bfc73b08757208574ee742d8b4b1f8a6fb1083584c036caf`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:ca114710bb35b862062fd51733a7dba1ba3e93be33e4eede442b0ce15c77b718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1b5c4f72bfc2f2cc8c8fea93b277e871acac9bc421f4587ae499a074a4fefacd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156576131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483a8bc460a9b517dd0230cc3d475ce0a9b9e1744e7959bb538f5572ec88139f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:20 GMT
ADD file:1a06059b1a097ecc61cb02965fc90e00183a8653d9ae009965823226559c5be9 in / 
# Wed, 22 Mar 2023 23:55:20 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:17:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:17:18 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:17:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:17:46 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:17:47 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:17:47 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:17:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:18:18 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:18:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:18:19 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:18:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:18:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:18:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:18:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:18:55 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:18:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ab8798141d463c224f18fa5dd1d249b554dda61be24da7aa516e4e2de324db76`  
		Last Modified: Wed, 22 Mar 2023 23:56:08 GMT  
		Size: 44.6 MB (44563376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75508f0dccd76c48588532e73fcc39ecd235b6f8349c658ba4e10c863a95c076`  
		Last Modified: Thu, 23 Mar 2023 00:19:30 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a1f5f86172459ac9f263a8f049036d17a9f59f8762f2222a0c0ba7d7e7e348`  
		Last Modified: Thu, 23 Mar 2023 00:19:31 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccc774632f39a5557e6005f85d9b32ad162c0a91eb4f0eb6b78c1b52a1a131d`  
		Last Modified: Thu, 23 Mar 2023 00:19:29 GMT  
		Size: 4.6 MB (4612146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7d864905655742ad222a835ff4edaaa87c0995bef926a3596448dd3c66bac0`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32480f1416f753cf219ff7c80cdeb4b0b5ae742e52c160d74ed4f13ebda5c807`  
		Last Modified: Thu, 23 Mar 2023 00:19:28 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b89229d2472b456f860ad13a7aebade35883a35acb83e049382895768a103a9`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 56.2 MB (56223601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229bb5ff022d1021b28bf0f791baba9c05b2f635576dcd7c0d2da25431fd972b`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a972d41dd67e3a7011a276a60717261d023296077f39afe611dead60c4445ffd`  
		Last Modified: Thu, 23 Mar 2023 00:19:35 GMT  
		Size: 50.2 MB (50184513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8283d390a92ef33392ce41d164da7cfb4b36e714d72d81548f5ca5be222eba7`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddba158ba54022083e4b58c97b21cbd5580ba227e949f25a492efedd098321b9`  
		Last Modified: Thu, 23 Mar 2023 00:19:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:657baef4941da52684daf5c048e1a12fb67966b0f78b24ece03f176f2ecee634
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155443156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996fa9077f757f6a87943dd5d5fff378cb0448baad30e625d7bdb4b8ce71df77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 22 Mar 2023 23:59:36 GMT
ADD file:b4a46acde2a8ffdb8874f11aadcfc90177b15422278a1b8fa87e7ed9c97cf2a4 in / 
# Wed, 22 Mar 2023 23:59:36 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:20:19 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Mar 2023 00:20:19 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 00:20:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 00:20:45 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:20:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Mar 2023 00:20:46 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:20:47 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Mar 2023 00:21:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Mar 2023 00:21:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Mar 2023 00:21:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Mar 2023 00:21:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Mar 2023 00:21:47 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 00:21:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 00:21:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 00:21:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 00:21:47 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 00:21:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:40ffb7074955cd4f083dfcadee0a1ef1e12dbe031bdf2325c8bae38711b1f70f`  
		Last Modified: Thu, 23 Mar 2023 00:00:22 GMT  
		Size: 43.5 MB (43460037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2447ceb7b2b15bbd81959c0472744d693ef3bd26dc3fcd72bc4feae2981c674`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90547588960ca61c5b858a871ec898e2132d3e726e02927788839ac44f7e8b2`  
		Last Modified: Thu, 23 Mar 2023 00:22:08 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989c2ac214cf31e965acd6a00e4861ba362bdad21503fadb60edf497db4f3e98`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 4.5 MB (4468367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaccc20c24ae65eeabb4e5b8131ab3cbd9f6ddb85787b14adf4281ea6d51bb2`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18556b046cb247ac0c905f09cc10ab904a995c40af90e027592ed97b3247479e`  
		Last Modified: Thu, 23 Mar 2023 00:22:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05489c77c7a7d715a7fc0003c17ba0eb1c6cec38d5db1e82dd8fc82b626ae2b`  
		Last Modified: Thu, 23 Mar 2023 00:22:10 GMT  
		Size: 55.6 MB (55602642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98130d34badf6c2c91c251c423385532971d92717c0213e03919d7398ceb8db5`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd0424f0a2cde2a4d2f36980987bb8a699c2baf12ce7fdac586f7b13c3f79e4`  
		Last Modified: Thu, 23 Mar 2023 00:22:11 GMT  
		Size: 51.0 MB (50989444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77021328e41962d496870a28b8bf00d6877368c5338ed48fbc35f7cf828f8780`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a3590288009eb3bfc73b08757208574ee742d8b4b1f8a6fb1083584c036caf`  
		Last Modified: Thu, 23 Mar 2023 00:22:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
