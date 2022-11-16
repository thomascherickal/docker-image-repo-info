<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5-debian`](#mysql5-debian)
-	[`mysql:5-oracle`](#mysql5-oracle)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7-debian`](#mysql57-debian)
-	[`mysql:5.7-oracle`](#mysql57-oracle)
-	[`mysql:5.7.40`](#mysql5740)
-	[`mysql:5.7.40-debian`](#mysql5740-debian)
-	[`mysql:5.7.40-oracle`](#mysql5740-oracle)
-	[`mysql:8`](#mysql8)
-	[`mysql:8-debian`](#mysql8-debian)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0.31`](#mysql8031)
-	[`mysql:8.0.31-debian`](#mysql8031-debian)
-	[`mysql:8.0.31-oracle`](#mysql8031-oracle)
-	[`mysql:debian`](#mysqldebian)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)

## `mysql:5`

```console
$ docker pull mysql@sha256:0e3435e72c493aec752d8274379b1eac4d634f47a7781a7a92b8636fa1dc94c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:55d2f4aa17fd27821a7fc575d2921485681a8aa5ac8411b75d7a163d895dfba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144285975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef0fab001e8dea739d538688b09e162bf54dd6c2bc04066bff99b5335cd6223`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:35 GMT
ADD file:aaaadfdf901c2df5f641e6c43b10817fcbd0caca73acb7672608f43ba71cefeb in / 
# Fri, 04 Nov 2022 23:33:36 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:36:26 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:36:26 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:36:29 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:36:47 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sat, 05 Nov 2022 02:36:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:36:48 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 05 Nov 2022 02:36:48 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Sat, 05 Nov 2022 02:36:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:37:06 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:37:07 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:37:07 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Sat, 05 Nov 2022 02:37:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:37:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:37:32 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:37:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:37:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:37:33 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:37:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9a0b9cd2dfe62ff7a933afe41891425abf01b0aaed70cedb028f03392d60037f`  
		Last Modified: Fri, 04 Nov 2022 23:35:26 GMT  
		Size: 49.8 MB (49827924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c637408ee7df7cd6e62a9fede4cb967dfff2c78d5fc9696bdda5753e03cffb0c`  
		Last Modified: Sat, 05 Nov 2022 02:38:56 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c517093c276008b69d7c9ae4e322cd0e97369293f972c009ab6e3ac05f50798`  
		Last Modified: Sat, 05 Nov 2022 02:38:56 GMT  
		Size: 930.2 KB (930228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301cc7d68c2a6517d07d136b6dd69d0ba624db02c2b425b85cd5095463498328`  
		Last Modified: Sat, 05 Nov 2022 02:38:54 GMT  
		Size: 4.5 MB (4538562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ca9bf9231a468ca8e638952c4e25435965f5446e72162f87740f3852574421`  
		Last Modified: Sat, 05 Nov 2022 02:38:53 GMT  
		Size: 2.7 KB (2655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae101e5c786802330f0f482df1b4c751a8dc07bc7977bd05a7dcd22e3421ed7`  
		Last Modified: Sat, 05 Nov 2022 02:38:53 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04baa409344ebae1d939845540196f7a24ba0db7da5aea2fb2bdf7b93913ef8a`  
		Last Modified: Sat, 05 Nov 2022 02:38:55 GMT  
		Size: 25.5 MB (25530141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b6015bf8537db46f7559e2a143a18db66ba37fafb8ddb3ede1a008631026a2`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6005bb052ef827d58b0bb7daa74921592043a9057f71c7f55f616dd53df1beb7`  
		Last Modified: Sat, 05 Nov 2022 02:39:03 GMT  
		Size: 63.4 MB (63449434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f303d570503342f3a4d383aad6093f58fdc135006c2e1a6155ec8549daa63d`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307a9a80c1df068cf45f516b05f99daa1b06825919403e44324c66ef15d2cdbb`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:b877923d9a3a233605b6fff7b1b66096ef95347953bdf8b53c644e4e4c2d6bd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:b70c887f9caf0bbdd214a7c6c768355de13ecc7ccb9b03cafc4e0e72873e129d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162596876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e85827503cde163497fe4dbc3c1c81d705b4db09166376e8b53a4d82763afd3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:02:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 15 Nov 2022 13:02:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:02:52 GMT
ENV GOSU_VERSION=1.14
# Tue, 15 Nov 2022 13:03:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 15 Nov 2022 13:03:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 15 Nov 2022 13:03:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:03:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 15 Nov 2022 13:03:09 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 15 Nov 2022 13:03:10 GMT
ENV MYSQL_VERSION=5.7.40-1debian10
# Tue, 15 Nov 2022 13:03:10 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 15 Nov 2022 13:03:30 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 15 Nov 2022 13:03:31 GMT
VOLUME [/var/lib/mysql]
# Tue, 15 Nov 2022 13:03:31 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:03:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 13:03:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:03:32 GMT
EXPOSE 3306 33060
# Tue, 15 Nov 2022 13:03:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a510d044b7fa285ab11ff2b921630bf7ef7f783b0d3b542b234756ff720a31`  
		Last Modified: Tue, 15 Nov 2022 13:04:46 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500105bda35026801de8c6b90a30c9c85dec9b17f329cc3cc8a290f7ec05d6c6`  
		Last Modified: Tue, 15 Nov 2022 13:04:44 GMT  
		Size: 4.2 MB (4182273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec0e829cb9c63abf33de3fba81f75214179f0e5fee33b4214497d2a1f6ceea1`  
		Last Modified: Tue, 15 Nov 2022 13:04:44 GMT  
		Size: 1.4 MB (1388891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05c9bcf57a0a6c938a4b447879a9b8b036037261f3284ceee456e7b02b3550b`  
		Last Modified: Tue, 15 Nov 2022 13:04:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fdb9acf81ea37d01f79d899999afd5cd9ad86595417f864e19cdb3d5a1fffb`  
		Last Modified: Tue, 15 Nov 2022 13:04:46 GMT  
		Size: 14.1 MB (14089378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f2f570a6edd65c0b3b554251d968470097014d810adfb27b96a98cd2e4a433`  
		Last Modified: Tue, 15 Nov 2022 13:04:42 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e884a2e58d9fcc54acea7d3e39908d7ecd42e1edfef73bb68191b54f991c6e67`  
		Last Modified: Tue, 15 Nov 2022 13:04:42 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9a1ff5f61c69e0b99c23045ec864acc99c0977ee4ff08e72fec757c2553f2b`  
		Last Modified: Tue, 15 Nov 2022 13:04:57 GMT  
		Size: 115.8 MB (115785814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db447849bdf4798b71bf9356ea7bb877bccdb13cbfcc41950625bd7f999a6ebb`  
		Last Modified: Tue, 15 Nov 2022 13:04:41 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4186431df56dd92a17a34b42da70b499494a80076ce02b2f62ab6d4b842d04c`  
		Last Modified: Tue, 15 Nov 2022 13:04:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:0e3435e72c493aec752d8274379b1eac4d634f47a7781a7a92b8636fa1dc94c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:55d2f4aa17fd27821a7fc575d2921485681a8aa5ac8411b75d7a163d895dfba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144285975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef0fab001e8dea739d538688b09e162bf54dd6c2bc04066bff99b5335cd6223`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:35 GMT
ADD file:aaaadfdf901c2df5f641e6c43b10817fcbd0caca73acb7672608f43ba71cefeb in / 
# Fri, 04 Nov 2022 23:33:36 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:36:26 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:36:26 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:36:29 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:36:47 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sat, 05 Nov 2022 02:36:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:36:48 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 05 Nov 2022 02:36:48 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Sat, 05 Nov 2022 02:36:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:37:06 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:37:07 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:37:07 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Sat, 05 Nov 2022 02:37:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:37:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:37:32 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:37:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:37:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:37:33 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:37:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9a0b9cd2dfe62ff7a933afe41891425abf01b0aaed70cedb028f03392d60037f`  
		Last Modified: Fri, 04 Nov 2022 23:35:26 GMT  
		Size: 49.8 MB (49827924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c637408ee7df7cd6e62a9fede4cb967dfff2c78d5fc9696bdda5753e03cffb0c`  
		Last Modified: Sat, 05 Nov 2022 02:38:56 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c517093c276008b69d7c9ae4e322cd0e97369293f972c009ab6e3ac05f50798`  
		Last Modified: Sat, 05 Nov 2022 02:38:56 GMT  
		Size: 930.2 KB (930228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301cc7d68c2a6517d07d136b6dd69d0ba624db02c2b425b85cd5095463498328`  
		Last Modified: Sat, 05 Nov 2022 02:38:54 GMT  
		Size: 4.5 MB (4538562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ca9bf9231a468ca8e638952c4e25435965f5446e72162f87740f3852574421`  
		Last Modified: Sat, 05 Nov 2022 02:38:53 GMT  
		Size: 2.7 KB (2655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae101e5c786802330f0f482df1b4c751a8dc07bc7977bd05a7dcd22e3421ed7`  
		Last Modified: Sat, 05 Nov 2022 02:38:53 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04baa409344ebae1d939845540196f7a24ba0db7da5aea2fb2bdf7b93913ef8a`  
		Last Modified: Sat, 05 Nov 2022 02:38:55 GMT  
		Size: 25.5 MB (25530141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b6015bf8537db46f7559e2a143a18db66ba37fafb8ddb3ede1a008631026a2`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6005bb052ef827d58b0bb7daa74921592043a9057f71c7f55f616dd53df1beb7`  
		Last Modified: Sat, 05 Nov 2022 02:39:03 GMT  
		Size: 63.4 MB (63449434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f303d570503342f3a4d383aad6093f58fdc135006c2e1a6155ec8549daa63d`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307a9a80c1df068cf45f516b05f99daa1b06825919403e44324c66ef15d2cdbb`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:0e3435e72c493aec752d8274379b1eac4d634f47a7781a7a92b8636fa1dc94c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:55d2f4aa17fd27821a7fc575d2921485681a8aa5ac8411b75d7a163d895dfba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144285975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef0fab001e8dea739d538688b09e162bf54dd6c2bc04066bff99b5335cd6223`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:35 GMT
ADD file:aaaadfdf901c2df5f641e6c43b10817fcbd0caca73acb7672608f43ba71cefeb in / 
# Fri, 04 Nov 2022 23:33:36 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:36:26 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:36:26 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:36:29 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:36:47 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sat, 05 Nov 2022 02:36:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:36:48 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 05 Nov 2022 02:36:48 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Sat, 05 Nov 2022 02:36:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:37:06 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:37:07 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:37:07 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Sat, 05 Nov 2022 02:37:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:37:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:37:32 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:37:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:37:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:37:33 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:37:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9a0b9cd2dfe62ff7a933afe41891425abf01b0aaed70cedb028f03392d60037f`  
		Last Modified: Fri, 04 Nov 2022 23:35:26 GMT  
		Size: 49.8 MB (49827924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c637408ee7df7cd6e62a9fede4cb967dfff2c78d5fc9696bdda5753e03cffb0c`  
		Last Modified: Sat, 05 Nov 2022 02:38:56 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c517093c276008b69d7c9ae4e322cd0e97369293f972c009ab6e3ac05f50798`  
		Last Modified: Sat, 05 Nov 2022 02:38:56 GMT  
		Size: 930.2 KB (930228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301cc7d68c2a6517d07d136b6dd69d0ba624db02c2b425b85cd5095463498328`  
		Last Modified: Sat, 05 Nov 2022 02:38:54 GMT  
		Size: 4.5 MB (4538562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ca9bf9231a468ca8e638952c4e25435965f5446e72162f87740f3852574421`  
		Last Modified: Sat, 05 Nov 2022 02:38:53 GMT  
		Size: 2.7 KB (2655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae101e5c786802330f0f482df1b4c751a8dc07bc7977bd05a7dcd22e3421ed7`  
		Last Modified: Sat, 05 Nov 2022 02:38:53 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04baa409344ebae1d939845540196f7a24ba0db7da5aea2fb2bdf7b93913ef8a`  
		Last Modified: Sat, 05 Nov 2022 02:38:55 GMT  
		Size: 25.5 MB (25530141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b6015bf8537db46f7559e2a143a18db66ba37fafb8ddb3ede1a008631026a2`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6005bb052ef827d58b0bb7daa74921592043a9057f71c7f55f616dd53df1beb7`  
		Last Modified: Sat, 05 Nov 2022 02:39:03 GMT  
		Size: 63.4 MB (63449434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f303d570503342f3a4d383aad6093f58fdc135006c2e1a6155ec8549daa63d`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307a9a80c1df068cf45f516b05f99daa1b06825919403e44324c66ef15d2cdbb`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:b877923d9a3a233605b6fff7b1b66096ef95347953bdf8b53c644e4e4c2d6bd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:b70c887f9caf0bbdd214a7c6c768355de13ecc7ccb9b03cafc4e0e72873e129d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162596876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e85827503cde163497fe4dbc3c1c81d705b4db09166376e8b53a4d82763afd3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:02:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 15 Nov 2022 13:02:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:02:52 GMT
ENV GOSU_VERSION=1.14
# Tue, 15 Nov 2022 13:03:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 15 Nov 2022 13:03:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 15 Nov 2022 13:03:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:03:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 15 Nov 2022 13:03:09 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 15 Nov 2022 13:03:10 GMT
ENV MYSQL_VERSION=5.7.40-1debian10
# Tue, 15 Nov 2022 13:03:10 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 15 Nov 2022 13:03:30 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 15 Nov 2022 13:03:31 GMT
VOLUME [/var/lib/mysql]
# Tue, 15 Nov 2022 13:03:31 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:03:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 13:03:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:03:32 GMT
EXPOSE 3306 33060
# Tue, 15 Nov 2022 13:03:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a510d044b7fa285ab11ff2b921630bf7ef7f783b0d3b542b234756ff720a31`  
		Last Modified: Tue, 15 Nov 2022 13:04:46 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500105bda35026801de8c6b90a30c9c85dec9b17f329cc3cc8a290f7ec05d6c6`  
		Last Modified: Tue, 15 Nov 2022 13:04:44 GMT  
		Size: 4.2 MB (4182273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec0e829cb9c63abf33de3fba81f75214179f0e5fee33b4214497d2a1f6ceea1`  
		Last Modified: Tue, 15 Nov 2022 13:04:44 GMT  
		Size: 1.4 MB (1388891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05c9bcf57a0a6c938a4b447879a9b8b036037261f3284ceee456e7b02b3550b`  
		Last Modified: Tue, 15 Nov 2022 13:04:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fdb9acf81ea37d01f79d899999afd5cd9ad86595417f864e19cdb3d5a1fffb`  
		Last Modified: Tue, 15 Nov 2022 13:04:46 GMT  
		Size: 14.1 MB (14089378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f2f570a6edd65c0b3b554251d968470097014d810adfb27b96a98cd2e4a433`  
		Last Modified: Tue, 15 Nov 2022 13:04:42 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e884a2e58d9fcc54acea7d3e39908d7ecd42e1edfef73bb68191b54f991c6e67`  
		Last Modified: Tue, 15 Nov 2022 13:04:42 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9a1ff5f61c69e0b99c23045ec864acc99c0977ee4ff08e72fec757c2553f2b`  
		Last Modified: Tue, 15 Nov 2022 13:04:57 GMT  
		Size: 115.8 MB (115785814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db447849bdf4798b71bf9356ea7bb877bccdb13cbfcc41950625bd7f999a6ebb`  
		Last Modified: Tue, 15 Nov 2022 13:04:41 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4186431df56dd92a17a34b42da70b499494a80076ce02b2f62ab6d4b842d04c`  
		Last Modified: Tue, 15 Nov 2022 13:04:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:0e3435e72c493aec752d8274379b1eac4d634f47a7781a7a92b8636fa1dc94c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:55d2f4aa17fd27821a7fc575d2921485681a8aa5ac8411b75d7a163d895dfba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144285975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef0fab001e8dea739d538688b09e162bf54dd6c2bc04066bff99b5335cd6223`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:35 GMT
ADD file:aaaadfdf901c2df5f641e6c43b10817fcbd0caca73acb7672608f43ba71cefeb in / 
# Fri, 04 Nov 2022 23:33:36 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:36:26 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:36:26 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:36:29 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:36:47 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sat, 05 Nov 2022 02:36:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:36:48 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 05 Nov 2022 02:36:48 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Sat, 05 Nov 2022 02:36:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:37:06 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:37:07 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:37:07 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Sat, 05 Nov 2022 02:37:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:37:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:37:32 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:37:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:37:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:37:33 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:37:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9a0b9cd2dfe62ff7a933afe41891425abf01b0aaed70cedb028f03392d60037f`  
		Last Modified: Fri, 04 Nov 2022 23:35:26 GMT  
		Size: 49.8 MB (49827924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c637408ee7df7cd6e62a9fede4cb967dfff2c78d5fc9696bdda5753e03cffb0c`  
		Last Modified: Sat, 05 Nov 2022 02:38:56 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c517093c276008b69d7c9ae4e322cd0e97369293f972c009ab6e3ac05f50798`  
		Last Modified: Sat, 05 Nov 2022 02:38:56 GMT  
		Size: 930.2 KB (930228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301cc7d68c2a6517d07d136b6dd69d0ba624db02c2b425b85cd5095463498328`  
		Last Modified: Sat, 05 Nov 2022 02:38:54 GMT  
		Size: 4.5 MB (4538562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ca9bf9231a468ca8e638952c4e25435965f5446e72162f87740f3852574421`  
		Last Modified: Sat, 05 Nov 2022 02:38:53 GMT  
		Size: 2.7 KB (2655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae101e5c786802330f0f482df1b4c751a8dc07bc7977bd05a7dcd22e3421ed7`  
		Last Modified: Sat, 05 Nov 2022 02:38:53 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04baa409344ebae1d939845540196f7a24ba0db7da5aea2fb2bdf7b93913ef8a`  
		Last Modified: Sat, 05 Nov 2022 02:38:55 GMT  
		Size: 25.5 MB (25530141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b6015bf8537db46f7559e2a143a18db66ba37fafb8ddb3ede1a008631026a2`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6005bb052ef827d58b0bb7daa74921592043a9057f71c7f55f616dd53df1beb7`  
		Last Modified: Sat, 05 Nov 2022 02:39:03 GMT  
		Size: 63.4 MB (63449434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f303d570503342f3a4d383aad6093f58fdc135006c2e1a6155ec8549daa63d`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307a9a80c1df068cf45f516b05f99daa1b06825919403e44324c66ef15d2cdbb`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40`

```console
$ docker pull mysql@sha256:0e3435e72c493aec752d8274379b1eac4d634f47a7781a7a92b8636fa1dc94c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40` - linux; amd64

```console
$ docker pull mysql@sha256:55d2f4aa17fd27821a7fc575d2921485681a8aa5ac8411b75d7a163d895dfba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144285975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef0fab001e8dea739d538688b09e162bf54dd6c2bc04066bff99b5335cd6223`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:35 GMT
ADD file:aaaadfdf901c2df5f641e6c43b10817fcbd0caca73acb7672608f43ba71cefeb in / 
# Fri, 04 Nov 2022 23:33:36 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:36:26 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:36:26 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:36:29 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:36:47 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sat, 05 Nov 2022 02:36:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:36:48 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 05 Nov 2022 02:36:48 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Sat, 05 Nov 2022 02:36:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:37:06 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:37:07 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:37:07 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Sat, 05 Nov 2022 02:37:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:37:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:37:32 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:37:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:37:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:37:33 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:37:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9a0b9cd2dfe62ff7a933afe41891425abf01b0aaed70cedb028f03392d60037f`  
		Last Modified: Fri, 04 Nov 2022 23:35:26 GMT  
		Size: 49.8 MB (49827924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c637408ee7df7cd6e62a9fede4cb967dfff2c78d5fc9696bdda5753e03cffb0c`  
		Last Modified: Sat, 05 Nov 2022 02:38:56 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c517093c276008b69d7c9ae4e322cd0e97369293f972c009ab6e3ac05f50798`  
		Last Modified: Sat, 05 Nov 2022 02:38:56 GMT  
		Size: 930.2 KB (930228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301cc7d68c2a6517d07d136b6dd69d0ba624db02c2b425b85cd5095463498328`  
		Last Modified: Sat, 05 Nov 2022 02:38:54 GMT  
		Size: 4.5 MB (4538562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ca9bf9231a468ca8e638952c4e25435965f5446e72162f87740f3852574421`  
		Last Modified: Sat, 05 Nov 2022 02:38:53 GMT  
		Size: 2.7 KB (2655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae101e5c786802330f0f482df1b4c751a8dc07bc7977bd05a7dcd22e3421ed7`  
		Last Modified: Sat, 05 Nov 2022 02:38:53 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04baa409344ebae1d939845540196f7a24ba0db7da5aea2fb2bdf7b93913ef8a`  
		Last Modified: Sat, 05 Nov 2022 02:38:55 GMT  
		Size: 25.5 MB (25530141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b6015bf8537db46f7559e2a143a18db66ba37fafb8ddb3ede1a008631026a2`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6005bb052ef827d58b0bb7daa74921592043a9057f71c7f55f616dd53df1beb7`  
		Last Modified: Sat, 05 Nov 2022 02:39:03 GMT  
		Size: 63.4 MB (63449434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f303d570503342f3a4d383aad6093f58fdc135006c2e1a6155ec8549daa63d`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307a9a80c1df068cf45f516b05f99daa1b06825919403e44324c66ef15d2cdbb`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40-debian`

```console
$ docker pull mysql@sha256:b877923d9a3a233605b6fff7b1b66096ef95347953bdf8b53c644e4e4c2d6bd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40-debian` - linux; amd64

```console
$ docker pull mysql@sha256:b70c887f9caf0bbdd214a7c6c768355de13ecc7ccb9b03cafc4e0e72873e129d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162596876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e85827503cde163497fe4dbc3c1c81d705b4db09166376e8b53a4d82763afd3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:02:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 15 Nov 2022 13:02:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:02:52 GMT
ENV GOSU_VERSION=1.14
# Tue, 15 Nov 2022 13:03:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 15 Nov 2022 13:03:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 15 Nov 2022 13:03:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:03:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 15 Nov 2022 13:03:09 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 15 Nov 2022 13:03:10 GMT
ENV MYSQL_VERSION=5.7.40-1debian10
# Tue, 15 Nov 2022 13:03:10 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 15 Nov 2022 13:03:30 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 15 Nov 2022 13:03:31 GMT
VOLUME [/var/lib/mysql]
# Tue, 15 Nov 2022 13:03:31 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:03:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 13:03:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:03:32 GMT
EXPOSE 3306 33060
# Tue, 15 Nov 2022 13:03:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a510d044b7fa285ab11ff2b921630bf7ef7f783b0d3b542b234756ff720a31`  
		Last Modified: Tue, 15 Nov 2022 13:04:46 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500105bda35026801de8c6b90a30c9c85dec9b17f329cc3cc8a290f7ec05d6c6`  
		Last Modified: Tue, 15 Nov 2022 13:04:44 GMT  
		Size: 4.2 MB (4182273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec0e829cb9c63abf33de3fba81f75214179f0e5fee33b4214497d2a1f6ceea1`  
		Last Modified: Tue, 15 Nov 2022 13:04:44 GMT  
		Size: 1.4 MB (1388891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05c9bcf57a0a6c938a4b447879a9b8b036037261f3284ceee456e7b02b3550b`  
		Last Modified: Tue, 15 Nov 2022 13:04:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fdb9acf81ea37d01f79d899999afd5cd9ad86595417f864e19cdb3d5a1fffb`  
		Last Modified: Tue, 15 Nov 2022 13:04:46 GMT  
		Size: 14.1 MB (14089378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f2f570a6edd65c0b3b554251d968470097014d810adfb27b96a98cd2e4a433`  
		Last Modified: Tue, 15 Nov 2022 13:04:42 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e884a2e58d9fcc54acea7d3e39908d7ecd42e1edfef73bb68191b54f991c6e67`  
		Last Modified: Tue, 15 Nov 2022 13:04:42 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9a1ff5f61c69e0b99c23045ec864acc99c0977ee4ff08e72fec757c2553f2b`  
		Last Modified: Tue, 15 Nov 2022 13:04:57 GMT  
		Size: 115.8 MB (115785814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db447849bdf4798b71bf9356ea7bb877bccdb13cbfcc41950625bd7f999a6ebb`  
		Last Modified: Tue, 15 Nov 2022 13:04:41 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4186431df56dd92a17a34b42da70b499494a80076ce02b2f62ab6d4b842d04c`  
		Last Modified: Tue, 15 Nov 2022 13:04:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40-oracle`

```console
$ docker pull mysql@sha256:0e3435e72c493aec752d8274379b1eac4d634f47a7781a7a92b8636fa1dc94c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:55d2f4aa17fd27821a7fc575d2921485681a8aa5ac8411b75d7a163d895dfba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144285975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef0fab001e8dea739d538688b09e162bf54dd6c2bc04066bff99b5335cd6223`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:35 GMT
ADD file:aaaadfdf901c2df5f641e6c43b10817fcbd0caca73acb7672608f43ba71cefeb in / 
# Fri, 04 Nov 2022 23:33:36 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:36:26 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:36:26 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:36:29 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:36:47 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sat, 05 Nov 2022 02:36:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:36:48 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 05 Nov 2022 02:36:48 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Sat, 05 Nov 2022 02:36:48 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:37:06 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:37:07 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:37:07 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Sat, 05 Nov 2022 02:37:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:37:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:37:32 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:37:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:37:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:37:33 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:37:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9a0b9cd2dfe62ff7a933afe41891425abf01b0aaed70cedb028f03392d60037f`  
		Last Modified: Fri, 04 Nov 2022 23:35:26 GMT  
		Size: 49.8 MB (49827924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c637408ee7df7cd6e62a9fede4cb967dfff2c78d5fc9696bdda5753e03cffb0c`  
		Last Modified: Sat, 05 Nov 2022 02:38:56 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c517093c276008b69d7c9ae4e322cd0e97369293f972c009ab6e3ac05f50798`  
		Last Modified: Sat, 05 Nov 2022 02:38:56 GMT  
		Size: 930.2 KB (930228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301cc7d68c2a6517d07d136b6dd69d0ba624db02c2b425b85cd5095463498328`  
		Last Modified: Sat, 05 Nov 2022 02:38:54 GMT  
		Size: 4.5 MB (4538562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ca9bf9231a468ca8e638952c4e25435965f5446e72162f87740f3852574421`  
		Last Modified: Sat, 05 Nov 2022 02:38:53 GMT  
		Size: 2.7 KB (2655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae101e5c786802330f0f482df1b4c751a8dc07bc7977bd05a7dcd22e3421ed7`  
		Last Modified: Sat, 05 Nov 2022 02:38:53 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04baa409344ebae1d939845540196f7a24ba0db7da5aea2fb2bdf7b93913ef8a`  
		Last Modified: Sat, 05 Nov 2022 02:38:55 GMT  
		Size: 25.5 MB (25530141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b6015bf8537db46f7559e2a143a18db66ba37fafb8ddb3ede1a008631026a2`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6005bb052ef827d58b0bb7daa74921592043a9057f71c7f55f616dd53df1beb7`  
		Last Modified: Sat, 05 Nov 2022 02:39:03 GMT  
		Size: 63.4 MB (63449434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f303d570503342f3a4d383aad6093f58fdc135006c2e1a6155ec8549daa63d`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307a9a80c1df068cf45f516b05f99daa1b06825919403e44324c66ef15d2cdbb`  
		Last Modified: Sat, 05 Nov 2022 02:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:25aace9734db96ae09c24c6a2eeb6db4720c41d493de352eb76007eddf437fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:bd6a2996d80605c41b1ebd8f822894471695b1fd2427505ac518e650a14ef8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.2 MB (157232215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04bf34fdf036292486d39f731cffaf0bb56522c340fe4841b2c71cf89c9d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:07 GMT
ADD file:00e6899b8d3eccf7f795d17f9316af6ae0f3955ef2204b61bd064f5173c18357 in / 
# Fri, 04 Nov 2022 23:33:07 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:34:46 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:34:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:34:50 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:35:13 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 05 Nov 2022 02:35:14 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:35:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:35:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:35:45 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:35:45 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:36:18 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:36:19 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:36:19 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:36:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:36:20 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:36:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:feec22b5b79860f47a87861bed3a29d5431a279cc239b44a2522a9ab5459d844`  
		Last Modified: Fri, 04 Nov 2022 23:34:48 GMT  
		Size: 40.6 MB (40580917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b33952322b1265ccfb1a2fa879b86ccb58a3c5f02567a902cac8d7d1e1fbcac`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8632ee03bb1ca20bb263a7bab04dda4995925a4ed5e2a16fa83e174a53a840c3`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636ccd115361ca8e84b27ef37d14d6119748b71900dade590ecd963afab4450c`  
		Last Modified: Sat, 05 Nov 2022 02:38:16 GMT  
		Size: 4.6 MB (4596992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c8fac8eead4f4a9e8284577eaf9ae5ca2c78a3cbecf1b9f0c7a4b78337665`  
		Last Modified: Sat, 05 Nov 2022 02:38:15 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44c54db9c140998b59508c389ead06ffbe863051125b2dd2b150db5d8f87010`  
		Last Modified: Sat, 05 Nov 2022 02:38:14 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9c45749101c2502030b52b11f5cf1031d08ceabeab91283742467bdbe2dc62`  
		Last Modified: Sat, 05 Nov 2022 02:38:21 GMT  
		Size: 56.0 MB (56047607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2fa3febc47da546527aae2d8de736b7562b0e8f5a37a63778aa86307af8d2d`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d5e1d3c311ae16390016bcf09a400cc9e67473f8ea5787abe0855f510e917b`  
		Last Modified: Sat, 05 Nov 2022 02:38:23 GMT  
		Size: 55.1 MB (55068188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3db2c5d8ec681907739aa09873795aa7ffacfacfbd43d79f140331029f8517`  
		Last Modified: Sat, 05 Nov 2022 02:38:13 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ead729abd92d539d786eed0146f98fbfb8a970de2f0b082e9a0aa4ecc6d1fc`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a0b6340a3f236d39451f2373c5d137bf64eb54233163c186ef1480e8844f0ffd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159044836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b61a400e8776905c7164e1adcf7c9457bfe43dca3db94b667a3e4dd8e7f02c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 23:40:44 GMT
ADD file:44569001378d2d59b2d169aba48a6b2b88529ca46fd5d85598eff7ca37ded076 in / 
# Tue, 15 Nov 2022 23:40:45 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 01:33:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 16 Nov 2022 01:33:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 16 Nov 2022 01:33:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Nov 2022 01:33:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 16 Nov 2022 01:33:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:33:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 16 Nov 2022 01:34:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 16 Nov 2022 01:34:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 16 Nov 2022 01:34:16 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:34:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 16 Nov 2022 01:34:46 GMT
VOLUME [/var/lib/mysql]
# Wed, 16 Nov 2022 01:34:46 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 16 Nov 2022 01:34:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 16 Nov 2022 01:34:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 01:34:46 GMT
EXPOSE 3306 33060
# Wed, 16 Nov 2022 01:34:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01d65ebb4955ae24720eb5c24ff08081fed75975aea7b87c96ef7e58175901e0`  
		Last Modified: Tue, 15 Nov 2022 23:41:32 GMT  
		Size: 42.8 MB (42774711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d609fcc3c7fb5a4b262e7f8a002961e11802f03e441d9e8a2c1d0a03b606e1ee`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c09cdcd2da34e1fedf1e87c4cf449692e8fcd446a600a227ff7a3c678eba26`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 857.2 KB (857169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a478ef641e124539c75eca120d506f59fc5058ce27559d948305ec930643717`  
		Last Modified: Wed, 16 Nov 2022 01:35:15 GMT  
		Size: 4.5 MB (4465955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3956cc2f3fb1e3431a0db90666aa3e21c2015b9ddd6da49babc7bb389a09e8`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c37cc7a1914f1576343f24a780bedcdea90a844ccd62488df65355b06468fd`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0cd074dc147bcc06f8561f3added6b2ea97772000b3628f2e03503691904e0`  
		Last Modified: Wed, 16 Nov 2022 01:35:18 GMT  
		Size: 55.5 MB (55457981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9186a35382189d0459f0ce2a8166b45cbf2be5599cfe5716bdbc5de71ee3d2b2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443c4afe5f0f372b7558dc78484a7577e29c0d906b2e4324fbeb81d6bee853f`  
		Last Modified: Wed, 16 Nov 2022 01:35:20 GMT  
		Size: 55.5 MB (55479334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dbcd809e720177fc48884b92fb5e724ada0908ef9449445df4847f40a9c3d2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb36129f08c1e07dd8ad073c1fa8012fb05b03766001cbc228fbddc20edec95e`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:a5f0cdc27aaaf52e125ef95feb8f16c8e01b6dfdc19bd4eee22d208877f7fec3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:b7723f5c0013576dded81e7da91a0292780c41c87ac0d141c7c11ac0c7b40bf6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177566940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7b8f072515bf2a39727cd3cbdd5e43895134aab2dab401fcbaefe720a4a447`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:01:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 15 Nov 2022 13:02:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:02:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 15 Nov 2022 13:02:12 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 15 Nov 2022 13:02:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 15 Nov 2022 13:02:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:02:20 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 15 Nov 2022 13:02:20 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 15 Nov 2022 13:02:21 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Tue, 15 Nov 2022 13:02:21 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 15 Nov 2022 13:02:37 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 15 Nov 2022 13:02:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 15 Nov 2022 13:02:38 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 15 Nov 2022 13:02:38 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:02:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 13:02:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:02:39 GMT
EXPOSE 3306 33060
# Tue, 15 Nov 2022 13:02:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c5f46b86bcde1607df33835202723f7b164fd874d81a292fdc328c68e714a3`  
		Last Modified: Tue, 15 Nov 2022 13:04:09 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c41730774e57a40d58b667771334846a553c84ce0cb8a5cd1525ab637ab56f`  
		Last Modified: Tue, 15 Nov 2022 13:04:10 GMT  
		Size: 4.4 MB (4415531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0b738276122ae857e7479755a5e0d5b75e21a1b92541afd6bd3c723ca17cb2`  
		Last Modified: Tue, 15 Nov 2022 13:04:09 GMT  
		Size: 1.4 MB (1419597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e2a4ee2f48e0bdb4367b24613350cb231b44cf2337d62cef351cdcecf9dea4`  
		Last Modified: Tue, 15 Nov 2022 13:04:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e97140efbd3e579539602d0908ec7f8f90d71d73a0850aa13480e28e64a1a`  
		Last Modified: Tue, 15 Nov 2022 13:04:10 GMT  
		Size: 12.7 MB (12662693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a25338f20c7cbc43f390e1dd932c88cc77fca7dcd28c224b225f1292b495129`  
		Last Modified: Tue, 15 Nov 2022 13:04:07 GMT  
		Size: 2.5 KB (2546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ab7c6b6e5a076a7d08e4a4b9d812324a3aa2732efd34a61ad88340b4120f3d`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cca68c51cd74b5a9928a31416fee5f7c053909f4dd69a871c032ba3b1c6e0c0`  
		Last Modified: Tue, 15 Nov 2022 13:04:26 GMT  
		Size: 127.6 MB (127645462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb97b3e2ff53ba242734da8a86e131f21c5ed0088a2f320944b0a9208093553`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f36551fe8601acb1b3a61be725080a34ebbdce748037cdfce1457bce5190fae`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbb3d0b9f8d905f0092d8dfc76996f24463ad13647feefd50946202fe7c4a31`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:25aace9734db96ae09c24c6a2eeb6db4720c41d493de352eb76007eddf437fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:bd6a2996d80605c41b1ebd8f822894471695b1fd2427505ac518e650a14ef8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.2 MB (157232215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04bf34fdf036292486d39f731cffaf0bb56522c340fe4841b2c71cf89c9d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:07 GMT
ADD file:00e6899b8d3eccf7f795d17f9316af6ae0f3955ef2204b61bd064f5173c18357 in / 
# Fri, 04 Nov 2022 23:33:07 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:34:46 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:34:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:34:50 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:35:13 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 05 Nov 2022 02:35:14 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:35:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:35:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:35:45 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:35:45 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:36:18 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:36:19 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:36:19 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:36:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:36:20 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:36:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:feec22b5b79860f47a87861bed3a29d5431a279cc239b44a2522a9ab5459d844`  
		Last Modified: Fri, 04 Nov 2022 23:34:48 GMT  
		Size: 40.6 MB (40580917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b33952322b1265ccfb1a2fa879b86ccb58a3c5f02567a902cac8d7d1e1fbcac`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8632ee03bb1ca20bb263a7bab04dda4995925a4ed5e2a16fa83e174a53a840c3`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636ccd115361ca8e84b27ef37d14d6119748b71900dade590ecd963afab4450c`  
		Last Modified: Sat, 05 Nov 2022 02:38:16 GMT  
		Size: 4.6 MB (4596992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c8fac8eead4f4a9e8284577eaf9ae5ca2c78a3cbecf1b9f0c7a4b78337665`  
		Last Modified: Sat, 05 Nov 2022 02:38:15 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44c54db9c140998b59508c389ead06ffbe863051125b2dd2b150db5d8f87010`  
		Last Modified: Sat, 05 Nov 2022 02:38:14 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9c45749101c2502030b52b11f5cf1031d08ceabeab91283742467bdbe2dc62`  
		Last Modified: Sat, 05 Nov 2022 02:38:21 GMT  
		Size: 56.0 MB (56047607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2fa3febc47da546527aae2d8de736b7562b0e8f5a37a63778aa86307af8d2d`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d5e1d3c311ae16390016bcf09a400cc9e67473f8ea5787abe0855f510e917b`  
		Last Modified: Sat, 05 Nov 2022 02:38:23 GMT  
		Size: 55.1 MB (55068188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3db2c5d8ec681907739aa09873795aa7ffacfacfbd43d79f140331029f8517`  
		Last Modified: Sat, 05 Nov 2022 02:38:13 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ead729abd92d539d786eed0146f98fbfb8a970de2f0b082e9a0aa4ecc6d1fc`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a0b6340a3f236d39451f2373c5d137bf64eb54233163c186ef1480e8844f0ffd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159044836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b61a400e8776905c7164e1adcf7c9457bfe43dca3db94b667a3e4dd8e7f02c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 23:40:44 GMT
ADD file:44569001378d2d59b2d169aba48a6b2b88529ca46fd5d85598eff7ca37ded076 in / 
# Tue, 15 Nov 2022 23:40:45 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 01:33:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 16 Nov 2022 01:33:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 16 Nov 2022 01:33:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Nov 2022 01:33:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 16 Nov 2022 01:33:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:33:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 16 Nov 2022 01:34:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 16 Nov 2022 01:34:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 16 Nov 2022 01:34:16 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:34:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 16 Nov 2022 01:34:46 GMT
VOLUME [/var/lib/mysql]
# Wed, 16 Nov 2022 01:34:46 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 16 Nov 2022 01:34:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 16 Nov 2022 01:34:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 01:34:46 GMT
EXPOSE 3306 33060
# Wed, 16 Nov 2022 01:34:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01d65ebb4955ae24720eb5c24ff08081fed75975aea7b87c96ef7e58175901e0`  
		Last Modified: Tue, 15 Nov 2022 23:41:32 GMT  
		Size: 42.8 MB (42774711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d609fcc3c7fb5a4b262e7f8a002961e11802f03e441d9e8a2c1d0a03b606e1ee`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c09cdcd2da34e1fedf1e87c4cf449692e8fcd446a600a227ff7a3c678eba26`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 857.2 KB (857169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a478ef641e124539c75eca120d506f59fc5058ce27559d948305ec930643717`  
		Last Modified: Wed, 16 Nov 2022 01:35:15 GMT  
		Size: 4.5 MB (4465955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3956cc2f3fb1e3431a0db90666aa3e21c2015b9ddd6da49babc7bb389a09e8`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c37cc7a1914f1576343f24a780bedcdea90a844ccd62488df65355b06468fd`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0cd074dc147bcc06f8561f3added6b2ea97772000b3628f2e03503691904e0`  
		Last Modified: Wed, 16 Nov 2022 01:35:18 GMT  
		Size: 55.5 MB (55457981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9186a35382189d0459f0ce2a8166b45cbf2be5599cfe5716bdbc5de71ee3d2b2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443c4afe5f0f372b7558dc78484a7577e29c0d906b2e4324fbeb81d6bee853f`  
		Last Modified: Wed, 16 Nov 2022 01:35:20 GMT  
		Size: 55.5 MB (55479334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dbcd809e720177fc48884b92fb5e724ada0908ef9449445df4847f40a9c3d2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb36129f08c1e07dd8ad073c1fa8012fb05b03766001cbc228fbddc20edec95e`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:25aace9734db96ae09c24c6a2eeb6db4720c41d493de352eb76007eddf437fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:bd6a2996d80605c41b1ebd8f822894471695b1fd2427505ac518e650a14ef8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.2 MB (157232215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04bf34fdf036292486d39f731cffaf0bb56522c340fe4841b2c71cf89c9d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:07 GMT
ADD file:00e6899b8d3eccf7f795d17f9316af6ae0f3955ef2204b61bd064f5173c18357 in / 
# Fri, 04 Nov 2022 23:33:07 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:34:46 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:34:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:34:50 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:35:13 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 05 Nov 2022 02:35:14 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:35:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:35:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:35:45 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:35:45 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:36:18 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:36:19 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:36:19 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:36:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:36:20 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:36:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:feec22b5b79860f47a87861bed3a29d5431a279cc239b44a2522a9ab5459d844`  
		Last Modified: Fri, 04 Nov 2022 23:34:48 GMT  
		Size: 40.6 MB (40580917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b33952322b1265ccfb1a2fa879b86ccb58a3c5f02567a902cac8d7d1e1fbcac`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8632ee03bb1ca20bb263a7bab04dda4995925a4ed5e2a16fa83e174a53a840c3`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636ccd115361ca8e84b27ef37d14d6119748b71900dade590ecd963afab4450c`  
		Last Modified: Sat, 05 Nov 2022 02:38:16 GMT  
		Size: 4.6 MB (4596992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c8fac8eead4f4a9e8284577eaf9ae5ca2c78a3cbecf1b9f0c7a4b78337665`  
		Last Modified: Sat, 05 Nov 2022 02:38:15 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44c54db9c140998b59508c389ead06ffbe863051125b2dd2b150db5d8f87010`  
		Last Modified: Sat, 05 Nov 2022 02:38:14 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9c45749101c2502030b52b11f5cf1031d08ceabeab91283742467bdbe2dc62`  
		Last Modified: Sat, 05 Nov 2022 02:38:21 GMT  
		Size: 56.0 MB (56047607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2fa3febc47da546527aae2d8de736b7562b0e8f5a37a63778aa86307af8d2d`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d5e1d3c311ae16390016bcf09a400cc9e67473f8ea5787abe0855f510e917b`  
		Last Modified: Sat, 05 Nov 2022 02:38:23 GMT  
		Size: 55.1 MB (55068188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3db2c5d8ec681907739aa09873795aa7ffacfacfbd43d79f140331029f8517`  
		Last Modified: Sat, 05 Nov 2022 02:38:13 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ead729abd92d539d786eed0146f98fbfb8a970de2f0b082e9a0aa4ecc6d1fc`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a0b6340a3f236d39451f2373c5d137bf64eb54233163c186ef1480e8844f0ffd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159044836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b61a400e8776905c7164e1adcf7c9457bfe43dca3db94b667a3e4dd8e7f02c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 23:40:44 GMT
ADD file:44569001378d2d59b2d169aba48a6b2b88529ca46fd5d85598eff7ca37ded076 in / 
# Tue, 15 Nov 2022 23:40:45 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 01:33:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 16 Nov 2022 01:33:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 16 Nov 2022 01:33:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Nov 2022 01:33:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 16 Nov 2022 01:33:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:33:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 16 Nov 2022 01:34:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 16 Nov 2022 01:34:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 16 Nov 2022 01:34:16 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:34:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 16 Nov 2022 01:34:46 GMT
VOLUME [/var/lib/mysql]
# Wed, 16 Nov 2022 01:34:46 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 16 Nov 2022 01:34:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 16 Nov 2022 01:34:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 01:34:46 GMT
EXPOSE 3306 33060
# Wed, 16 Nov 2022 01:34:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01d65ebb4955ae24720eb5c24ff08081fed75975aea7b87c96ef7e58175901e0`  
		Last Modified: Tue, 15 Nov 2022 23:41:32 GMT  
		Size: 42.8 MB (42774711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d609fcc3c7fb5a4b262e7f8a002961e11802f03e441d9e8a2c1d0a03b606e1ee`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c09cdcd2da34e1fedf1e87c4cf449692e8fcd446a600a227ff7a3c678eba26`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 857.2 KB (857169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a478ef641e124539c75eca120d506f59fc5058ce27559d948305ec930643717`  
		Last Modified: Wed, 16 Nov 2022 01:35:15 GMT  
		Size: 4.5 MB (4465955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3956cc2f3fb1e3431a0db90666aa3e21c2015b9ddd6da49babc7bb389a09e8`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c37cc7a1914f1576343f24a780bedcdea90a844ccd62488df65355b06468fd`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0cd074dc147bcc06f8561f3added6b2ea97772000b3628f2e03503691904e0`  
		Last Modified: Wed, 16 Nov 2022 01:35:18 GMT  
		Size: 55.5 MB (55457981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9186a35382189d0459f0ce2a8166b45cbf2be5599cfe5716bdbc5de71ee3d2b2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443c4afe5f0f372b7558dc78484a7577e29c0d906b2e4324fbeb81d6bee853f`  
		Last Modified: Wed, 16 Nov 2022 01:35:20 GMT  
		Size: 55.5 MB (55479334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dbcd809e720177fc48884b92fb5e724ada0908ef9449445df4847f40a9c3d2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb36129f08c1e07dd8ad073c1fa8012fb05b03766001cbc228fbddc20edec95e`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:a5f0cdc27aaaf52e125ef95feb8f16c8e01b6dfdc19bd4eee22d208877f7fec3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:b7723f5c0013576dded81e7da91a0292780c41c87ac0d141c7c11ac0c7b40bf6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177566940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7b8f072515bf2a39727cd3cbdd5e43895134aab2dab401fcbaefe720a4a447`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:01:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 15 Nov 2022 13:02:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:02:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 15 Nov 2022 13:02:12 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 15 Nov 2022 13:02:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 15 Nov 2022 13:02:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:02:20 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 15 Nov 2022 13:02:20 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 15 Nov 2022 13:02:21 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Tue, 15 Nov 2022 13:02:21 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 15 Nov 2022 13:02:37 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 15 Nov 2022 13:02:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 15 Nov 2022 13:02:38 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 15 Nov 2022 13:02:38 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:02:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 13:02:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:02:39 GMT
EXPOSE 3306 33060
# Tue, 15 Nov 2022 13:02:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c5f46b86bcde1607df33835202723f7b164fd874d81a292fdc328c68e714a3`  
		Last Modified: Tue, 15 Nov 2022 13:04:09 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c41730774e57a40d58b667771334846a553c84ce0cb8a5cd1525ab637ab56f`  
		Last Modified: Tue, 15 Nov 2022 13:04:10 GMT  
		Size: 4.4 MB (4415531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0b738276122ae857e7479755a5e0d5b75e21a1b92541afd6bd3c723ca17cb2`  
		Last Modified: Tue, 15 Nov 2022 13:04:09 GMT  
		Size: 1.4 MB (1419597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e2a4ee2f48e0bdb4367b24613350cb231b44cf2337d62cef351cdcecf9dea4`  
		Last Modified: Tue, 15 Nov 2022 13:04:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e97140efbd3e579539602d0908ec7f8f90d71d73a0850aa13480e28e64a1a`  
		Last Modified: Tue, 15 Nov 2022 13:04:10 GMT  
		Size: 12.7 MB (12662693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a25338f20c7cbc43f390e1dd932c88cc77fca7dcd28c224b225f1292b495129`  
		Last Modified: Tue, 15 Nov 2022 13:04:07 GMT  
		Size: 2.5 KB (2546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ab7c6b6e5a076a7d08e4a4b9d812324a3aa2732efd34a61ad88340b4120f3d`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cca68c51cd74b5a9928a31416fee5f7c053909f4dd69a871c032ba3b1c6e0c0`  
		Last Modified: Tue, 15 Nov 2022 13:04:26 GMT  
		Size: 127.6 MB (127645462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb97b3e2ff53ba242734da8a86e131f21c5ed0088a2f320944b0a9208093553`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f36551fe8601acb1b3a61be725080a34ebbdce748037cdfce1457bce5190fae`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbb3d0b9f8d905f0092d8dfc76996f24463ad13647feefd50946202fe7c4a31`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:25aace9734db96ae09c24c6a2eeb6db4720c41d493de352eb76007eddf437fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:bd6a2996d80605c41b1ebd8f822894471695b1fd2427505ac518e650a14ef8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.2 MB (157232215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04bf34fdf036292486d39f731cffaf0bb56522c340fe4841b2c71cf89c9d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:07 GMT
ADD file:00e6899b8d3eccf7f795d17f9316af6ae0f3955ef2204b61bd064f5173c18357 in / 
# Fri, 04 Nov 2022 23:33:07 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:34:46 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:34:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:34:50 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:35:13 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 05 Nov 2022 02:35:14 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:35:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:35:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:35:45 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:35:45 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:36:18 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:36:19 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:36:19 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:36:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:36:20 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:36:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:feec22b5b79860f47a87861bed3a29d5431a279cc239b44a2522a9ab5459d844`  
		Last Modified: Fri, 04 Nov 2022 23:34:48 GMT  
		Size: 40.6 MB (40580917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b33952322b1265ccfb1a2fa879b86ccb58a3c5f02567a902cac8d7d1e1fbcac`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8632ee03bb1ca20bb263a7bab04dda4995925a4ed5e2a16fa83e174a53a840c3`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636ccd115361ca8e84b27ef37d14d6119748b71900dade590ecd963afab4450c`  
		Last Modified: Sat, 05 Nov 2022 02:38:16 GMT  
		Size: 4.6 MB (4596992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c8fac8eead4f4a9e8284577eaf9ae5ca2c78a3cbecf1b9f0c7a4b78337665`  
		Last Modified: Sat, 05 Nov 2022 02:38:15 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44c54db9c140998b59508c389ead06ffbe863051125b2dd2b150db5d8f87010`  
		Last Modified: Sat, 05 Nov 2022 02:38:14 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9c45749101c2502030b52b11f5cf1031d08ceabeab91283742467bdbe2dc62`  
		Last Modified: Sat, 05 Nov 2022 02:38:21 GMT  
		Size: 56.0 MB (56047607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2fa3febc47da546527aae2d8de736b7562b0e8f5a37a63778aa86307af8d2d`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d5e1d3c311ae16390016bcf09a400cc9e67473f8ea5787abe0855f510e917b`  
		Last Modified: Sat, 05 Nov 2022 02:38:23 GMT  
		Size: 55.1 MB (55068188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3db2c5d8ec681907739aa09873795aa7ffacfacfbd43d79f140331029f8517`  
		Last Modified: Sat, 05 Nov 2022 02:38:13 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ead729abd92d539d786eed0146f98fbfb8a970de2f0b082e9a0aa4ecc6d1fc`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a0b6340a3f236d39451f2373c5d137bf64eb54233163c186ef1480e8844f0ffd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159044836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b61a400e8776905c7164e1adcf7c9457bfe43dca3db94b667a3e4dd8e7f02c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 23:40:44 GMT
ADD file:44569001378d2d59b2d169aba48a6b2b88529ca46fd5d85598eff7ca37ded076 in / 
# Tue, 15 Nov 2022 23:40:45 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 01:33:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 16 Nov 2022 01:33:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 16 Nov 2022 01:33:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Nov 2022 01:33:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 16 Nov 2022 01:33:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:33:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 16 Nov 2022 01:34:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 16 Nov 2022 01:34:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 16 Nov 2022 01:34:16 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:34:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 16 Nov 2022 01:34:46 GMT
VOLUME [/var/lib/mysql]
# Wed, 16 Nov 2022 01:34:46 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 16 Nov 2022 01:34:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 16 Nov 2022 01:34:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 01:34:46 GMT
EXPOSE 3306 33060
# Wed, 16 Nov 2022 01:34:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01d65ebb4955ae24720eb5c24ff08081fed75975aea7b87c96ef7e58175901e0`  
		Last Modified: Tue, 15 Nov 2022 23:41:32 GMT  
		Size: 42.8 MB (42774711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d609fcc3c7fb5a4b262e7f8a002961e11802f03e441d9e8a2c1d0a03b606e1ee`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c09cdcd2da34e1fedf1e87c4cf449692e8fcd446a600a227ff7a3c678eba26`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 857.2 KB (857169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a478ef641e124539c75eca120d506f59fc5058ce27559d948305ec930643717`  
		Last Modified: Wed, 16 Nov 2022 01:35:15 GMT  
		Size: 4.5 MB (4465955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3956cc2f3fb1e3431a0db90666aa3e21c2015b9ddd6da49babc7bb389a09e8`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c37cc7a1914f1576343f24a780bedcdea90a844ccd62488df65355b06468fd`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0cd074dc147bcc06f8561f3added6b2ea97772000b3628f2e03503691904e0`  
		Last Modified: Wed, 16 Nov 2022 01:35:18 GMT  
		Size: 55.5 MB (55457981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9186a35382189d0459f0ce2a8166b45cbf2be5599cfe5716bdbc5de71ee3d2b2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443c4afe5f0f372b7558dc78484a7577e29c0d906b2e4324fbeb81d6bee853f`  
		Last Modified: Wed, 16 Nov 2022 01:35:20 GMT  
		Size: 55.5 MB (55479334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dbcd809e720177fc48884b92fb5e724ada0908ef9449445df4847f40a9c3d2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb36129f08c1e07dd8ad073c1fa8012fb05b03766001cbc228fbddc20edec95e`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31`

```console
$ docker pull mysql@sha256:25aace9734db96ae09c24c6a2eeb6db4720c41d493de352eb76007eddf437fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.31` - linux; amd64

```console
$ docker pull mysql@sha256:bd6a2996d80605c41b1ebd8f822894471695b1fd2427505ac518e650a14ef8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.2 MB (157232215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04bf34fdf036292486d39f731cffaf0bb56522c340fe4841b2c71cf89c9d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:07 GMT
ADD file:00e6899b8d3eccf7f795d17f9316af6ae0f3955ef2204b61bd064f5173c18357 in / 
# Fri, 04 Nov 2022 23:33:07 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:34:46 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:34:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:34:50 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:35:13 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 05 Nov 2022 02:35:14 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:35:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:35:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:35:45 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:35:45 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:36:18 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:36:19 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:36:19 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:36:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:36:20 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:36:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:feec22b5b79860f47a87861bed3a29d5431a279cc239b44a2522a9ab5459d844`  
		Last Modified: Fri, 04 Nov 2022 23:34:48 GMT  
		Size: 40.6 MB (40580917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b33952322b1265ccfb1a2fa879b86ccb58a3c5f02567a902cac8d7d1e1fbcac`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8632ee03bb1ca20bb263a7bab04dda4995925a4ed5e2a16fa83e174a53a840c3`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636ccd115361ca8e84b27ef37d14d6119748b71900dade590ecd963afab4450c`  
		Last Modified: Sat, 05 Nov 2022 02:38:16 GMT  
		Size: 4.6 MB (4596992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c8fac8eead4f4a9e8284577eaf9ae5ca2c78a3cbecf1b9f0c7a4b78337665`  
		Last Modified: Sat, 05 Nov 2022 02:38:15 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44c54db9c140998b59508c389ead06ffbe863051125b2dd2b150db5d8f87010`  
		Last Modified: Sat, 05 Nov 2022 02:38:14 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9c45749101c2502030b52b11f5cf1031d08ceabeab91283742467bdbe2dc62`  
		Last Modified: Sat, 05 Nov 2022 02:38:21 GMT  
		Size: 56.0 MB (56047607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2fa3febc47da546527aae2d8de736b7562b0e8f5a37a63778aa86307af8d2d`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d5e1d3c311ae16390016bcf09a400cc9e67473f8ea5787abe0855f510e917b`  
		Last Modified: Sat, 05 Nov 2022 02:38:23 GMT  
		Size: 55.1 MB (55068188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3db2c5d8ec681907739aa09873795aa7ffacfacfbd43d79f140331029f8517`  
		Last Modified: Sat, 05 Nov 2022 02:38:13 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ead729abd92d539d786eed0146f98fbfb8a970de2f0b082e9a0aa4ecc6d1fc`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.31` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a0b6340a3f236d39451f2373c5d137bf64eb54233163c186ef1480e8844f0ffd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159044836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b61a400e8776905c7164e1adcf7c9457bfe43dca3db94b667a3e4dd8e7f02c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 23:40:44 GMT
ADD file:44569001378d2d59b2d169aba48a6b2b88529ca46fd5d85598eff7ca37ded076 in / 
# Tue, 15 Nov 2022 23:40:45 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 01:33:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 16 Nov 2022 01:33:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 16 Nov 2022 01:33:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Nov 2022 01:33:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 16 Nov 2022 01:33:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:33:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 16 Nov 2022 01:34:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 16 Nov 2022 01:34:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 16 Nov 2022 01:34:16 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:34:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 16 Nov 2022 01:34:46 GMT
VOLUME [/var/lib/mysql]
# Wed, 16 Nov 2022 01:34:46 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 16 Nov 2022 01:34:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 16 Nov 2022 01:34:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 01:34:46 GMT
EXPOSE 3306 33060
# Wed, 16 Nov 2022 01:34:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01d65ebb4955ae24720eb5c24ff08081fed75975aea7b87c96ef7e58175901e0`  
		Last Modified: Tue, 15 Nov 2022 23:41:32 GMT  
		Size: 42.8 MB (42774711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d609fcc3c7fb5a4b262e7f8a002961e11802f03e441d9e8a2c1d0a03b606e1ee`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c09cdcd2da34e1fedf1e87c4cf449692e8fcd446a600a227ff7a3c678eba26`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 857.2 KB (857169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a478ef641e124539c75eca120d506f59fc5058ce27559d948305ec930643717`  
		Last Modified: Wed, 16 Nov 2022 01:35:15 GMT  
		Size: 4.5 MB (4465955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3956cc2f3fb1e3431a0db90666aa3e21c2015b9ddd6da49babc7bb389a09e8`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c37cc7a1914f1576343f24a780bedcdea90a844ccd62488df65355b06468fd`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0cd074dc147bcc06f8561f3added6b2ea97772000b3628f2e03503691904e0`  
		Last Modified: Wed, 16 Nov 2022 01:35:18 GMT  
		Size: 55.5 MB (55457981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9186a35382189d0459f0ce2a8166b45cbf2be5599cfe5716bdbc5de71ee3d2b2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443c4afe5f0f372b7558dc78484a7577e29c0d906b2e4324fbeb81d6bee853f`  
		Last Modified: Wed, 16 Nov 2022 01:35:20 GMT  
		Size: 55.5 MB (55479334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dbcd809e720177fc48884b92fb5e724ada0908ef9449445df4847f40a9c3d2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb36129f08c1e07dd8ad073c1fa8012fb05b03766001cbc228fbddc20edec95e`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31-debian`

```console
$ docker pull mysql@sha256:a5f0cdc27aaaf52e125ef95feb8f16c8e01b6dfdc19bd4eee22d208877f7fec3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.31-debian` - linux; amd64

```console
$ docker pull mysql@sha256:b7723f5c0013576dded81e7da91a0292780c41c87ac0d141c7c11ac0c7b40bf6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177566940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7b8f072515bf2a39727cd3cbdd5e43895134aab2dab401fcbaefe720a4a447`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:01:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 15 Nov 2022 13:02:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:02:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 15 Nov 2022 13:02:12 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 15 Nov 2022 13:02:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 15 Nov 2022 13:02:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:02:20 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 15 Nov 2022 13:02:20 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 15 Nov 2022 13:02:21 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Tue, 15 Nov 2022 13:02:21 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 15 Nov 2022 13:02:37 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 15 Nov 2022 13:02:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 15 Nov 2022 13:02:38 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 15 Nov 2022 13:02:38 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:02:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 13:02:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:02:39 GMT
EXPOSE 3306 33060
# Tue, 15 Nov 2022 13:02:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c5f46b86bcde1607df33835202723f7b164fd874d81a292fdc328c68e714a3`  
		Last Modified: Tue, 15 Nov 2022 13:04:09 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c41730774e57a40d58b667771334846a553c84ce0cb8a5cd1525ab637ab56f`  
		Last Modified: Tue, 15 Nov 2022 13:04:10 GMT  
		Size: 4.4 MB (4415531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0b738276122ae857e7479755a5e0d5b75e21a1b92541afd6bd3c723ca17cb2`  
		Last Modified: Tue, 15 Nov 2022 13:04:09 GMT  
		Size: 1.4 MB (1419597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e2a4ee2f48e0bdb4367b24613350cb231b44cf2337d62cef351cdcecf9dea4`  
		Last Modified: Tue, 15 Nov 2022 13:04:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e97140efbd3e579539602d0908ec7f8f90d71d73a0850aa13480e28e64a1a`  
		Last Modified: Tue, 15 Nov 2022 13:04:10 GMT  
		Size: 12.7 MB (12662693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a25338f20c7cbc43f390e1dd932c88cc77fca7dcd28c224b225f1292b495129`  
		Last Modified: Tue, 15 Nov 2022 13:04:07 GMT  
		Size: 2.5 KB (2546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ab7c6b6e5a076a7d08e4a4b9d812324a3aa2732efd34a61ad88340b4120f3d`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cca68c51cd74b5a9928a31416fee5f7c053909f4dd69a871c032ba3b1c6e0c0`  
		Last Modified: Tue, 15 Nov 2022 13:04:26 GMT  
		Size: 127.6 MB (127645462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb97b3e2ff53ba242734da8a86e131f21c5ed0088a2f320944b0a9208093553`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f36551fe8601acb1b3a61be725080a34ebbdce748037cdfce1457bce5190fae`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbb3d0b9f8d905f0092d8dfc76996f24463ad13647feefd50946202fe7c4a31`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31-oracle`

```console
$ docker pull mysql@sha256:25aace9734db96ae09c24c6a2eeb6db4720c41d493de352eb76007eddf437fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.31-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:bd6a2996d80605c41b1ebd8f822894471695b1fd2427505ac518e650a14ef8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.2 MB (157232215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04bf34fdf036292486d39f731cffaf0bb56522c340fe4841b2c71cf89c9d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:07 GMT
ADD file:00e6899b8d3eccf7f795d17f9316af6ae0f3955ef2204b61bd064f5173c18357 in / 
# Fri, 04 Nov 2022 23:33:07 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:34:46 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:34:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:34:50 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:35:13 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 05 Nov 2022 02:35:14 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:35:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:35:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:35:45 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:35:45 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:36:18 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:36:19 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:36:19 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:36:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:36:20 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:36:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:feec22b5b79860f47a87861bed3a29d5431a279cc239b44a2522a9ab5459d844`  
		Last Modified: Fri, 04 Nov 2022 23:34:48 GMT  
		Size: 40.6 MB (40580917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b33952322b1265ccfb1a2fa879b86ccb58a3c5f02567a902cac8d7d1e1fbcac`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8632ee03bb1ca20bb263a7bab04dda4995925a4ed5e2a16fa83e174a53a840c3`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636ccd115361ca8e84b27ef37d14d6119748b71900dade590ecd963afab4450c`  
		Last Modified: Sat, 05 Nov 2022 02:38:16 GMT  
		Size: 4.6 MB (4596992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c8fac8eead4f4a9e8284577eaf9ae5ca2c78a3cbecf1b9f0c7a4b78337665`  
		Last Modified: Sat, 05 Nov 2022 02:38:15 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44c54db9c140998b59508c389ead06ffbe863051125b2dd2b150db5d8f87010`  
		Last Modified: Sat, 05 Nov 2022 02:38:14 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9c45749101c2502030b52b11f5cf1031d08ceabeab91283742467bdbe2dc62`  
		Last Modified: Sat, 05 Nov 2022 02:38:21 GMT  
		Size: 56.0 MB (56047607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2fa3febc47da546527aae2d8de736b7562b0e8f5a37a63778aa86307af8d2d`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d5e1d3c311ae16390016bcf09a400cc9e67473f8ea5787abe0855f510e917b`  
		Last Modified: Sat, 05 Nov 2022 02:38:23 GMT  
		Size: 55.1 MB (55068188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3db2c5d8ec681907739aa09873795aa7ffacfacfbd43d79f140331029f8517`  
		Last Modified: Sat, 05 Nov 2022 02:38:13 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ead729abd92d539d786eed0146f98fbfb8a970de2f0b082e9a0aa4ecc6d1fc`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.31-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a0b6340a3f236d39451f2373c5d137bf64eb54233163c186ef1480e8844f0ffd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159044836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b61a400e8776905c7164e1adcf7c9457bfe43dca3db94b667a3e4dd8e7f02c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 23:40:44 GMT
ADD file:44569001378d2d59b2d169aba48a6b2b88529ca46fd5d85598eff7ca37ded076 in / 
# Tue, 15 Nov 2022 23:40:45 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 01:33:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 16 Nov 2022 01:33:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 16 Nov 2022 01:33:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Nov 2022 01:33:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 16 Nov 2022 01:33:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:33:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 16 Nov 2022 01:34:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 16 Nov 2022 01:34:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 16 Nov 2022 01:34:16 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:34:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 16 Nov 2022 01:34:46 GMT
VOLUME [/var/lib/mysql]
# Wed, 16 Nov 2022 01:34:46 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 16 Nov 2022 01:34:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 16 Nov 2022 01:34:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 01:34:46 GMT
EXPOSE 3306 33060
# Wed, 16 Nov 2022 01:34:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01d65ebb4955ae24720eb5c24ff08081fed75975aea7b87c96ef7e58175901e0`  
		Last Modified: Tue, 15 Nov 2022 23:41:32 GMT  
		Size: 42.8 MB (42774711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d609fcc3c7fb5a4b262e7f8a002961e11802f03e441d9e8a2c1d0a03b606e1ee`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c09cdcd2da34e1fedf1e87c4cf449692e8fcd446a600a227ff7a3c678eba26`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 857.2 KB (857169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a478ef641e124539c75eca120d506f59fc5058ce27559d948305ec930643717`  
		Last Modified: Wed, 16 Nov 2022 01:35:15 GMT  
		Size: 4.5 MB (4465955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3956cc2f3fb1e3431a0db90666aa3e21c2015b9ddd6da49babc7bb389a09e8`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c37cc7a1914f1576343f24a780bedcdea90a844ccd62488df65355b06468fd`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0cd074dc147bcc06f8561f3added6b2ea97772000b3628f2e03503691904e0`  
		Last Modified: Wed, 16 Nov 2022 01:35:18 GMT  
		Size: 55.5 MB (55457981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9186a35382189d0459f0ce2a8166b45cbf2be5599cfe5716bdbc5de71ee3d2b2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443c4afe5f0f372b7558dc78484a7577e29c0d906b2e4324fbeb81d6bee853f`  
		Last Modified: Wed, 16 Nov 2022 01:35:20 GMT  
		Size: 55.5 MB (55479334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dbcd809e720177fc48884b92fb5e724ada0908ef9449445df4847f40a9c3d2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb36129f08c1e07dd8ad073c1fa8012fb05b03766001cbc228fbddc20edec95e`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:a5f0cdc27aaaf52e125ef95feb8f16c8e01b6dfdc19bd4eee22d208877f7fec3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:b7723f5c0013576dded81e7da91a0292780c41c87ac0d141c7c11ac0c7b40bf6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177566940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7b8f072515bf2a39727cd3cbdd5e43895134aab2dab401fcbaefe720a4a447`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:01:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 15 Nov 2022 13:02:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:02:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 15 Nov 2022 13:02:12 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 15 Nov 2022 13:02:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 15 Nov 2022 13:02:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:02:20 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 15 Nov 2022 13:02:20 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 15 Nov 2022 13:02:21 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Tue, 15 Nov 2022 13:02:21 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 15 Nov 2022 13:02:37 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 15 Nov 2022 13:02:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 15 Nov 2022 13:02:38 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 15 Nov 2022 13:02:38 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 15 Nov 2022 13:02:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 13:02:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:02:39 GMT
EXPOSE 3306 33060
# Tue, 15 Nov 2022 13:02:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c5f46b86bcde1607df33835202723f7b164fd874d81a292fdc328c68e714a3`  
		Last Modified: Tue, 15 Nov 2022 13:04:09 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c41730774e57a40d58b667771334846a553c84ce0cb8a5cd1525ab637ab56f`  
		Last Modified: Tue, 15 Nov 2022 13:04:10 GMT  
		Size: 4.4 MB (4415531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0b738276122ae857e7479755a5e0d5b75e21a1b92541afd6bd3c723ca17cb2`  
		Last Modified: Tue, 15 Nov 2022 13:04:09 GMT  
		Size: 1.4 MB (1419597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e2a4ee2f48e0bdb4367b24613350cb231b44cf2337d62cef351cdcecf9dea4`  
		Last Modified: Tue, 15 Nov 2022 13:04:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e97140efbd3e579539602d0908ec7f8f90d71d73a0850aa13480e28e64a1a`  
		Last Modified: Tue, 15 Nov 2022 13:04:10 GMT  
		Size: 12.7 MB (12662693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a25338f20c7cbc43f390e1dd932c88cc77fca7dcd28c224b225f1292b495129`  
		Last Modified: Tue, 15 Nov 2022 13:04:07 GMT  
		Size: 2.5 KB (2546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ab7c6b6e5a076a7d08e4a4b9d812324a3aa2732efd34a61ad88340b4120f3d`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cca68c51cd74b5a9928a31416fee5f7c053909f4dd69a871c032ba3b1c6e0c0`  
		Last Modified: Tue, 15 Nov 2022 13:04:26 GMT  
		Size: 127.6 MB (127645462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb97b3e2ff53ba242734da8a86e131f21c5ed0088a2f320944b0a9208093553`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f36551fe8601acb1b3a61be725080a34ebbdce748037cdfce1457bce5190fae`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dbb3d0b9f8d905f0092d8dfc76996f24463ad13647feefd50946202fe7c4a31`  
		Last Modified: Tue, 15 Nov 2022 13:04:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:25aace9734db96ae09c24c6a2eeb6db4720c41d493de352eb76007eddf437fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:bd6a2996d80605c41b1ebd8f822894471695b1fd2427505ac518e650a14ef8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.2 MB (157232215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04bf34fdf036292486d39f731cffaf0bb56522c340fe4841b2c71cf89c9d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:07 GMT
ADD file:00e6899b8d3eccf7f795d17f9316af6ae0f3955ef2204b61bd064f5173c18357 in / 
# Fri, 04 Nov 2022 23:33:07 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:34:46 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:34:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:34:50 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:35:13 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 05 Nov 2022 02:35:14 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:35:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:35:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:35:45 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:35:45 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:36:18 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:36:19 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:36:19 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:36:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:36:20 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:36:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:feec22b5b79860f47a87861bed3a29d5431a279cc239b44a2522a9ab5459d844`  
		Last Modified: Fri, 04 Nov 2022 23:34:48 GMT  
		Size: 40.6 MB (40580917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b33952322b1265ccfb1a2fa879b86ccb58a3c5f02567a902cac8d7d1e1fbcac`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8632ee03bb1ca20bb263a7bab04dda4995925a4ed5e2a16fa83e174a53a840c3`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636ccd115361ca8e84b27ef37d14d6119748b71900dade590ecd963afab4450c`  
		Last Modified: Sat, 05 Nov 2022 02:38:16 GMT  
		Size: 4.6 MB (4596992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c8fac8eead4f4a9e8284577eaf9ae5ca2c78a3cbecf1b9f0c7a4b78337665`  
		Last Modified: Sat, 05 Nov 2022 02:38:15 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44c54db9c140998b59508c389ead06ffbe863051125b2dd2b150db5d8f87010`  
		Last Modified: Sat, 05 Nov 2022 02:38:14 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9c45749101c2502030b52b11f5cf1031d08ceabeab91283742467bdbe2dc62`  
		Last Modified: Sat, 05 Nov 2022 02:38:21 GMT  
		Size: 56.0 MB (56047607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2fa3febc47da546527aae2d8de736b7562b0e8f5a37a63778aa86307af8d2d`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d5e1d3c311ae16390016bcf09a400cc9e67473f8ea5787abe0855f510e917b`  
		Last Modified: Sat, 05 Nov 2022 02:38:23 GMT  
		Size: 55.1 MB (55068188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3db2c5d8ec681907739aa09873795aa7ffacfacfbd43d79f140331029f8517`  
		Last Modified: Sat, 05 Nov 2022 02:38:13 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ead729abd92d539d786eed0146f98fbfb8a970de2f0b082e9a0aa4ecc6d1fc`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a0b6340a3f236d39451f2373c5d137bf64eb54233163c186ef1480e8844f0ffd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159044836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b61a400e8776905c7164e1adcf7c9457bfe43dca3db94b667a3e4dd8e7f02c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 23:40:44 GMT
ADD file:44569001378d2d59b2d169aba48a6b2b88529ca46fd5d85598eff7ca37ded076 in / 
# Tue, 15 Nov 2022 23:40:45 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 01:33:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 16 Nov 2022 01:33:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 16 Nov 2022 01:33:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Nov 2022 01:33:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 16 Nov 2022 01:33:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:33:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 16 Nov 2022 01:34:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 16 Nov 2022 01:34:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 16 Nov 2022 01:34:16 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:34:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 16 Nov 2022 01:34:46 GMT
VOLUME [/var/lib/mysql]
# Wed, 16 Nov 2022 01:34:46 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 16 Nov 2022 01:34:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 16 Nov 2022 01:34:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 01:34:46 GMT
EXPOSE 3306 33060
# Wed, 16 Nov 2022 01:34:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01d65ebb4955ae24720eb5c24ff08081fed75975aea7b87c96ef7e58175901e0`  
		Last Modified: Tue, 15 Nov 2022 23:41:32 GMT  
		Size: 42.8 MB (42774711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d609fcc3c7fb5a4b262e7f8a002961e11802f03e441d9e8a2c1d0a03b606e1ee`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c09cdcd2da34e1fedf1e87c4cf449692e8fcd446a600a227ff7a3c678eba26`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 857.2 KB (857169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a478ef641e124539c75eca120d506f59fc5058ce27559d948305ec930643717`  
		Last Modified: Wed, 16 Nov 2022 01:35:15 GMT  
		Size: 4.5 MB (4465955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3956cc2f3fb1e3431a0db90666aa3e21c2015b9ddd6da49babc7bb389a09e8`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c37cc7a1914f1576343f24a780bedcdea90a844ccd62488df65355b06468fd`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0cd074dc147bcc06f8561f3added6b2ea97772000b3628f2e03503691904e0`  
		Last Modified: Wed, 16 Nov 2022 01:35:18 GMT  
		Size: 55.5 MB (55457981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9186a35382189d0459f0ce2a8166b45cbf2be5599cfe5716bdbc5de71ee3d2b2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443c4afe5f0f372b7558dc78484a7577e29c0d906b2e4324fbeb81d6bee853f`  
		Last Modified: Wed, 16 Nov 2022 01:35:20 GMT  
		Size: 55.5 MB (55479334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dbcd809e720177fc48884b92fb5e724ada0908ef9449445df4847f40a9c3d2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb36129f08c1e07dd8ad073c1fa8012fb05b03766001cbc228fbddc20edec95e`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:25aace9734db96ae09c24c6a2eeb6db4720c41d493de352eb76007eddf437fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:bd6a2996d80605c41b1ebd8f822894471695b1fd2427505ac518e650a14ef8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.2 MB (157232215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04bf34fdf036292486d39f731cffaf0bb56522c340fe4841b2c71cf89c9d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:07 GMT
ADD file:00e6899b8d3eccf7f795d17f9316af6ae0f3955ef2204b61bd064f5173c18357 in / 
# Fri, 04 Nov 2022 23:33:07 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:34:46 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:34:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:34:50 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:35:13 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 05 Nov 2022 02:35:14 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:35:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:35:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:35:45 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:35:45 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:36:18 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:36:19 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:36:19 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:36:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:36:20 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:36:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:feec22b5b79860f47a87861bed3a29d5431a279cc239b44a2522a9ab5459d844`  
		Last Modified: Fri, 04 Nov 2022 23:34:48 GMT  
		Size: 40.6 MB (40580917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b33952322b1265ccfb1a2fa879b86ccb58a3c5f02567a902cac8d7d1e1fbcac`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8632ee03bb1ca20bb263a7bab04dda4995925a4ed5e2a16fa83e174a53a840c3`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636ccd115361ca8e84b27ef37d14d6119748b71900dade590ecd963afab4450c`  
		Last Modified: Sat, 05 Nov 2022 02:38:16 GMT  
		Size: 4.6 MB (4596992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c8fac8eead4f4a9e8284577eaf9ae5ca2c78a3cbecf1b9f0c7a4b78337665`  
		Last Modified: Sat, 05 Nov 2022 02:38:15 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44c54db9c140998b59508c389ead06ffbe863051125b2dd2b150db5d8f87010`  
		Last Modified: Sat, 05 Nov 2022 02:38:14 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9c45749101c2502030b52b11f5cf1031d08ceabeab91283742467bdbe2dc62`  
		Last Modified: Sat, 05 Nov 2022 02:38:21 GMT  
		Size: 56.0 MB (56047607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2fa3febc47da546527aae2d8de736b7562b0e8f5a37a63778aa86307af8d2d`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d5e1d3c311ae16390016bcf09a400cc9e67473f8ea5787abe0855f510e917b`  
		Last Modified: Sat, 05 Nov 2022 02:38:23 GMT  
		Size: 55.1 MB (55068188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3db2c5d8ec681907739aa09873795aa7ffacfacfbd43d79f140331029f8517`  
		Last Modified: Sat, 05 Nov 2022 02:38:13 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ead729abd92d539d786eed0146f98fbfb8a970de2f0b082e9a0aa4ecc6d1fc`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a0b6340a3f236d39451f2373c5d137bf64eb54233163c186ef1480e8844f0ffd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159044836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b61a400e8776905c7164e1adcf7c9457bfe43dca3db94b667a3e4dd8e7f02c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 23:40:44 GMT
ADD file:44569001378d2d59b2d169aba48a6b2b88529ca46fd5d85598eff7ca37ded076 in / 
# Tue, 15 Nov 2022 23:40:45 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 01:33:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 16 Nov 2022 01:33:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 16 Nov 2022 01:33:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Nov 2022 01:33:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 16 Nov 2022 01:33:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:33:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 16 Nov 2022 01:34:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 16 Nov 2022 01:34:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 16 Nov 2022 01:34:16 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:34:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 16 Nov 2022 01:34:46 GMT
VOLUME [/var/lib/mysql]
# Wed, 16 Nov 2022 01:34:46 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 16 Nov 2022 01:34:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 16 Nov 2022 01:34:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 01:34:46 GMT
EXPOSE 3306 33060
# Wed, 16 Nov 2022 01:34:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01d65ebb4955ae24720eb5c24ff08081fed75975aea7b87c96ef7e58175901e0`  
		Last Modified: Tue, 15 Nov 2022 23:41:32 GMT  
		Size: 42.8 MB (42774711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d609fcc3c7fb5a4b262e7f8a002961e11802f03e441d9e8a2c1d0a03b606e1ee`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c09cdcd2da34e1fedf1e87c4cf449692e8fcd446a600a227ff7a3c678eba26`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 857.2 KB (857169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a478ef641e124539c75eca120d506f59fc5058ce27559d948305ec930643717`  
		Last Modified: Wed, 16 Nov 2022 01:35:15 GMT  
		Size: 4.5 MB (4465955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3956cc2f3fb1e3431a0db90666aa3e21c2015b9ddd6da49babc7bb389a09e8`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c37cc7a1914f1576343f24a780bedcdea90a844ccd62488df65355b06468fd`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0cd074dc147bcc06f8561f3added6b2ea97772000b3628f2e03503691904e0`  
		Last Modified: Wed, 16 Nov 2022 01:35:18 GMT  
		Size: 55.5 MB (55457981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9186a35382189d0459f0ce2a8166b45cbf2be5599cfe5716bdbc5de71ee3d2b2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443c4afe5f0f372b7558dc78484a7577e29c0d906b2e4324fbeb81d6bee853f`  
		Last Modified: Wed, 16 Nov 2022 01:35:20 GMT  
		Size: 55.5 MB (55479334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dbcd809e720177fc48884b92fb5e724ada0908ef9449445df4847f40a9c3d2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb36129f08c1e07dd8ad073c1fa8012fb05b03766001cbc228fbddc20edec95e`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
