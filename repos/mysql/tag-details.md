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
$ docker pull mysql@sha256:94176d0ad4ed85767fc0d74b8071387109a0390e7c1afd39788269c96d2dad74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:4ff8da589a6dd1ff2323a50b409575cb5ca7d5dd1169783a911476c757ed48f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144346386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262701d58edd77960f86dc48c4090fe972d329b9aba26788eff6c46c8bbbfb11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:32:03 GMT
ADD file:d7b7ed3315719e2a7f19233b68dbf42298d9d6e1a882de7154751ad29710eeac in / 
# Fri, 07 Oct 2022 20:32:03 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:07:13 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:07:13 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:07:16 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:07:35 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 07 Oct 2022 21:07:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:07:36 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 11 Oct 2022 20:29:54 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Tue, 11 Oct 2022 20:29:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 11 Oct 2022 20:30:13 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 11 Oct 2022 20:30:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 11 Oct 2022 20:30:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Tue, 11 Oct 2022 20:30:40 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 11 Oct 2022 20:30:41 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:30:41 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 20:30:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 20:30:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 20:30:42 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 20:30:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0056409b8e897373ba0cef19c5e1f387c06dafd5e11f3f2f0f22d34c8acb6717`  
		Last Modified: Fri, 07 Oct 2022 20:34:25 GMT  
		Size: 49.9 MB (49869229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219bd535343da2b375f2b97b3dbb9bafb7b73ed81a353dfe8f4cc8d07458e7c9`  
		Last Modified: Fri, 07 Oct 2022 21:09:28 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f220ee65eb90231c15c775fbeafd88aa10dc6840cf78a4b81fe0a509950f316d`  
		Last Modified: Fri, 07 Oct 2022 21:09:28 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbb395b2290fd2673caeb1b3d2fa4613fd74fb6e73327dc64b4d62c7b095bdb`  
		Last Modified: Fri, 07 Oct 2022 21:09:27 GMT  
		Size: 4.5 MB (4546582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645e487e5f0a70ac505c9c639fa41269beebe9c9bc3b0fe8806b224df42f0f62`  
		Last Modified: Fri, 07 Oct 2022 21:09:25 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fa38d2e1fbdcf43177247a8341f9fb5987ca1260a05dd1800eb0bea2cf60af`  
		Last Modified: Tue, 11 Oct 2022 20:33:03 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d9f4f7e8b404939e94555c990938ac92ebf5b6811c413a6cbced1125568e82`  
		Last Modified: Tue, 11 Oct 2022 20:33:05 GMT  
		Size: 25.5 MB (25530580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03fcfe5d90e3009534a22bac14c4fe1c7aedc3cfdd6a3205760e3eb50a66b81`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c4d4272e305eddda735964d9b3ec3e174e11efcb4fa6842c6922af8edac0b9`  
		Last Modified: Tue, 11 Oct 2022 20:33:12 GMT  
		Size: 63.5 MB (63460088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a8ad6eeebe68aa2729bf4325ccaebe03dfab39ed7eda5f3e39231dcaafd8e4`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919524a8718b6f154a115b2d995184e2362c8f03cc807b4722ecc42abbe3a2cd`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:e590a0c91b789b683a965fc07713df52a07352e4b7cb744633240bd6a26adca4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c628f772392369a2796350690755d1378dad89e26bf6ce96cb9f6ad1d2e2ac8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162584232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c18eb45f07cad6c6c289cbe3377ed6515e8cacbbe2ff0d3d3baf1f3d78c1229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:22:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Oct 2022 04:22:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:22:42 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Oct 2022 04:22:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 04:22:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 04:22:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:22:59 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 05 Oct 2022 04:22:59 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 11 Oct 2022 20:30:52 GMT
ENV MYSQL_VERSION=5.7.40-1debian10
# Tue, 11 Oct 2022 20:30:52 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 11 Oct 2022 20:31:15 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 11 Oct 2022 20:31:16 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:31:16 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 20:31:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 20:31:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 20:31:17 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 20:31:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a11d1b00d26182c3e9edb027d075aab8c6529517f09b58b9474b42e96b7282`  
		Last Modified: Wed, 05 Oct 2022 04:24:27 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65869aed91d26fee82355255ac43a74ad1b1efab8c4f9733cb985f5a65a215bc`  
		Last Modified: Wed, 05 Oct 2022 04:24:25 GMT  
		Size: 4.2 MB (4179215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b594fff16bcffe32ae29c2e6ef1d64e50b63c956002ed96f4aeb670ae2c9d15`  
		Last Modified: Wed, 05 Oct 2022 04:24:25 GMT  
		Size: 1.4 MB (1386660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46e1e42bcc85e082d51a8bdfde663ae17168e85c0773a7f9d7ffbacfc03abd4`  
		Last Modified: Wed, 05 Oct 2022 04:24:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ecc9da4c857053937cf0e8c8f6b93d1e20a238dc8986301597f014a58607ef`  
		Last Modified: Wed, 05 Oct 2022 04:24:28 GMT  
		Size: 14.1 MB (14086928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed6254a5eabd760fd83f3fe87470ef4c5d74e38809164e20d82ccea7403ad82`  
		Last Modified: Wed, 05 Oct 2022 04:24:23 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e6956b2984bd9420bd93fbf6ab3b0b6eb05e610a6cc63fc8a4361edea1ce76`  
		Last Modified: Tue, 11 Oct 2022 20:33:36 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3981ba85697c0896f2a3b11bebf494e3de8f006cd7a0c5704239dddfba3f1ce8`  
		Last Modified: Tue, 11 Oct 2022 20:33:51 GMT  
		Size: 115.8 MB (115783190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434009cd59041398592f7524b509c94dc271297ba8893ed401789a6e17612ab5`  
		Last Modified: Tue, 11 Oct 2022 20:33:36 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57a2382417ad6af5f0a2fcaa6e1a97c3ff9aeaa05e431a8cddedf9fb58fbfef`  
		Last Modified: Tue, 11 Oct 2022 20:33:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:94176d0ad4ed85767fc0d74b8071387109a0390e7c1afd39788269c96d2dad74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:4ff8da589a6dd1ff2323a50b409575cb5ca7d5dd1169783a911476c757ed48f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144346386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262701d58edd77960f86dc48c4090fe972d329b9aba26788eff6c46c8bbbfb11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:32:03 GMT
ADD file:d7b7ed3315719e2a7f19233b68dbf42298d9d6e1a882de7154751ad29710eeac in / 
# Fri, 07 Oct 2022 20:32:03 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:07:13 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:07:13 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:07:16 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:07:35 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 07 Oct 2022 21:07:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:07:36 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 11 Oct 2022 20:29:54 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Tue, 11 Oct 2022 20:29:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 11 Oct 2022 20:30:13 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 11 Oct 2022 20:30:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 11 Oct 2022 20:30:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Tue, 11 Oct 2022 20:30:40 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 11 Oct 2022 20:30:41 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:30:41 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 20:30:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 20:30:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 20:30:42 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 20:30:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0056409b8e897373ba0cef19c5e1f387c06dafd5e11f3f2f0f22d34c8acb6717`  
		Last Modified: Fri, 07 Oct 2022 20:34:25 GMT  
		Size: 49.9 MB (49869229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219bd535343da2b375f2b97b3dbb9bafb7b73ed81a353dfe8f4cc8d07458e7c9`  
		Last Modified: Fri, 07 Oct 2022 21:09:28 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f220ee65eb90231c15c775fbeafd88aa10dc6840cf78a4b81fe0a509950f316d`  
		Last Modified: Fri, 07 Oct 2022 21:09:28 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbb395b2290fd2673caeb1b3d2fa4613fd74fb6e73327dc64b4d62c7b095bdb`  
		Last Modified: Fri, 07 Oct 2022 21:09:27 GMT  
		Size: 4.5 MB (4546582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645e487e5f0a70ac505c9c639fa41269beebe9c9bc3b0fe8806b224df42f0f62`  
		Last Modified: Fri, 07 Oct 2022 21:09:25 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fa38d2e1fbdcf43177247a8341f9fb5987ca1260a05dd1800eb0bea2cf60af`  
		Last Modified: Tue, 11 Oct 2022 20:33:03 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d9f4f7e8b404939e94555c990938ac92ebf5b6811c413a6cbced1125568e82`  
		Last Modified: Tue, 11 Oct 2022 20:33:05 GMT  
		Size: 25.5 MB (25530580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03fcfe5d90e3009534a22bac14c4fe1c7aedc3cfdd6a3205760e3eb50a66b81`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c4d4272e305eddda735964d9b3ec3e174e11efcb4fa6842c6922af8edac0b9`  
		Last Modified: Tue, 11 Oct 2022 20:33:12 GMT  
		Size: 63.5 MB (63460088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a8ad6eeebe68aa2729bf4325ccaebe03dfab39ed7eda5f3e39231dcaafd8e4`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919524a8718b6f154a115b2d995184e2362c8f03cc807b4722ecc42abbe3a2cd`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:94176d0ad4ed85767fc0d74b8071387109a0390e7c1afd39788269c96d2dad74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:4ff8da589a6dd1ff2323a50b409575cb5ca7d5dd1169783a911476c757ed48f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144346386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262701d58edd77960f86dc48c4090fe972d329b9aba26788eff6c46c8bbbfb11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:32:03 GMT
ADD file:d7b7ed3315719e2a7f19233b68dbf42298d9d6e1a882de7154751ad29710eeac in / 
# Fri, 07 Oct 2022 20:32:03 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:07:13 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:07:13 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:07:16 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:07:35 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 07 Oct 2022 21:07:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:07:36 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 11 Oct 2022 20:29:54 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Tue, 11 Oct 2022 20:29:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 11 Oct 2022 20:30:13 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 11 Oct 2022 20:30:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 11 Oct 2022 20:30:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Tue, 11 Oct 2022 20:30:40 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 11 Oct 2022 20:30:41 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:30:41 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 20:30:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 20:30:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 20:30:42 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 20:30:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0056409b8e897373ba0cef19c5e1f387c06dafd5e11f3f2f0f22d34c8acb6717`  
		Last Modified: Fri, 07 Oct 2022 20:34:25 GMT  
		Size: 49.9 MB (49869229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219bd535343da2b375f2b97b3dbb9bafb7b73ed81a353dfe8f4cc8d07458e7c9`  
		Last Modified: Fri, 07 Oct 2022 21:09:28 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f220ee65eb90231c15c775fbeafd88aa10dc6840cf78a4b81fe0a509950f316d`  
		Last Modified: Fri, 07 Oct 2022 21:09:28 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbb395b2290fd2673caeb1b3d2fa4613fd74fb6e73327dc64b4d62c7b095bdb`  
		Last Modified: Fri, 07 Oct 2022 21:09:27 GMT  
		Size: 4.5 MB (4546582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645e487e5f0a70ac505c9c639fa41269beebe9c9bc3b0fe8806b224df42f0f62`  
		Last Modified: Fri, 07 Oct 2022 21:09:25 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fa38d2e1fbdcf43177247a8341f9fb5987ca1260a05dd1800eb0bea2cf60af`  
		Last Modified: Tue, 11 Oct 2022 20:33:03 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d9f4f7e8b404939e94555c990938ac92ebf5b6811c413a6cbced1125568e82`  
		Last Modified: Tue, 11 Oct 2022 20:33:05 GMT  
		Size: 25.5 MB (25530580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03fcfe5d90e3009534a22bac14c4fe1c7aedc3cfdd6a3205760e3eb50a66b81`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c4d4272e305eddda735964d9b3ec3e174e11efcb4fa6842c6922af8edac0b9`  
		Last Modified: Tue, 11 Oct 2022 20:33:12 GMT  
		Size: 63.5 MB (63460088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a8ad6eeebe68aa2729bf4325ccaebe03dfab39ed7eda5f3e39231dcaafd8e4`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919524a8718b6f154a115b2d995184e2362c8f03cc807b4722ecc42abbe3a2cd`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:e590a0c91b789b683a965fc07713df52a07352e4b7cb744633240bd6a26adca4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c628f772392369a2796350690755d1378dad89e26bf6ce96cb9f6ad1d2e2ac8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162584232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c18eb45f07cad6c6c289cbe3377ed6515e8cacbbe2ff0d3d3baf1f3d78c1229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:22:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Oct 2022 04:22:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:22:42 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Oct 2022 04:22:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 04:22:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 04:22:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:22:59 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 05 Oct 2022 04:22:59 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 11 Oct 2022 20:30:52 GMT
ENV MYSQL_VERSION=5.7.40-1debian10
# Tue, 11 Oct 2022 20:30:52 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 11 Oct 2022 20:31:15 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 11 Oct 2022 20:31:16 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:31:16 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 20:31:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 20:31:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 20:31:17 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 20:31:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a11d1b00d26182c3e9edb027d075aab8c6529517f09b58b9474b42e96b7282`  
		Last Modified: Wed, 05 Oct 2022 04:24:27 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65869aed91d26fee82355255ac43a74ad1b1efab8c4f9733cb985f5a65a215bc`  
		Last Modified: Wed, 05 Oct 2022 04:24:25 GMT  
		Size: 4.2 MB (4179215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b594fff16bcffe32ae29c2e6ef1d64e50b63c956002ed96f4aeb670ae2c9d15`  
		Last Modified: Wed, 05 Oct 2022 04:24:25 GMT  
		Size: 1.4 MB (1386660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46e1e42bcc85e082d51a8bdfde663ae17168e85c0773a7f9d7ffbacfc03abd4`  
		Last Modified: Wed, 05 Oct 2022 04:24:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ecc9da4c857053937cf0e8c8f6b93d1e20a238dc8986301597f014a58607ef`  
		Last Modified: Wed, 05 Oct 2022 04:24:28 GMT  
		Size: 14.1 MB (14086928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed6254a5eabd760fd83f3fe87470ef4c5d74e38809164e20d82ccea7403ad82`  
		Last Modified: Wed, 05 Oct 2022 04:24:23 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e6956b2984bd9420bd93fbf6ab3b0b6eb05e610a6cc63fc8a4361edea1ce76`  
		Last Modified: Tue, 11 Oct 2022 20:33:36 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3981ba85697c0896f2a3b11bebf494e3de8f006cd7a0c5704239dddfba3f1ce8`  
		Last Modified: Tue, 11 Oct 2022 20:33:51 GMT  
		Size: 115.8 MB (115783190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434009cd59041398592f7524b509c94dc271297ba8893ed401789a6e17612ab5`  
		Last Modified: Tue, 11 Oct 2022 20:33:36 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57a2382417ad6af5f0a2fcaa6e1a97c3ff9aeaa05e431a8cddedf9fb58fbfef`  
		Last Modified: Tue, 11 Oct 2022 20:33:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:94176d0ad4ed85767fc0d74b8071387109a0390e7c1afd39788269c96d2dad74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:4ff8da589a6dd1ff2323a50b409575cb5ca7d5dd1169783a911476c757ed48f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144346386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262701d58edd77960f86dc48c4090fe972d329b9aba26788eff6c46c8bbbfb11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:32:03 GMT
ADD file:d7b7ed3315719e2a7f19233b68dbf42298d9d6e1a882de7154751ad29710eeac in / 
# Fri, 07 Oct 2022 20:32:03 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:07:13 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:07:13 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:07:16 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:07:35 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 07 Oct 2022 21:07:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:07:36 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 11 Oct 2022 20:29:54 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Tue, 11 Oct 2022 20:29:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 11 Oct 2022 20:30:13 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 11 Oct 2022 20:30:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 11 Oct 2022 20:30:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Tue, 11 Oct 2022 20:30:40 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 11 Oct 2022 20:30:41 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:30:41 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 20:30:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 20:30:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 20:30:42 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 20:30:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0056409b8e897373ba0cef19c5e1f387c06dafd5e11f3f2f0f22d34c8acb6717`  
		Last Modified: Fri, 07 Oct 2022 20:34:25 GMT  
		Size: 49.9 MB (49869229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219bd535343da2b375f2b97b3dbb9bafb7b73ed81a353dfe8f4cc8d07458e7c9`  
		Last Modified: Fri, 07 Oct 2022 21:09:28 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f220ee65eb90231c15c775fbeafd88aa10dc6840cf78a4b81fe0a509950f316d`  
		Last Modified: Fri, 07 Oct 2022 21:09:28 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbb395b2290fd2673caeb1b3d2fa4613fd74fb6e73327dc64b4d62c7b095bdb`  
		Last Modified: Fri, 07 Oct 2022 21:09:27 GMT  
		Size: 4.5 MB (4546582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645e487e5f0a70ac505c9c639fa41269beebe9c9bc3b0fe8806b224df42f0f62`  
		Last Modified: Fri, 07 Oct 2022 21:09:25 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fa38d2e1fbdcf43177247a8341f9fb5987ca1260a05dd1800eb0bea2cf60af`  
		Last Modified: Tue, 11 Oct 2022 20:33:03 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d9f4f7e8b404939e94555c990938ac92ebf5b6811c413a6cbced1125568e82`  
		Last Modified: Tue, 11 Oct 2022 20:33:05 GMT  
		Size: 25.5 MB (25530580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03fcfe5d90e3009534a22bac14c4fe1c7aedc3cfdd6a3205760e3eb50a66b81`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c4d4272e305eddda735964d9b3ec3e174e11efcb4fa6842c6922af8edac0b9`  
		Last Modified: Tue, 11 Oct 2022 20:33:12 GMT  
		Size: 63.5 MB (63460088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a8ad6eeebe68aa2729bf4325ccaebe03dfab39ed7eda5f3e39231dcaafd8e4`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919524a8718b6f154a115b2d995184e2362c8f03cc807b4722ecc42abbe3a2cd`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40`

```console
$ docker pull mysql@sha256:94176d0ad4ed85767fc0d74b8071387109a0390e7c1afd39788269c96d2dad74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40` - linux; amd64

```console
$ docker pull mysql@sha256:4ff8da589a6dd1ff2323a50b409575cb5ca7d5dd1169783a911476c757ed48f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144346386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262701d58edd77960f86dc48c4090fe972d329b9aba26788eff6c46c8bbbfb11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:32:03 GMT
ADD file:d7b7ed3315719e2a7f19233b68dbf42298d9d6e1a882de7154751ad29710eeac in / 
# Fri, 07 Oct 2022 20:32:03 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:07:13 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:07:13 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:07:16 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:07:35 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 07 Oct 2022 21:07:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:07:36 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 11 Oct 2022 20:29:54 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Tue, 11 Oct 2022 20:29:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 11 Oct 2022 20:30:13 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 11 Oct 2022 20:30:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 11 Oct 2022 20:30:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Tue, 11 Oct 2022 20:30:40 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 11 Oct 2022 20:30:41 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:30:41 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 20:30:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 20:30:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 20:30:42 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 20:30:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0056409b8e897373ba0cef19c5e1f387c06dafd5e11f3f2f0f22d34c8acb6717`  
		Last Modified: Fri, 07 Oct 2022 20:34:25 GMT  
		Size: 49.9 MB (49869229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219bd535343da2b375f2b97b3dbb9bafb7b73ed81a353dfe8f4cc8d07458e7c9`  
		Last Modified: Fri, 07 Oct 2022 21:09:28 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f220ee65eb90231c15c775fbeafd88aa10dc6840cf78a4b81fe0a509950f316d`  
		Last Modified: Fri, 07 Oct 2022 21:09:28 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbb395b2290fd2673caeb1b3d2fa4613fd74fb6e73327dc64b4d62c7b095bdb`  
		Last Modified: Fri, 07 Oct 2022 21:09:27 GMT  
		Size: 4.5 MB (4546582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645e487e5f0a70ac505c9c639fa41269beebe9c9bc3b0fe8806b224df42f0f62`  
		Last Modified: Fri, 07 Oct 2022 21:09:25 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fa38d2e1fbdcf43177247a8341f9fb5987ca1260a05dd1800eb0bea2cf60af`  
		Last Modified: Tue, 11 Oct 2022 20:33:03 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d9f4f7e8b404939e94555c990938ac92ebf5b6811c413a6cbced1125568e82`  
		Last Modified: Tue, 11 Oct 2022 20:33:05 GMT  
		Size: 25.5 MB (25530580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03fcfe5d90e3009534a22bac14c4fe1c7aedc3cfdd6a3205760e3eb50a66b81`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c4d4272e305eddda735964d9b3ec3e174e11efcb4fa6842c6922af8edac0b9`  
		Last Modified: Tue, 11 Oct 2022 20:33:12 GMT  
		Size: 63.5 MB (63460088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a8ad6eeebe68aa2729bf4325ccaebe03dfab39ed7eda5f3e39231dcaafd8e4`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919524a8718b6f154a115b2d995184e2362c8f03cc807b4722ecc42abbe3a2cd`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40-debian`

```console
$ docker pull mysql@sha256:e590a0c91b789b683a965fc07713df52a07352e4b7cb744633240bd6a26adca4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c628f772392369a2796350690755d1378dad89e26bf6ce96cb9f6ad1d2e2ac8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162584232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c18eb45f07cad6c6c289cbe3377ed6515e8cacbbe2ff0d3d3baf1f3d78c1229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:22:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Oct 2022 04:22:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:22:42 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Oct 2022 04:22:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 04:22:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 04:22:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:22:59 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 05 Oct 2022 04:22:59 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 11 Oct 2022 20:30:52 GMT
ENV MYSQL_VERSION=5.7.40-1debian10
# Tue, 11 Oct 2022 20:30:52 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 11 Oct 2022 20:31:15 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 11 Oct 2022 20:31:16 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:31:16 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 20:31:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 20:31:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 20:31:17 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 20:31:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a11d1b00d26182c3e9edb027d075aab8c6529517f09b58b9474b42e96b7282`  
		Last Modified: Wed, 05 Oct 2022 04:24:27 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65869aed91d26fee82355255ac43a74ad1b1efab8c4f9733cb985f5a65a215bc`  
		Last Modified: Wed, 05 Oct 2022 04:24:25 GMT  
		Size: 4.2 MB (4179215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b594fff16bcffe32ae29c2e6ef1d64e50b63c956002ed96f4aeb670ae2c9d15`  
		Last Modified: Wed, 05 Oct 2022 04:24:25 GMT  
		Size: 1.4 MB (1386660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46e1e42bcc85e082d51a8bdfde663ae17168e85c0773a7f9d7ffbacfc03abd4`  
		Last Modified: Wed, 05 Oct 2022 04:24:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ecc9da4c857053937cf0e8c8f6b93d1e20a238dc8986301597f014a58607ef`  
		Last Modified: Wed, 05 Oct 2022 04:24:28 GMT  
		Size: 14.1 MB (14086928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed6254a5eabd760fd83f3fe87470ef4c5d74e38809164e20d82ccea7403ad82`  
		Last Modified: Wed, 05 Oct 2022 04:24:23 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e6956b2984bd9420bd93fbf6ab3b0b6eb05e610a6cc63fc8a4361edea1ce76`  
		Last Modified: Tue, 11 Oct 2022 20:33:36 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3981ba85697c0896f2a3b11bebf494e3de8f006cd7a0c5704239dddfba3f1ce8`  
		Last Modified: Tue, 11 Oct 2022 20:33:51 GMT  
		Size: 115.8 MB (115783190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434009cd59041398592f7524b509c94dc271297ba8893ed401789a6e17612ab5`  
		Last Modified: Tue, 11 Oct 2022 20:33:36 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57a2382417ad6af5f0a2fcaa6e1a97c3ff9aeaa05e431a8cddedf9fb58fbfef`  
		Last Modified: Tue, 11 Oct 2022 20:33:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40-oracle`

```console
$ docker pull mysql@sha256:94176d0ad4ed85767fc0d74b8071387109a0390e7c1afd39788269c96d2dad74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:4ff8da589a6dd1ff2323a50b409575cb5ca7d5dd1169783a911476c757ed48f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144346386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262701d58edd77960f86dc48c4090fe972d329b9aba26788eff6c46c8bbbfb11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:32:03 GMT
ADD file:d7b7ed3315719e2a7f19233b68dbf42298d9d6e1a882de7154751ad29710eeac in / 
# Fri, 07 Oct 2022 20:32:03 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:07:13 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:07:13 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:07:16 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:07:35 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 07 Oct 2022 21:07:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:07:36 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 11 Oct 2022 20:29:54 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Tue, 11 Oct 2022 20:29:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 11 Oct 2022 20:30:13 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 11 Oct 2022 20:30:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 11 Oct 2022 20:30:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Tue, 11 Oct 2022 20:30:40 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 11 Oct 2022 20:30:41 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:30:41 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 20:30:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 20:30:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 20:30:42 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 20:30:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0056409b8e897373ba0cef19c5e1f387c06dafd5e11f3f2f0f22d34c8acb6717`  
		Last Modified: Fri, 07 Oct 2022 20:34:25 GMT  
		Size: 49.9 MB (49869229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219bd535343da2b375f2b97b3dbb9bafb7b73ed81a353dfe8f4cc8d07458e7c9`  
		Last Modified: Fri, 07 Oct 2022 21:09:28 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f220ee65eb90231c15c775fbeafd88aa10dc6840cf78a4b81fe0a509950f316d`  
		Last Modified: Fri, 07 Oct 2022 21:09:28 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbb395b2290fd2673caeb1b3d2fa4613fd74fb6e73327dc64b4d62c7b095bdb`  
		Last Modified: Fri, 07 Oct 2022 21:09:27 GMT  
		Size: 4.5 MB (4546582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645e487e5f0a70ac505c9c639fa41269beebe9c9bc3b0fe8806b224df42f0f62`  
		Last Modified: Fri, 07 Oct 2022 21:09:25 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fa38d2e1fbdcf43177247a8341f9fb5987ca1260a05dd1800eb0bea2cf60af`  
		Last Modified: Tue, 11 Oct 2022 20:33:03 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d9f4f7e8b404939e94555c990938ac92ebf5b6811c413a6cbced1125568e82`  
		Last Modified: Tue, 11 Oct 2022 20:33:05 GMT  
		Size: 25.5 MB (25530580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03fcfe5d90e3009534a22bac14c4fe1c7aedc3cfdd6a3205760e3eb50a66b81`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c4d4272e305eddda735964d9b3ec3e174e11efcb4fa6842c6922af8edac0b9`  
		Last Modified: Tue, 11 Oct 2022 20:33:12 GMT  
		Size: 63.5 MB (63460088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a8ad6eeebe68aa2729bf4325ccaebe03dfab39ed7eda5f3e39231dcaafd8e4`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919524a8718b6f154a115b2d995184e2362c8f03cc807b4722ecc42abbe3a2cd`  
		Last Modified: Tue, 11 Oct 2022 20:33:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:147572c972192417add6f1cf65ea33edfd44086e461a3381601b53e1662f5d15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:fb3d8639a938515aaac38acb13c4acc061366a20322c55bbedae9d127cd2f2b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157265417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b83de8fb1a29d9b47d3ecbff86f67d22f8418f6e6ef5d349aaca2c2919074a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 21:20:42 GMT
ADD file:ceac4c0bc6dd71b3868d5af15bdaab832a2f61b45c12116b2df42ef8cfbf9fa1 in / 
# Wed, 12 Oct 2022 21:20:42 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:37:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:37:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:37:33 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:37:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:37:57 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:37:58 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:38:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:38:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:38:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:39:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:39:04 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:39:04 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:39:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:39:05 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:39:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ed150ed0abef03007b46722de75bcb3e517f22532a46146fcec4fb1761d4347`  
		Last Modified: Wed, 12 Oct 2022 21:22:08 GMT  
		Size: 40.6 MB (40589408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fede58e17ac8f886aa620315c1c85d2979e38aa05aebf00aacba6d240a18620`  
		Last Modified: Wed, 12 Oct 2022 21:39:40 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994a6ddd6efe5eef3b2be88576cfa2e823d47f0c7db10554360438631d0f786b`  
		Last Modified: Wed, 12 Oct 2022 21:39:41 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028bda79779b4b2f4b249922d92841289aeae64aea45154be16cd17cfe986fdd`  
		Last Modified: Wed, 12 Oct 2022 21:39:39 GMT  
		Size: 4.6 MB (4606927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426fbe9e56a28ac107f62e7fb3b835c320ff0997c762490c853ae8242765da9f`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a00e58dd193f3585ff724fd8ba4f7c78d83cf33b851a186b925b36317542f34`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4f64494005d7365861de3808b1c39783259162154a12b6b6694e5303732c2b`  
		Last Modified: Wed, 12 Oct 2022 21:39:45 GMT  
		Size: 56.0 MB (56046404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba8ab3534a7c32755a032486836b05d3d5a724ba6e7127ce259a0ea02fae975`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695938edf88c0409d640f6edcb00898d28478ed80505fd449f6c05c2b99ec3d`  
		Last Modified: Wed, 12 Oct 2022 21:39:46 GMT  
		Size: 55.1 MB (55084174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3754e2587bed8ece9b5713bcb14924d27691927399a3750fb6d8ebceb000d771`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f154543e74f792239c3ac5377c8deb20f3956a8e60db04486c4313c0979d7`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:4a90a0b47798672d3e19064171610cd055cb1d5b702dcf67d6c675c9cb61a96d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155564637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262f364f4f01337f2027e10c7ca2994dc28883afb24386100c89351126d76fe4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 20:40:56 GMT
ADD file:049ff2e28998fde860d1a12f43ec245d10345a71953f67108180c23c237ce26e in / 
# Wed, 12 Oct 2022 20:40:56 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:24:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:24:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:24:47 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:25:15 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:25:17 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:25:18 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:25:19 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:25:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:25:52 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:25:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:25:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:26:33 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:26:34 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:26:36 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:26:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:26:38 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:26:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:828689dcde4b0fe396ab27cf3a6d5f71ee01d48891421ec4381d74ed415be5d0`  
		Last Modified: Wed, 12 Oct 2022 20:42:33 GMT  
		Size: 39.4 MB (39409290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f061378e43d33dc614866c620ab52f8985729cda946779352b12f6a73d099d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1a79ec4c767ad1034121ce2905bb5a3326d01d2c3e24a384b55d34a923bcba`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 857.1 KB (857150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29639854082a90b6e050d61546185cee56cbc0a0224e0a37222ab57bd00917d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:18 GMT  
		Size: 4.4 MB (4433340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be1d8abaf67b766b14bd7b5ee219ce3181b651617cede1fbef78809e83ae2f3`  
		Last Modified: Wed, 12 Oct 2022 21:27:17 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862924992b62147c16c1cad215c391bd43f107b291971074dda31445e6171439`  
		Last Modified: Wed, 12 Oct 2022 21:27:15 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8afc4c260a8060504c3a8696a68694051c62b5dad9774d6b95cc57e9cc10c7`  
		Last Modified: Wed, 12 Oct 2022 21:27:21 GMT  
		Size: 55.4 MB (55421557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb5afa1cf8a3c9f31ed89a4b56cdf88a1d9638c5cadbfc1d8e971265c90892b`  
		Last Modified: Wed, 12 Oct 2022 21:27:13 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693834f1d9bae56fd201dd9a4d7b2eadf83d04d230f650f0c1948876324517e8`  
		Last Modified: Wed, 12 Oct 2022 21:27:23 GMT  
		Size: 55.4 MB (55433646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3411c71dcce2f58523c25058a0800a7e635b92e410e805a30120b936e51a2cb8`  
		Last Modified: Wed, 12 Oct 2022 21:27:16 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877257953583c21228d6fcef6578b5bdfe8729c7f6ee6b366bade14693a92fa5`  
		Last Modified: Wed, 12 Oct 2022 21:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:159ec35fdd08e138171efa47528aa6a5b683fd769e21378f54f0596a3fea3a4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:151ed8848186e29228574349982a0fdabda35a49452f0da8d1d64488f7e1ccc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177571480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b60588a78bb65c66fde258cd85570c6e8d4bbc637e798a0cc011a463effcf92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:21:45 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Oct 2022 04:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:21:51 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Oct 2022 04:22:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 04:22:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 04:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:22:07 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 05 Oct 2022 04:22:07 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 11 Oct 2022 20:29:30 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Tue, 11 Oct 2022 20:29:31 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 11 Oct 2022 20:29:47 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 11 Oct 2022 20:29:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:29:48 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 11 Oct 2022 20:29:48 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 20:29:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 20:29:49 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 20:29:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f498ba1a3ae2dfa82359e0fb959af536134a1360d33dfa87638e409b70b3fa3`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c224eff0af51a4254bf410ca8f6cab7044171639fc6e7b29cd55248bb609d02`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 4.4 MB (4414808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acdd40c1260704addfdb3a21bf71ae5c14567100f98acd4d8dfec303294e1c5f`  
		Last Modified: Wed, 05 Oct 2022 04:23:50 GMT  
		Size: 1.4 MB (1418452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c3ece0305cbf295220adfdacf8c9e9fdf5de35ea07e505913ea4ee6e1f4f74`  
		Last Modified: Wed, 05 Oct 2022 04:23:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a10286651685e256e36f218063406728987d0f36c285adf41d41f8665661b74`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 12.7 MB (12661783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a34b42ee331888b70b38f6c96cacce54fe2bb4cf6e2ccefdd7add2144d5a3e`  
		Last Modified: Wed, 05 Oct 2022 04:23:49 GMT  
		Size: 2.5 KB (2546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5d04bddbd0c7caeacce07fffaa07f1b523fe80e9415cc5c88fe8387468c2ec`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b2bd56df6d823af6ff936600b456e3a7e94bbab1df9a52b59df7ed84c832d`  
		Last Modified: Tue, 11 Oct 2022 20:32:43 GMT  
		Size: 127.6 MB (127645294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ca09d481ffc70add23e3d81c2a8d0bf7c30928edf8650a3cd3464c14022eb6`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5840a45093cbfdd7cab682cbf5b5f879086883904300f5dfe84441a0129bfe6`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6e4d6f9231e9ee88d7085aa68eac1de6d4789d9508824387327e8db28ce074`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:147572c972192417add6f1cf65ea33edfd44086e461a3381601b53e1662f5d15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:fb3d8639a938515aaac38acb13c4acc061366a20322c55bbedae9d127cd2f2b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157265417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b83de8fb1a29d9b47d3ecbff86f67d22f8418f6e6ef5d349aaca2c2919074a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 21:20:42 GMT
ADD file:ceac4c0bc6dd71b3868d5af15bdaab832a2f61b45c12116b2df42ef8cfbf9fa1 in / 
# Wed, 12 Oct 2022 21:20:42 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:37:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:37:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:37:33 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:37:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:37:57 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:37:58 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:38:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:38:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:38:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:39:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:39:04 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:39:04 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:39:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:39:05 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:39:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ed150ed0abef03007b46722de75bcb3e517f22532a46146fcec4fb1761d4347`  
		Last Modified: Wed, 12 Oct 2022 21:22:08 GMT  
		Size: 40.6 MB (40589408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fede58e17ac8f886aa620315c1c85d2979e38aa05aebf00aacba6d240a18620`  
		Last Modified: Wed, 12 Oct 2022 21:39:40 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994a6ddd6efe5eef3b2be88576cfa2e823d47f0c7db10554360438631d0f786b`  
		Last Modified: Wed, 12 Oct 2022 21:39:41 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028bda79779b4b2f4b249922d92841289aeae64aea45154be16cd17cfe986fdd`  
		Last Modified: Wed, 12 Oct 2022 21:39:39 GMT  
		Size: 4.6 MB (4606927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426fbe9e56a28ac107f62e7fb3b835c320ff0997c762490c853ae8242765da9f`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a00e58dd193f3585ff724fd8ba4f7c78d83cf33b851a186b925b36317542f34`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4f64494005d7365861de3808b1c39783259162154a12b6b6694e5303732c2b`  
		Last Modified: Wed, 12 Oct 2022 21:39:45 GMT  
		Size: 56.0 MB (56046404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba8ab3534a7c32755a032486836b05d3d5a724ba6e7127ce259a0ea02fae975`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695938edf88c0409d640f6edcb00898d28478ed80505fd449f6c05c2b99ec3d`  
		Last Modified: Wed, 12 Oct 2022 21:39:46 GMT  
		Size: 55.1 MB (55084174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3754e2587bed8ece9b5713bcb14924d27691927399a3750fb6d8ebceb000d771`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f154543e74f792239c3ac5377c8deb20f3956a8e60db04486c4313c0979d7`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:4a90a0b47798672d3e19064171610cd055cb1d5b702dcf67d6c675c9cb61a96d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155564637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262f364f4f01337f2027e10c7ca2994dc28883afb24386100c89351126d76fe4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 20:40:56 GMT
ADD file:049ff2e28998fde860d1a12f43ec245d10345a71953f67108180c23c237ce26e in / 
# Wed, 12 Oct 2022 20:40:56 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:24:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:24:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:24:47 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:25:15 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:25:17 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:25:18 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:25:19 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:25:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:25:52 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:25:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:25:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:26:33 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:26:34 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:26:36 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:26:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:26:38 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:26:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:828689dcde4b0fe396ab27cf3a6d5f71ee01d48891421ec4381d74ed415be5d0`  
		Last Modified: Wed, 12 Oct 2022 20:42:33 GMT  
		Size: 39.4 MB (39409290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f061378e43d33dc614866c620ab52f8985729cda946779352b12f6a73d099d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1a79ec4c767ad1034121ce2905bb5a3326d01d2c3e24a384b55d34a923bcba`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 857.1 KB (857150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29639854082a90b6e050d61546185cee56cbc0a0224e0a37222ab57bd00917d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:18 GMT  
		Size: 4.4 MB (4433340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be1d8abaf67b766b14bd7b5ee219ce3181b651617cede1fbef78809e83ae2f3`  
		Last Modified: Wed, 12 Oct 2022 21:27:17 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862924992b62147c16c1cad215c391bd43f107b291971074dda31445e6171439`  
		Last Modified: Wed, 12 Oct 2022 21:27:15 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8afc4c260a8060504c3a8696a68694051c62b5dad9774d6b95cc57e9cc10c7`  
		Last Modified: Wed, 12 Oct 2022 21:27:21 GMT  
		Size: 55.4 MB (55421557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb5afa1cf8a3c9f31ed89a4b56cdf88a1d9638c5cadbfc1d8e971265c90892b`  
		Last Modified: Wed, 12 Oct 2022 21:27:13 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693834f1d9bae56fd201dd9a4d7b2eadf83d04d230f650f0c1948876324517e8`  
		Last Modified: Wed, 12 Oct 2022 21:27:23 GMT  
		Size: 55.4 MB (55433646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3411c71dcce2f58523c25058a0800a7e635b92e410e805a30120b936e51a2cb8`  
		Last Modified: Wed, 12 Oct 2022 21:27:16 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877257953583c21228d6fcef6578b5bdfe8729c7f6ee6b366bade14693a92fa5`  
		Last Modified: Wed, 12 Oct 2022 21:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:147572c972192417add6f1cf65ea33edfd44086e461a3381601b53e1662f5d15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:fb3d8639a938515aaac38acb13c4acc061366a20322c55bbedae9d127cd2f2b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157265417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b83de8fb1a29d9b47d3ecbff86f67d22f8418f6e6ef5d349aaca2c2919074a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 21:20:42 GMT
ADD file:ceac4c0bc6dd71b3868d5af15bdaab832a2f61b45c12116b2df42ef8cfbf9fa1 in / 
# Wed, 12 Oct 2022 21:20:42 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:37:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:37:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:37:33 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:37:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:37:57 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:37:58 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:38:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:38:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:38:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:39:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:39:04 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:39:04 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:39:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:39:05 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:39:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ed150ed0abef03007b46722de75bcb3e517f22532a46146fcec4fb1761d4347`  
		Last Modified: Wed, 12 Oct 2022 21:22:08 GMT  
		Size: 40.6 MB (40589408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fede58e17ac8f886aa620315c1c85d2979e38aa05aebf00aacba6d240a18620`  
		Last Modified: Wed, 12 Oct 2022 21:39:40 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994a6ddd6efe5eef3b2be88576cfa2e823d47f0c7db10554360438631d0f786b`  
		Last Modified: Wed, 12 Oct 2022 21:39:41 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028bda79779b4b2f4b249922d92841289aeae64aea45154be16cd17cfe986fdd`  
		Last Modified: Wed, 12 Oct 2022 21:39:39 GMT  
		Size: 4.6 MB (4606927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426fbe9e56a28ac107f62e7fb3b835c320ff0997c762490c853ae8242765da9f`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a00e58dd193f3585ff724fd8ba4f7c78d83cf33b851a186b925b36317542f34`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4f64494005d7365861de3808b1c39783259162154a12b6b6694e5303732c2b`  
		Last Modified: Wed, 12 Oct 2022 21:39:45 GMT  
		Size: 56.0 MB (56046404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba8ab3534a7c32755a032486836b05d3d5a724ba6e7127ce259a0ea02fae975`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695938edf88c0409d640f6edcb00898d28478ed80505fd449f6c05c2b99ec3d`  
		Last Modified: Wed, 12 Oct 2022 21:39:46 GMT  
		Size: 55.1 MB (55084174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3754e2587bed8ece9b5713bcb14924d27691927399a3750fb6d8ebceb000d771`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f154543e74f792239c3ac5377c8deb20f3956a8e60db04486c4313c0979d7`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:4a90a0b47798672d3e19064171610cd055cb1d5b702dcf67d6c675c9cb61a96d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155564637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262f364f4f01337f2027e10c7ca2994dc28883afb24386100c89351126d76fe4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 20:40:56 GMT
ADD file:049ff2e28998fde860d1a12f43ec245d10345a71953f67108180c23c237ce26e in / 
# Wed, 12 Oct 2022 20:40:56 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:24:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:24:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:24:47 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:25:15 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:25:17 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:25:18 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:25:19 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:25:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:25:52 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:25:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:25:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:26:33 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:26:34 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:26:36 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:26:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:26:38 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:26:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:828689dcde4b0fe396ab27cf3a6d5f71ee01d48891421ec4381d74ed415be5d0`  
		Last Modified: Wed, 12 Oct 2022 20:42:33 GMT  
		Size: 39.4 MB (39409290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f061378e43d33dc614866c620ab52f8985729cda946779352b12f6a73d099d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1a79ec4c767ad1034121ce2905bb5a3326d01d2c3e24a384b55d34a923bcba`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 857.1 KB (857150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29639854082a90b6e050d61546185cee56cbc0a0224e0a37222ab57bd00917d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:18 GMT  
		Size: 4.4 MB (4433340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be1d8abaf67b766b14bd7b5ee219ce3181b651617cede1fbef78809e83ae2f3`  
		Last Modified: Wed, 12 Oct 2022 21:27:17 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862924992b62147c16c1cad215c391bd43f107b291971074dda31445e6171439`  
		Last Modified: Wed, 12 Oct 2022 21:27:15 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8afc4c260a8060504c3a8696a68694051c62b5dad9774d6b95cc57e9cc10c7`  
		Last Modified: Wed, 12 Oct 2022 21:27:21 GMT  
		Size: 55.4 MB (55421557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb5afa1cf8a3c9f31ed89a4b56cdf88a1d9638c5cadbfc1d8e971265c90892b`  
		Last Modified: Wed, 12 Oct 2022 21:27:13 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693834f1d9bae56fd201dd9a4d7b2eadf83d04d230f650f0c1948876324517e8`  
		Last Modified: Wed, 12 Oct 2022 21:27:23 GMT  
		Size: 55.4 MB (55433646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3411c71dcce2f58523c25058a0800a7e635b92e410e805a30120b936e51a2cb8`  
		Last Modified: Wed, 12 Oct 2022 21:27:16 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877257953583c21228d6fcef6578b5bdfe8729c7f6ee6b366bade14693a92fa5`  
		Last Modified: Wed, 12 Oct 2022 21:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:159ec35fdd08e138171efa47528aa6a5b683fd769e21378f54f0596a3fea3a4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:151ed8848186e29228574349982a0fdabda35a49452f0da8d1d64488f7e1ccc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177571480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b60588a78bb65c66fde258cd85570c6e8d4bbc637e798a0cc011a463effcf92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:21:45 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Oct 2022 04:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:21:51 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Oct 2022 04:22:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 04:22:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 04:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:22:07 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 05 Oct 2022 04:22:07 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 11 Oct 2022 20:29:30 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Tue, 11 Oct 2022 20:29:31 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 11 Oct 2022 20:29:47 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 11 Oct 2022 20:29:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:29:48 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 11 Oct 2022 20:29:48 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 20:29:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 20:29:49 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 20:29:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f498ba1a3ae2dfa82359e0fb959af536134a1360d33dfa87638e409b70b3fa3`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c224eff0af51a4254bf410ca8f6cab7044171639fc6e7b29cd55248bb609d02`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 4.4 MB (4414808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acdd40c1260704addfdb3a21bf71ae5c14567100f98acd4d8dfec303294e1c5f`  
		Last Modified: Wed, 05 Oct 2022 04:23:50 GMT  
		Size: 1.4 MB (1418452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c3ece0305cbf295220adfdacf8c9e9fdf5de35ea07e505913ea4ee6e1f4f74`  
		Last Modified: Wed, 05 Oct 2022 04:23:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a10286651685e256e36f218063406728987d0f36c285adf41d41f8665661b74`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 12.7 MB (12661783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a34b42ee331888b70b38f6c96cacce54fe2bb4cf6e2ccefdd7add2144d5a3e`  
		Last Modified: Wed, 05 Oct 2022 04:23:49 GMT  
		Size: 2.5 KB (2546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5d04bddbd0c7caeacce07fffaa07f1b523fe80e9415cc5c88fe8387468c2ec`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b2bd56df6d823af6ff936600b456e3a7e94bbab1df9a52b59df7ed84c832d`  
		Last Modified: Tue, 11 Oct 2022 20:32:43 GMT  
		Size: 127.6 MB (127645294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ca09d481ffc70add23e3d81c2a8d0bf7c30928edf8650a3cd3464c14022eb6`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5840a45093cbfdd7cab682cbf5b5f879086883904300f5dfe84441a0129bfe6`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6e4d6f9231e9ee88d7085aa68eac1de6d4789d9508824387327e8db28ce074`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:147572c972192417add6f1cf65ea33edfd44086e461a3381601b53e1662f5d15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:fb3d8639a938515aaac38acb13c4acc061366a20322c55bbedae9d127cd2f2b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157265417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b83de8fb1a29d9b47d3ecbff86f67d22f8418f6e6ef5d349aaca2c2919074a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 21:20:42 GMT
ADD file:ceac4c0bc6dd71b3868d5af15bdaab832a2f61b45c12116b2df42ef8cfbf9fa1 in / 
# Wed, 12 Oct 2022 21:20:42 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:37:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:37:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:37:33 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:37:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:37:57 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:37:58 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:38:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:38:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:38:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:39:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:39:04 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:39:04 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:39:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:39:05 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:39:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ed150ed0abef03007b46722de75bcb3e517f22532a46146fcec4fb1761d4347`  
		Last Modified: Wed, 12 Oct 2022 21:22:08 GMT  
		Size: 40.6 MB (40589408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fede58e17ac8f886aa620315c1c85d2979e38aa05aebf00aacba6d240a18620`  
		Last Modified: Wed, 12 Oct 2022 21:39:40 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994a6ddd6efe5eef3b2be88576cfa2e823d47f0c7db10554360438631d0f786b`  
		Last Modified: Wed, 12 Oct 2022 21:39:41 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028bda79779b4b2f4b249922d92841289aeae64aea45154be16cd17cfe986fdd`  
		Last Modified: Wed, 12 Oct 2022 21:39:39 GMT  
		Size: 4.6 MB (4606927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426fbe9e56a28ac107f62e7fb3b835c320ff0997c762490c853ae8242765da9f`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a00e58dd193f3585ff724fd8ba4f7c78d83cf33b851a186b925b36317542f34`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4f64494005d7365861de3808b1c39783259162154a12b6b6694e5303732c2b`  
		Last Modified: Wed, 12 Oct 2022 21:39:45 GMT  
		Size: 56.0 MB (56046404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba8ab3534a7c32755a032486836b05d3d5a724ba6e7127ce259a0ea02fae975`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695938edf88c0409d640f6edcb00898d28478ed80505fd449f6c05c2b99ec3d`  
		Last Modified: Wed, 12 Oct 2022 21:39:46 GMT  
		Size: 55.1 MB (55084174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3754e2587bed8ece9b5713bcb14924d27691927399a3750fb6d8ebceb000d771`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f154543e74f792239c3ac5377c8deb20f3956a8e60db04486c4313c0979d7`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:4a90a0b47798672d3e19064171610cd055cb1d5b702dcf67d6c675c9cb61a96d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155564637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262f364f4f01337f2027e10c7ca2994dc28883afb24386100c89351126d76fe4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 20:40:56 GMT
ADD file:049ff2e28998fde860d1a12f43ec245d10345a71953f67108180c23c237ce26e in / 
# Wed, 12 Oct 2022 20:40:56 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:24:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:24:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:24:47 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:25:15 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:25:17 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:25:18 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:25:19 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:25:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:25:52 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:25:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:25:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:26:33 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:26:34 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:26:36 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:26:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:26:38 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:26:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:828689dcde4b0fe396ab27cf3a6d5f71ee01d48891421ec4381d74ed415be5d0`  
		Last Modified: Wed, 12 Oct 2022 20:42:33 GMT  
		Size: 39.4 MB (39409290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f061378e43d33dc614866c620ab52f8985729cda946779352b12f6a73d099d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1a79ec4c767ad1034121ce2905bb5a3326d01d2c3e24a384b55d34a923bcba`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 857.1 KB (857150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29639854082a90b6e050d61546185cee56cbc0a0224e0a37222ab57bd00917d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:18 GMT  
		Size: 4.4 MB (4433340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be1d8abaf67b766b14bd7b5ee219ce3181b651617cede1fbef78809e83ae2f3`  
		Last Modified: Wed, 12 Oct 2022 21:27:17 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862924992b62147c16c1cad215c391bd43f107b291971074dda31445e6171439`  
		Last Modified: Wed, 12 Oct 2022 21:27:15 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8afc4c260a8060504c3a8696a68694051c62b5dad9774d6b95cc57e9cc10c7`  
		Last Modified: Wed, 12 Oct 2022 21:27:21 GMT  
		Size: 55.4 MB (55421557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb5afa1cf8a3c9f31ed89a4b56cdf88a1d9638c5cadbfc1d8e971265c90892b`  
		Last Modified: Wed, 12 Oct 2022 21:27:13 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693834f1d9bae56fd201dd9a4d7b2eadf83d04d230f650f0c1948876324517e8`  
		Last Modified: Wed, 12 Oct 2022 21:27:23 GMT  
		Size: 55.4 MB (55433646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3411c71dcce2f58523c25058a0800a7e635b92e410e805a30120b936e51a2cb8`  
		Last Modified: Wed, 12 Oct 2022 21:27:16 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877257953583c21228d6fcef6578b5bdfe8729c7f6ee6b366bade14693a92fa5`  
		Last Modified: Wed, 12 Oct 2022 21:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31`

```console
$ docker pull mysql@sha256:147572c972192417add6f1cf65ea33edfd44086e461a3381601b53e1662f5d15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.31` - linux; amd64

```console
$ docker pull mysql@sha256:fb3d8639a938515aaac38acb13c4acc061366a20322c55bbedae9d127cd2f2b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157265417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b83de8fb1a29d9b47d3ecbff86f67d22f8418f6e6ef5d349aaca2c2919074a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 21:20:42 GMT
ADD file:ceac4c0bc6dd71b3868d5af15bdaab832a2f61b45c12116b2df42ef8cfbf9fa1 in / 
# Wed, 12 Oct 2022 21:20:42 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:37:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:37:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:37:33 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:37:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:37:57 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:37:58 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:38:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:38:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:38:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:39:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:39:04 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:39:04 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:39:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:39:05 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:39:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ed150ed0abef03007b46722de75bcb3e517f22532a46146fcec4fb1761d4347`  
		Last Modified: Wed, 12 Oct 2022 21:22:08 GMT  
		Size: 40.6 MB (40589408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fede58e17ac8f886aa620315c1c85d2979e38aa05aebf00aacba6d240a18620`  
		Last Modified: Wed, 12 Oct 2022 21:39:40 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994a6ddd6efe5eef3b2be88576cfa2e823d47f0c7db10554360438631d0f786b`  
		Last Modified: Wed, 12 Oct 2022 21:39:41 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028bda79779b4b2f4b249922d92841289aeae64aea45154be16cd17cfe986fdd`  
		Last Modified: Wed, 12 Oct 2022 21:39:39 GMT  
		Size: 4.6 MB (4606927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426fbe9e56a28ac107f62e7fb3b835c320ff0997c762490c853ae8242765da9f`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a00e58dd193f3585ff724fd8ba4f7c78d83cf33b851a186b925b36317542f34`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4f64494005d7365861de3808b1c39783259162154a12b6b6694e5303732c2b`  
		Last Modified: Wed, 12 Oct 2022 21:39:45 GMT  
		Size: 56.0 MB (56046404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba8ab3534a7c32755a032486836b05d3d5a724ba6e7127ce259a0ea02fae975`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695938edf88c0409d640f6edcb00898d28478ed80505fd449f6c05c2b99ec3d`  
		Last Modified: Wed, 12 Oct 2022 21:39:46 GMT  
		Size: 55.1 MB (55084174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3754e2587bed8ece9b5713bcb14924d27691927399a3750fb6d8ebceb000d771`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f154543e74f792239c3ac5377c8deb20f3956a8e60db04486c4313c0979d7`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.31` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:4a90a0b47798672d3e19064171610cd055cb1d5b702dcf67d6c675c9cb61a96d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155564637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262f364f4f01337f2027e10c7ca2994dc28883afb24386100c89351126d76fe4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 20:40:56 GMT
ADD file:049ff2e28998fde860d1a12f43ec245d10345a71953f67108180c23c237ce26e in / 
# Wed, 12 Oct 2022 20:40:56 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:24:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:24:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:24:47 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:25:15 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:25:17 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:25:18 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:25:19 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:25:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:25:52 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:25:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:25:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:26:33 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:26:34 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:26:36 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:26:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:26:38 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:26:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:828689dcde4b0fe396ab27cf3a6d5f71ee01d48891421ec4381d74ed415be5d0`  
		Last Modified: Wed, 12 Oct 2022 20:42:33 GMT  
		Size: 39.4 MB (39409290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f061378e43d33dc614866c620ab52f8985729cda946779352b12f6a73d099d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1a79ec4c767ad1034121ce2905bb5a3326d01d2c3e24a384b55d34a923bcba`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 857.1 KB (857150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29639854082a90b6e050d61546185cee56cbc0a0224e0a37222ab57bd00917d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:18 GMT  
		Size: 4.4 MB (4433340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be1d8abaf67b766b14bd7b5ee219ce3181b651617cede1fbef78809e83ae2f3`  
		Last Modified: Wed, 12 Oct 2022 21:27:17 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862924992b62147c16c1cad215c391bd43f107b291971074dda31445e6171439`  
		Last Modified: Wed, 12 Oct 2022 21:27:15 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8afc4c260a8060504c3a8696a68694051c62b5dad9774d6b95cc57e9cc10c7`  
		Last Modified: Wed, 12 Oct 2022 21:27:21 GMT  
		Size: 55.4 MB (55421557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb5afa1cf8a3c9f31ed89a4b56cdf88a1d9638c5cadbfc1d8e971265c90892b`  
		Last Modified: Wed, 12 Oct 2022 21:27:13 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693834f1d9bae56fd201dd9a4d7b2eadf83d04d230f650f0c1948876324517e8`  
		Last Modified: Wed, 12 Oct 2022 21:27:23 GMT  
		Size: 55.4 MB (55433646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3411c71dcce2f58523c25058a0800a7e635b92e410e805a30120b936e51a2cb8`  
		Last Modified: Wed, 12 Oct 2022 21:27:16 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877257953583c21228d6fcef6578b5bdfe8729c7f6ee6b366bade14693a92fa5`  
		Last Modified: Wed, 12 Oct 2022 21:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31-debian`

```console
$ docker pull mysql@sha256:159ec35fdd08e138171efa47528aa6a5b683fd769e21378f54f0596a3fea3a4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.31-debian` - linux; amd64

```console
$ docker pull mysql@sha256:151ed8848186e29228574349982a0fdabda35a49452f0da8d1d64488f7e1ccc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177571480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b60588a78bb65c66fde258cd85570c6e8d4bbc637e798a0cc011a463effcf92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:21:45 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Oct 2022 04:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:21:51 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Oct 2022 04:22:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 04:22:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 04:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:22:07 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 05 Oct 2022 04:22:07 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 11 Oct 2022 20:29:30 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Tue, 11 Oct 2022 20:29:31 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 11 Oct 2022 20:29:47 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 11 Oct 2022 20:29:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:29:48 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 11 Oct 2022 20:29:48 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 20:29:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 20:29:49 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 20:29:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f498ba1a3ae2dfa82359e0fb959af536134a1360d33dfa87638e409b70b3fa3`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c224eff0af51a4254bf410ca8f6cab7044171639fc6e7b29cd55248bb609d02`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 4.4 MB (4414808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acdd40c1260704addfdb3a21bf71ae5c14567100f98acd4d8dfec303294e1c5f`  
		Last Modified: Wed, 05 Oct 2022 04:23:50 GMT  
		Size: 1.4 MB (1418452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c3ece0305cbf295220adfdacf8c9e9fdf5de35ea07e505913ea4ee6e1f4f74`  
		Last Modified: Wed, 05 Oct 2022 04:23:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a10286651685e256e36f218063406728987d0f36c285adf41d41f8665661b74`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 12.7 MB (12661783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a34b42ee331888b70b38f6c96cacce54fe2bb4cf6e2ccefdd7add2144d5a3e`  
		Last Modified: Wed, 05 Oct 2022 04:23:49 GMT  
		Size: 2.5 KB (2546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5d04bddbd0c7caeacce07fffaa07f1b523fe80e9415cc5c88fe8387468c2ec`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b2bd56df6d823af6ff936600b456e3a7e94bbab1df9a52b59df7ed84c832d`  
		Last Modified: Tue, 11 Oct 2022 20:32:43 GMT  
		Size: 127.6 MB (127645294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ca09d481ffc70add23e3d81c2a8d0bf7c30928edf8650a3cd3464c14022eb6`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5840a45093cbfdd7cab682cbf5b5f879086883904300f5dfe84441a0129bfe6`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6e4d6f9231e9ee88d7085aa68eac1de6d4789d9508824387327e8db28ce074`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31-oracle`

```console
$ docker pull mysql@sha256:147572c972192417add6f1cf65ea33edfd44086e461a3381601b53e1662f5d15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.31-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:fb3d8639a938515aaac38acb13c4acc061366a20322c55bbedae9d127cd2f2b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157265417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b83de8fb1a29d9b47d3ecbff86f67d22f8418f6e6ef5d349aaca2c2919074a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 21:20:42 GMT
ADD file:ceac4c0bc6dd71b3868d5af15bdaab832a2f61b45c12116b2df42ef8cfbf9fa1 in / 
# Wed, 12 Oct 2022 21:20:42 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:37:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:37:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:37:33 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:37:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:37:57 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:37:58 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:38:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:38:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:38:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:39:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:39:04 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:39:04 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:39:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:39:05 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:39:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ed150ed0abef03007b46722de75bcb3e517f22532a46146fcec4fb1761d4347`  
		Last Modified: Wed, 12 Oct 2022 21:22:08 GMT  
		Size: 40.6 MB (40589408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fede58e17ac8f886aa620315c1c85d2979e38aa05aebf00aacba6d240a18620`  
		Last Modified: Wed, 12 Oct 2022 21:39:40 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994a6ddd6efe5eef3b2be88576cfa2e823d47f0c7db10554360438631d0f786b`  
		Last Modified: Wed, 12 Oct 2022 21:39:41 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028bda79779b4b2f4b249922d92841289aeae64aea45154be16cd17cfe986fdd`  
		Last Modified: Wed, 12 Oct 2022 21:39:39 GMT  
		Size: 4.6 MB (4606927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426fbe9e56a28ac107f62e7fb3b835c320ff0997c762490c853ae8242765da9f`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a00e58dd193f3585ff724fd8ba4f7c78d83cf33b851a186b925b36317542f34`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4f64494005d7365861de3808b1c39783259162154a12b6b6694e5303732c2b`  
		Last Modified: Wed, 12 Oct 2022 21:39:45 GMT  
		Size: 56.0 MB (56046404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba8ab3534a7c32755a032486836b05d3d5a724ba6e7127ce259a0ea02fae975`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695938edf88c0409d640f6edcb00898d28478ed80505fd449f6c05c2b99ec3d`  
		Last Modified: Wed, 12 Oct 2022 21:39:46 GMT  
		Size: 55.1 MB (55084174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3754e2587bed8ece9b5713bcb14924d27691927399a3750fb6d8ebceb000d771`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f154543e74f792239c3ac5377c8deb20f3956a8e60db04486c4313c0979d7`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.31-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:4a90a0b47798672d3e19064171610cd055cb1d5b702dcf67d6c675c9cb61a96d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155564637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262f364f4f01337f2027e10c7ca2994dc28883afb24386100c89351126d76fe4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 20:40:56 GMT
ADD file:049ff2e28998fde860d1a12f43ec245d10345a71953f67108180c23c237ce26e in / 
# Wed, 12 Oct 2022 20:40:56 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:24:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:24:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:24:47 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:25:15 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:25:17 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:25:18 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:25:19 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:25:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:25:52 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:25:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:25:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:26:33 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:26:34 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:26:36 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:26:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:26:38 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:26:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:828689dcde4b0fe396ab27cf3a6d5f71ee01d48891421ec4381d74ed415be5d0`  
		Last Modified: Wed, 12 Oct 2022 20:42:33 GMT  
		Size: 39.4 MB (39409290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f061378e43d33dc614866c620ab52f8985729cda946779352b12f6a73d099d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1a79ec4c767ad1034121ce2905bb5a3326d01d2c3e24a384b55d34a923bcba`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 857.1 KB (857150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29639854082a90b6e050d61546185cee56cbc0a0224e0a37222ab57bd00917d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:18 GMT  
		Size: 4.4 MB (4433340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be1d8abaf67b766b14bd7b5ee219ce3181b651617cede1fbef78809e83ae2f3`  
		Last Modified: Wed, 12 Oct 2022 21:27:17 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862924992b62147c16c1cad215c391bd43f107b291971074dda31445e6171439`  
		Last Modified: Wed, 12 Oct 2022 21:27:15 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8afc4c260a8060504c3a8696a68694051c62b5dad9774d6b95cc57e9cc10c7`  
		Last Modified: Wed, 12 Oct 2022 21:27:21 GMT  
		Size: 55.4 MB (55421557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb5afa1cf8a3c9f31ed89a4b56cdf88a1d9638c5cadbfc1d8e971265c90892b`  
		Last Modified: Wed, 12 Oct 2022 21:27:13 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693834f1d9bae56fd201dd9a4d7b2eadf83d04d230f650f0c1948876324517e8`  
		Last Modified: Wed, 12 Oct 2022 21:27:23 GMT  
		Size: 55.4 MB (55433646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3411c71dcce2f58523c25058a0800a7e635b92e410e805a30120b936e51a2cb8`  
		Last Modified: Wed, 12 Oct 2022 21:27:16 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877257953583c21228d6fcef6578b5bdfe8729c7f6ee6b366bade14693a92fa5`  
		Last Modified: Wed, 12 Oct 2022 21:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:159ec35fdd08e138171efa47528aa6a5b683fd769e21378f54f0596a3fea3a4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:151ed8848186e29228574349982a0fdabda35a49452f0da8d1d64488f7e1ccc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177571480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b60588a78bb65c66fde258cd85570c6e8d4bbc637e798a0cc011a463effcf92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:21:45 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Oct 2022 04:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:21:51 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Oct 2022 04:22:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 04:22:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 04:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:22:07 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 05 Oct 2022 04:22:07 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 11 Oct 2022 20:29:30 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Tue, 11 Oct 2022 20:29:31 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 11 Oct 2022 20:29:47 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 11 Oct 2022 20:29:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:29:48 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 11 Oct 2022 20:29:48 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 20:29:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 20:29:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 20:29:49 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 20:29:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f498ba1a3ae2dfa82359e0fb959af536134a1360d33dfa87638e409b70b3fa3`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c224eff0af51a4254bf410ca8f6cab7044171639fc6e7b29cd55248bb609d02`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 4.4 MB (4414808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acdd40c1260704addfdb3a21bf71ae5c14567100f98acd4d8dfec303294e1c5f`  
		Last Modified: Wed, 05 Oct 2022 04:23:50 GMT  
		Size: 1.4 MB (1418452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c3ece0305cbf295220adfdacf8c9e9fdf5de35ea07e505913ea4ee6e1f4f74`  
		Last Modified: Wed, 05 Oct 2022 04:23:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a10286651685e256e36f218063406728987d0f36c285adf41d41f8665661b74`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 12.7 MB (12661783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a34b42ee331888b70b38f6c96cacce54fe2bb4cf6e2ccefdd7add2144d5a3e`  
		Last Modified: Wed, 05 Oct 2022 04:23:49 GMT  
		Size: 2.5 KB (2546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5d04bddbd0c7caeacce07fffaa07f1b523fe80e9415cc5c88fe8387468c2ec`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b2bd56df6d823af6ff936600b456e3a7e94bbab1df9a52b59df7ed84c832d`  
		Last Modified: Tue, 11 Oct 2022 20:32:43 GMT  
		Size: 127.6 MB (127645294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ca09d481ffc70add23e3d81c2a8d0bf7c30928edf8650a3cd3464c14022eb6`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5840a45093cbfdd7cab682cbf5b5f879086883904300f5dfe84441a0129bfe6`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6e4d6f9231e9ee88d7085aa68eac1de6d4789d9508824387327e8db28ce074`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:147572c972192417add6f1cf65ea33edfd44086e461a3381601b53e1662f5d15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:fb3d8639a938515aaac38acb13c4acc061366a20322c55bbedae9d127cd2f2b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157265417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b83de8fb1a29d9b47d3ecbff86f67d22f8418f6e6ef5d349aaca2c2919074a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 21:20:42 GMT
ADD file:ceac4c0bc6dd71b3868d5af15bdaab832a2f61b45c12116b2df42ef8cfbf9fa1 in / 
# Wed, 12 Oct 2022 21:20:42 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:37:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:37:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:37:33 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:37:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:37:57 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:37:58 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:38:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:38:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:38:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:39:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:39:04 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:39:04 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:39:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:39:05 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:39:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ed150ed0abef03007b46722de75bcb3e517f22532a46146fcec4fb1761d4347`  
		Last Modified: Wed, 12 Oct 2022 21:22:08 GMT  
		Size: 40.6 MB (40589408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fede58e17ac8f886aa620315c1c85d2979e38aa05aebf00aacba6d240a18620`  
		Last Modified: Wed, 12 Oct 2022 21:39:40 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994a6ddd6efe5eef3b2be88576cfa2e823d47f0c7db10554360438631d0f786b`  
		Last Modified: Wed, 12 Oct 2022 21:39:41 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028bda79779b4b2f4b249922d92841289aeae64aea45154be16cd17cfe986fdd`  
		Last Modified: Wed, 12 Oct 2022 21:39:39 GMT  
		Size: 4.6 MB (4606927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426fbe9e56a28ac107f62e7fb3b835c320ff0997c762490c853ae8242765da9f`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a00e58dd193f3585ff724fd8ba4f7c78d83cf33b851a186b925b36317542f34`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4f64494005d7365861de3808b1c39783259162154a12b6b6694e5303732c2b`  
		Last Modified: Wed, 12 Oct 2022 21:39:45 GMT  
		Size: 56.0 MB (56046404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba8ab3534a7c32755a032486836b05d3d5a724ba6e7127ce259a0ea02fae975`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695938edf88c0409d640f6edcb00898d28478ed80505fd449f6c05c2b99ec3d`  
		Last Modified: Wed, 12 Oct 2022 21:39:46 GMT  
		Size: 55.1 MB (55084174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3754e2587bed8ece9b5713bcb14924d27691927399a3750fb6d8ebceb000d771`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f154543e74f792239c3ac5377c8deb20f3956a8e60db04486c4313c0979d7`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:4a90a0b47798672d3e19064171610cd055cb1d5b702dcf67d6c675c9cb61a96d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155564637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262f364f4f01337f2027e10c7ca2994dc28883afb24386100c89351126d76fe4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 20:40:56 GMT
ADD file:049ff2e28998fde860d1a12f43ec245d10345a71953f67108180c23c237ce26e in / 
# Wed, 12 Oct 2022 20:40:56 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:24:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:24:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:24:47 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:25:15 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:25:17 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:25:18 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:25:19 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:25:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:25:52 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:25:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:25:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:26:33 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:26:34 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:26:36 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:26:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:26:38 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:26:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:828689dcde4b0fe396ab27cf3a6d5f71ee01d48891421ec4381d74ed415be5d0`  
		Last Modified: Wed, 12 Oct 2022 20:42:33 GMT  
		Size: 39.4 MB (39409290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f061378e43d33dc614866c620ab52f8985729cda946779352b12f6a73d099d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1a79ec4c767ad1034121ce2905bb5a3326d01d2c3e24a384b55d34a923bcba`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 857.1 KB (857150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29639854082a90b6e050d61546185cee56cbc0a0224e0a37222ab57bd00917d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:18 GMT  
		Size: 4.4 MB (4433340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be1d8abaf67b766b14bd7b5ee219ce3181b651617cede1fbef78809e83ae2f3`  
		Last Modified: Wed, 12 Oct 2022 21:27:17 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862924992b62147c16c1cad215c391bd43f107b291971074dda31445e6171439`  
		Last Modified: Wed, 12 Oct 2022 21:27:15 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8afc4c260a8060504c3a8696a68694051c62b5dad9774d6b95cc57e9cc10c7`  
		Last Modified: Wed, 12 Oct 2022 21:27:21 GMT  
		Size: 55.4 MB (55421557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb5afa1cf8a3c9f31ed89a4b56cdf88a1d9638c5cadbfc1d8e971265c90892b`  
		Last Modified: Wed, 12 Oct 2022 21:27:13 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693834f1d9bae56fd201dd9a4d7b2eadf83d04d230f650f0c1948876324517e8`  
		Last Modified: Wed, 12 Oct 2022 21:27:23 GMT  
		Size: 55.4 MB (55433646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3411c71dcce2f58523c25058a0800a7e635b92e410e805a30120b936e51a2cb8`  
		Last Modified: Wed, 12 Oct 2022 21:27:16 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877257953583c21228d6fcef6578b5bdfe8729c7f6ee6b366bade14693a92fa5`  
		Last Modified: Wed, 12 Oct 2022 21:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:147572c972192417add6f1cf65ea33edfd44086e461a3381601b53e1662f5d15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:fb3d8639a938515aaac38acb13c4acc061366a20322c55bbedae9d127cd2f2b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157265417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b83de8fb1a29d9b47d3ecbff86f67d22f8418f6e6ef5d349aaca2c2919074a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 21:20:42 GMT
ADD file:ceac4c0bc6dd71b3868d5af15bdaab832a2f61b45c12116b2df42ef8cfbf9fa1 in / 
# Wed, 12 Oct 2022 21:20:42 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:37:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:37:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:37:33 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:37:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:37:57 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:37:58 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:38:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:38:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:38:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:39:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:39:04 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:39:04 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:39:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:39:05 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:39:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ed150ed0abef03007b46722de75bcb3e517f22532a46146fcec4fb1761d4347`  
		Last Modified: Wed, 12 Oct 2022 21:22:08 GMT  
		Size: 40.6 MB (40589408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fede58e17ac8f886aa620315c1c85d2979e38aa05aebf00aacba6d240a18620`  
		Last Modified: Wed, 12 Oct 2022 21:39:40 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994a6ddd6efe5eef3b2be88576cfa2e823d47f0c7db10554360438631d0f786b`  
		Last Modified: Wed, 12 Oct 2022 21:39:41 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028bda79779b4b2f4b249922d92841289aeae64aea45154be16cd17cfe986fdd`  
		Last Modified: Wed, 12 Oct 2022 21:39:39 GMT  
		Size: 4.6 MB (4606927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426fbe9e56a28ac107f62e7fb3b835c320ff0997c762490c853ae8242765da9f`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a00e58dd193f3585ff724fd8ba4f7c78d83cf33b851a186b925b36317542f34`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4f64494005d7365861de3808b1c39783259162154a12b6b6694e5303732c2b`  
		Last Modified: Wed, 12 Oct 2022 21:39:45 GMT  
		Size: 56.0 MB (56046404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba8ab3534a7c32755a032486836b05d3d5a724ba6e7127ce259a0ea02fae975`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695938edf88c0409d640f6edcb00898d28478ed80505fd449f6c05c2b99ec3d`  
		Last Modified: Wed, 12 Oct 2022 21:39:46 GMT  
		Size: 55.1 MB (55084174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3754e2587bed8ece9b5713bcb14924d27691927399a3750fb6d8ebceb000d771`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f154543e74f792239c3ac5377c8deb20f3956a8e60db04486c4313c0979d7`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:4a90a0b47798672d3e19064171610cd055cb1d5b702dcf67d6c675c9cb61a96d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155564637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262f364f4f01337f2027e10c7ca2994dc28883afb24386100c89351126d76fe4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 20:40:56 GMT
ADD file:049ff2e28998fde860d1a12f43ec245d10345a71953f67108180c23c237ce26e in / 
# Wed, 12 Oct 2022 20:40:56 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:24:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:24:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:24:47 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:25:15 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:25:17 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:25:18 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:25:19 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:25:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:25:52 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:25:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:25:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:26:33 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:26:34 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:26:36 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:26:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:26:38 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:26:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:828689dcde4b0fe396ab27cf3a6d5f71ee01d48891421ec4381d74ed415be5d0`  
		Last Modified: Wed, 12 Oct 2022 20:42:33 GMT  
		Size: 39.4 MB (39409290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f061378e43d33dc614866c620ab52f8985729cda946779352b12f6a73d099d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1a79ec4c767ad1034121ce2905bb5a3326d01d2c3e24a384b55d34a923bcba`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 857.1 KB (857150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29639854082a90b6e050d61546185cee56cbc0a0224e0a37222ab57bd00917d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:18 GMT  
		Size: 4.4 MB (4433340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be1d8abaf67b766b14bd7b5ee219ce3181b651617cede1fbef78809e83ae2f3`  
		Last Modified: Wed, 12 Oct 2022 21:27:17 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862924992b62147c16c1cad215c391bd43f107b291971074dda31445e6171439`  
		Last Modified: Wed, 12 Oct 2022 21:27:15 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8afc4c260a8060504c3a8696a68694051c62b5dad9774d6b95cc57e9cc10c7`  
		Last Modified: Wed, 12 Oct 2022 21:27:21 GMT  
		Size: 55.4 MB (55421557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb5afa1cf8a3c9f31ed89a4b56cdf88a1d9638c5cadbfc1d8e971265c90892b`  
		Last Modified: Wed, 12 Oct 2022 21:27:13 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693834f1d9bae56fd201dd9a4d7b2eadf83d04d230f650f0c1948876324517e8`  
		Last Modified: Wed, 12 Oct 2022 21:27:23 GMT  
		Size: 55.4 MB (55433646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3411c71dcce2f58523c25058a0800a7e635b92e410e805a30120b936e51a2cb8`  
		Last Modified: Wed, 12 Oct 2022 21:27:16 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877257953583c21228d6fcef6578b5bdfe8729c7f6ee6b366bade14693a92fa5`  
		Last Modified: Wed, 12 Oct 2022 21:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
