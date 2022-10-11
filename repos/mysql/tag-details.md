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
$ docker pull mysql@sha256:a85b8313feb7298ae240c4beb33a1b4d2e3a3867d3195bab9ed9346d332217c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:b39b95329c868c3875ea6eb23c9a2a27168c3531f83c96c24324213f75793636
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129460661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb175b0743cc4475f4440b3d9dacbe7e3f29dc455a60999ce260366709bb1d00`
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
# Fri, 07 Oct 2022 21:07:36 GMT
ENV MYSQL_VERSION=5.7.39-1.el7
# Fri, 07 Oct 2022 21:07:36 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:07:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:07:55 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:07:55 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el7
# Fri, 07 Oct 2022 21:08:16 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:08:17 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:08:17 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:08:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:08:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:08:18 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:08:18 GMT
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
	-	`sha256:266b96d99da24606359f05ed90b8d9bc96019eecf841fef22bfaf7c2f6451e84`  
		Last Modified: Fri, 07 Oct 2022 21:09:25 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1965015916405436be1a814fdec2dbfd63857a2c7a0ab466c69df9b1af0238`  
		Last Modified: Fri, 07 Oct 2022 21:09:27 GMT  
		Size: 25.5 MB (25506028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5976bb40e48b9bcaf847b190e836781ec8391a56ba1411e877fc68352a218a`  
		Last Modified: Fri, 07 Oct 2022 21:09:23 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dde9165879ec22185c6d0e588b3c0b09e4515df9c1f44ccf727096c324cff6`  
		Last Modified: Fri, 07 Oct 2022 21:09:32 GMT  
		Size: 48.6 MB (48598915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604d9c61b75931c108ef1d876ab74535f26212280a2ff7d0502d55f4028407bf`  
		Last Modified: Fri, 07 Oct 2022 21:09:23 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd75db384927c06c5bea0df9ad95522c8ab23a4fa4e07125693e38132b89675`  
		Last Modified: Fri, 07 Oct 2022 21:09:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:f1c5bbefe1aaff6c816fb7193391668521cd0eb3587560fd15faeb9b226b77a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:e60db24aaf5c748b3e5f3320c843282e6ebd87039faa188e4bf986dd574e54d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162534124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6abe8c2c2f9465506e659685eb6012bed544ebb0a3ce91b9bd1c6c8ee63e2d30`
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
# Wed, 05 Oct 2022 04:22:59 GMT
ENV MYSQL_VERSION=5.7.39-1debian10
# Wed, 05 Oct 2022 04:23:00 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 05 Oct 2022 04:23:20 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 05 Oct 2022 04:23:20 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Oct 2022 04:23:21 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:23:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:23:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:23:21 GMT
EXPOSE 3306 33060
# Wed, 05 Oct 2022 04:23:22 GMT
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
	-	`sha256:c0225260858f5bec45902e81dc388af9707d656b2ac6d16a89c0195636bbd76c`  
		Last Modified: Wed, 05 Oct 2022 04:24:23 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5200d9e491caac48656cd7f43bfb68ddeb2a210567b8ef6f7c4399df3b3332`  
		Last Modified: Wed, 05 Oct 2022 04:24:38 GMT  
		Size: 115.7 MB (115733089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d6ad7fb947346c41003be489f740c140d6deb361bcba625733a8971f79fe2a`  
		Last Modified: Wed, 05 Oct 2022 04:24:23 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013f5c86a18f9fa9483bb890aa37484141e557cab4c119fff68c34da2e22e5d8`  
		Last Modified: Wed, 05 Oct 2022 04:24:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:a85b8313feb7298ae240c4beb33a1b4d2e3a3867d3195bab9ed9346d332217c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:b39b95329c868c3875ea6eb23c9a2a27168c3531f83c96c24324213f75793636
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129460661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb175b0743cc4475f4440b3d9dacbe7e3f29dc455a60999ce260366709bb1d00`
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
# Fri, 07 Oct 2022 21:07:36 GMT
ENV MYSQL_VERSION=5.7.39-1.el7
# Fri, 07 Oct 2022 21:07:36 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:07:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:07:55 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:07:55 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el7
# Fri, 07 Oct 2022 21:08:16 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:08:17 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:08:17 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:08:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:08:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:08:18 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:08:18 GMT
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
	-	`sha256:266b96d99da24606359f05ed90b8d9bc96019eecf841fef22bfaf7c2f6451e84`  
		Last Modified: Fri, 07 Oct 2022 21:09:25 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1965015916405436be1a814fdec2dbfd63857a2c7a0ab466c69df9b1af0238`  
		Last Modified: Fri, 07 Oct 2022 21:09:27 GMT  
		Size: 25.5 MB (25506028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5976bb40e48b9bcaf847b190e836781ec8391a56ba1411e877fc68352a218a`  
		Last Modified: Fri, 07 Oct 2022 21:09:23 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dde9165879ec22185c6d0e588b3c0b09e4515df9c1f44ccf727096c324cff6`  
		Last Modified: Fri, 07 Oct 2022 21:09:32 GMT  
		Size: 48.6 MB (48598915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604d9c61b75931c108ef1d876ab74535f26212280a2ff7d0502d55f4028407bf`  
		Last Modified: Fri, 07 Oct 2022 21:09:23 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd75db384927c06c5bea0df9ad95522c8ab23a4fa4e07125693e38132b89675`  
		Last Modified: Fri, 07 Oct 2022 21:09:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:a85b8313feb7298ae240c4beb33a1b4d2e3a3867d3195bab9ed9346d332217c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:b39b95329c868c3875ea6eb23c9a2a27168c3531f83c96c24324213f75793636
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129460661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb175b0743cc4475f4440b3d9dacbe7e3f29dc455a60999ce260366709bb1d00`
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
# Fri, 07 Oct 2022 21:07:36 GMT
ENV MYSQL_VERSION=5.7.39-1.el7
# Fri, 07 Oct 2022 21:07:36 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:07:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:07:55 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:07:55 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el7
# Fri, 07 Oct 2022 21:08:16 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:08:17 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:08:17 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:08:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:08:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:08:18 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:08:18 GMT
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
	-	`sha256:266b96d99da24606359f05ed90b8d9bc96019eecf841fef22bfaf7c2f6451e84`  
		Last Modified: Fri, 07 Oct 2022 21:09:25 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1965015916405436be1a814fdec2dbfd63857a2c7a0ab466c69df9b1af0238`  
		Last Modified: Fri, 07 Oct 2022 21:09:27 GMT  
		Size: 25.5 MB (25506028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5976bb40e48b9bcaf847b190e836781ec8391a56ba1411e877fc68352a218a`  
		Last Modified: Fri, 07 Oct 2022 21:09:23 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dde9165879ec22185c6d0e588b3c0b09e4515df9c1f44ccf727096c324cff6`  
		Last Modified: Fri, 07 Oct 2022 21:09:32 GMT  
		Size: 48.6 MB (48598915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604d9c61b75931c108ef1d876ab74535f26212280a2ff7d0502d55f4028407bf`  
		Last Modified: Fri, 07 Oct 2022 21:09:23 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd75db384927c06c5bea0df9ad95522c8ab23a4fa4e07125693e38132b89675`  
		Last Modified: Fri, 07 Oct 2022 21:09:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:f1c5bbefe1aaff6c816fb7193391668521cd0eb3587560fd15faeb9b226b77a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:e60db24aaf5c748b3e5f3320c843282e6ebd87039faa188e4bf986dd574e54d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162534124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6abe8c2c2f9465506e659685eb6012bed544ebb0a3ce91b9bd1c6c8ee63e2d30`
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
# Wed, 05 Oct 2022 04:22:59 GMT
ENV MYSQL_VERSION=5.7.39-1debian10
# Wed, 05 Oct 2022 04:23:00 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 05 Oct 2022 04:23:20 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 05 Oct 2022 04:23:20 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Oct 2022 04:23:21 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:23:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:23:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:23:21 GMT
EXPOSE 3306 33060
# Wed, 05 Oct 2022 04:23:22 GMT
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
	-	`sha256:c0225260858f5bec45902e81dc388af9707d656b2ac6d16a89c0195636bbd76c`  
		Last Modified: Wed, 05 Oct 2022 04:24:23 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5200d9e491caac48656cd7f43bfb68ddeb2a210567b8ef6f7c4399df3b3332`  
		Last Modified: Wed, 05 Oct 2022 04:24:38 GMT  
		Size: 115.7 MB (115733089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d6ad7fb947346c41003be489f740c140d6deb361bcba625733a8971f79fe2a`  
		Last Modified: Wed, 05 Oct 2022 04:24:23 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013f5c86a18f9fa9483bb890aa37484141e557cab4c119fff68c34da2e22e5d8`  
		Last Modified: Wed, 05 Oct 2022 04:24:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:a85b8313feb7298ae240c4beb33a1b4d2e3a3867d3195bab9ed9346d332217c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:b39b95329c868c3875ea6eb23c9a2a27168c3531f83c96c24324213f75793636
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129460661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb175b0743cc4475f4440b3d9dacbe7e3f29dc455a60999ce260366709bb1d00`
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
# Fri, 07 Oct 2022 21:07:36 GMT
ENV MYSQL_VERSION=5.7.39-1.el7
# Fri, 07 Oct 2022 21:07:36 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:07:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:07:55 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:07:55 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el7
# Fri, 07 Oct 2022 21:08:16 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:08:17 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:08:17 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:08:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:08:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:08:18 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:08:18 GMT
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
	-	`sha256:266b96d99da24606359f05ed90b8d9bc96019eecf841fef22bfaf7c2f6451e84`  
		Last Modified: Fri, 07 Oct 2022 21:09:25 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1965015916405436be1a814fdec2dbfd63857a2c7a0ab466c69df9b1af0238`  
		Last Modified: Fri, 07 Oct 2022 21:09:27 GMT  
		Size: 25.5 MB (25506028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5976bb40e48b9bcaf847b190e836781ec8391a56ba1411e877fc68352a218a`  
		Last Modified: Fri, 07 Oct 2022 21:09:23 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dde9165879ec22185c6d0e588b3c0b09e4515df9c1f44ccf727096c324cff6`  
		Last Modified: Fri, 07 Oct 2022 21:09:32 GMT  
		Size: 48.6 MB (48598915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604d9c61b75931c108ef1d876ab74535f26212280a2ff7d0502d55f4028407bf`  
		Last Modified: Fri, 07 Oct 2022 21:09:23 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd75db384927c06c5bea0df9ad95522c8ab23a4fa4e07125693e38132b89675`  
		Last Modified: Fri, 07 Oct 2022 21:09:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40`

**does not exist** (yet?)

## `mysql:5.7.40-debian`

**does not exist** (yet?)

## `mysql:5.7.40-oracle`

**does not exist** (yet?)

## `mysql:8`

```console
$ docker pull mysql@sha256:3c1aab708f6e57fc4dccafe36baccc7219acfb4ec450f3fb6d370ea89409e906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:f90d1aeb92a5c7b3a4178a3052d8bc27b1f52a811aacb27b619c10b778b9f281
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133890226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbaea59d1b4194257138a6434ec0820a13097dd7e900135e78daf9759fe2407a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:31:40 GMT
ADD file:40e1b0533d9ae91c868834395cbd4b74cf2a47965791be201c03ae764f9da2b0 in / 
# Fri, 07 Oct 2022 20:31:41 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:05:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:05:33 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:05:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:05:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:06:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:06:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:06:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:07:04 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:07:04 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:07:05 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:07:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:07:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:07:05 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:07:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:295ca23427284cb123fd4c132a1ecb521e7f787ac75dadec342f744a343efec4`  
		Last Modified: Fri, 07 Oct 2022 20:33:22 GMT  
		Size: 40.6 MB (40589568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79af4312a7e0fb060724a99077fbd6a3460284520318bbfe874d11e472aed010`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d3d73d17046a044f9f4a45aa0f74afa79387dc1eb634ef96eb39a947b3077d`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b8724b397717c0920f045a0dc9b778426bb5ed5ff17f2ecaece3b27914fe3`  
		Last Modified: Fri, 07 Oct 2022 21:08:49 GMT  
		Size: 4.6 MB (4606973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cf360b4a14d6543edc2e7f35ce87406aa7b82c29e252f8ef911f39dcbc6de2`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0115482cc006f85365a790dc394ead0f59f922046bb77b3509e6f7989b32b2a5`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a360b08917ea13f41e1d042db0163b46c0069b93a5e2995543ab10fa70541e16`  
		Last Modified: Fri, 07 Oct 2022 21:08:54 GMT  
		Size: 47.7 MB (47733932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12deeb3c132385712ac84f6ab3842432f96d231682957f254fdb8400156b3736`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1dc10db1e9a87dda49ac546d7263db2fd5e6163aa17228c7d60f464bf91098`  
		Last Modified: Fri, 07 Oct 2022 21:08:53 GMT  
		Size: 40.0 MB (40021240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64be404ad29c0faf50a4c5855fcbbb8491b2f8fd89ac4df11b3a0b26f990a4da`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921fe8879a2ef55d203b4ad84ee572904a1afb7b195013a82bc3568b85624e2`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c6f2eef8a149e0efd0515ab57a41f84cf06859eab6babb0b349d8d75e1c68544
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142631938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1699df6c42a3ed6b4a8f6e65ec1886dfab6ab4f213eadc8e44b6f79630d5ac01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:51:45 GMT
ADD file:6eb7b065ffe8855d82638de19bd23fba329883c96f01d093e7bc6bdb5da836a3 in / 
# Fri, 07 Oct 2022 20:51:46 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:09:40 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:09:41 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:09:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:10:14 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:10:16 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:10:17 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 07 Oct 2022 21:10:18 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:10:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:10:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:10:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:10:55 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:11:30 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:11:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:11:32 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:11:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:11:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:11:34 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:11:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d45c82139e084eb338a0a2346c4ec4c6d2bfa4acda9194cf6602728b4a3e89f`  
		Last Modified: Fri, 07 Oct 2022 20:53:34 GMT  
		Size: 39.4 MB (39409020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c544deffc3a52cba4e3a2ec48f677586760eb4717c161c4adebcb8ce20402a8`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af07bf98dff8f0d9fa86a18b24151f9803947d9d622097b25bf3f5874b2bd6c9`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0554dfac498a04af357c6a46c1e81c7a38af77e0f18e416c035c3e64f7d9905e`  
		Last Modified: Fri, 07 Oct 2022 21:12:12 GMT  
		Size: 4.4 MB (4433409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f612237e783e94a541b8163f9f2a3d5d66b3b804fdddcd51e7b752f50f7ffaec`  
		Last Modified: Fri, 07 Oct 2022 21:12:11 GMT  
		Size: 2.6 KB (2610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db27487a0c82f6090e67e6b7ea5caddb59f62cf16ac8c91558438a1b0408525`  
		Last Modified: Fri, 07 Oct 2022 21:12:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87b5be864804505c24ba253a53076347702ebd268e3106024a742665fa83dda`  
		Last Modified: Fri, 07 Oct 2022 21:12:17 GMT  
		Size: 53.8 MB (53817534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afd03a0f65e88ab8ba56cc8cd838d009c7fdea1c1491dccdcf631766227e5d4`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ceb4bec32c454301ab7ef00f268ba79aaa6b1ea01012c3167779ff0c90574c`  
		Last Modified: Fri, 07 Oct 2022 21:12:17 GMT  
		Size: 44.1 MB (44105166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2151a4f39c78b2ecbc36299c2154651d21fa2c2555e1d40582e76b4852ec6a8c`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e70080d6082a60048ca786d5834ca53ccf4cc2b3860b6089fa0f1b8e0cbe15`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:c00749f00b317206048b8eaf304ded3941ecaf452b73a8e178b8ea2d1fc29342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:12477b35d174c1a410da24a05c4884693836e2a863521aa339a1298ce48b8369
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157889330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34e66721c05dacebba2911adc611de5a71b95458b5a7208fb961aa3051b5eec2`
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
# Wed, 05 Oct 2022 04:22:08 GMT
ENV MYSQL_VERSION=8.0.30-1debian11
# Wed, 05 Oct 2022 04:22:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 05 Oct 2022 04:22:23 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 05 Oct 2022 04:22:24 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Oct 2022 04:22:24 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 05 Oct 2022 04:22:24 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:22:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:22:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:22:25 GMT
EXPOSE 3306 33060
# Wed, 05 Oct 2022 04:22:25 GMT
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
	-	`sha256:f1363e6677cacb6f7960a756d9b4c0aa8d4c8ec02869cb4a6d9159faa60ecba4`  
		Last Modified: Wed, 05 Oct 2022 04:23:47 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1110efce5dd0e631830f85c1a0c25efbba11b2e55314c04bb4fc0f97a30fdfc`  
		Last Modified: Wed, 05 Oct 2022 04:24:04 GMT  
		Size: 108.0 MB (107963159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fda2bd249a81a6cde8a8959a44831ac82aa8e5ecf3e1d508cf07ae87454330`  
		Last Modified: Wed, 05 Oct 2022 04:23:47 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89080d4312c49459448781df923db9f843c0f978fc5100842de22d34ce9b142`  
		Last Modified: Wed, 05 Oct 2022 04:23:47 GMT  
		Size: 5.4 KB (5382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d74113edbbb66aa319322589f5e5f54f3ac373cc17fb9a2fdd5c3fe2f877345`  
		Last Modified: Wed, 05 Oct 2022 04:23:47 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:3c1aab708f6e57fc4dccafe36baccc7219acfb4ec450f3fb6d370ea89409e906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:f90d1aeb92a5c7b3a4178a3052d8bc27b1f52a811aacb27b619c10b778b9f281
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133890226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbaea59d1b4194257138a6434ec0820a13097dd7e900135e78daf9759fe2407a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:31:40 GMT
ADD file:40e1b0533d9ae91c868834395cbd4b74cf2a47965791be201c03ae764f9da2b0 in / 
# Fri, 07 Oct 2022 20:31:41 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:05:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:05:33 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:05:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:05:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:06:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:06:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:06:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:07:04 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:07:04 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:07:05 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:07:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:07:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:07:05 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:07:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:295ca23427284cb123fd4c132a1ecb521e7f787ac75dadec342f744a343efec4`  
		Last Modified: Fri, 07 Oct 2022 20:33:22 GMT  
		Size: 40.6 MB (40589568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79af4312a7e0fb060724a99077fbd6a3460284520318bbfe874d11e472aed010`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d3d73d17046a044f9f4a45aa0f74afa79387dc1eb634ef96eb39a947b3077d`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b8724b397717c0920f045a0dc9b778426bb5ed5ff17f2ecaece3b27914fe3`  
		Last Modified: Fri, 07 Oct 2022 21:08:49 GMT  
		Size: 4.6 MB (4606973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cf360b4a14d6543edc2e7f35ce87406aa7b82c29e252f8ef911f39dcbc6de2`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0115482cc006f85365a790dc394ead0f59f922046bb77b3509e6f7989b32b2a5`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a360b08917ea13f41e1d042db0163b46c0069b93a5e2995543ab10fa70541e16`  
		Last Modified: Fri, 07 Oct 2022 21:08:54 GMT  
		Size: 47.7 MB (47733932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12deeb3c132385712ac84f6ab3842432f96d231682957f254fdb8400156b3736`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1dc10db1e9a87dda49ac546d7263db2fd5e6163aa17228c7d60f464bf91098`  
		Last Modified: Fri, 07 Oct 2022 21:08:53 GMT  
		Size: 40.0 MB (40021240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64be404ad29c0faf50a4c5855fcbbb8491b2f8fd89ac4df11b3a0b26f990a4da`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921fe8879a2ef55d203b4ad84ee572904a1afb7b195013a82bc3568b85624e2`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c6f2eef8a149e0efd0515ab57a41f84cf06859eab6babb0b349d8d75e1c68544
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142631938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1699df6c42a3ed6b4a8f6e65ec1886dfab6ab4f213eadc8e44b6f79630d5ac01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:51:45 GMT
ADD file:6eb7b065ffe8855d82638de19bd23fba329883c96f01d093e7bc6bdb5da836a3 in / 
# Fri, 07 Oct 2022 20:51:46 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:09:40 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:09:41 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:09:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:10:14 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:10:16 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:10:17 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 07 Oct 2022 21:10:18 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:10:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:10:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:10:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:10:55 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:11:30 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:11:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:11:32 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:11:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:11:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:11:34 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:11:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d45c82139e084eb338a0a2346c4ec4c6d2bfa4acda9194cf6602728b4a3e89f`  
		Last Modified: Fri, 07 Oct 2022 20:53:34 GMT  
		Size: 39.4 MB (39409020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c544deffc3a52cba4e3a2ec48f677586760eb4717c161c4adebcb8ce20402a8`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af07bf98dff8f0d9fa86a18b24151f9803947d9d622097b25bf3f5874b2bd6c9`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0554dfac498a04af357c6a46c1e81c7a38af77e0f18e416c035c3e64f7d9905e`  
		Last Modified: Fri, 07 Oct 2022 21:12:12 GMT  
		Size: 4.4 MB (4433409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f612237e783e94a541b8163f9f2a3d5d66b3b804fdddcd51e7b752f50f7ffaec`  
		Last Modified: Fri, 07 Oct 2022 21:12:11 GMT  
		Size: 2.6 KB (2610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db27487a0c82f6090e67e6b7ea5caddb59f62cf16ac8c91558438a1b0408525`  
		Last Modified: Fri, 07 Oct 2022 21:12:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87b5be864804505c24ba253a53076347702ebd268e3106024a742665fa83dda`  
		Last Modified: Fri, 07 Oct 2022 21:12:17 GMT  
		Size: 53.8 MB (53817534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afd03a0f65e88ab8ba56cc8cd838d009c7fdea1c1491dccdcf631766227e5d4`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ceb4bec32c454301ab7ef00f268ba79aaa6b1ea01012c3167779ff0c90574c`  
		Last Modified: Fri, 07 Oct 2022 21:12:17 GMT  
		Size: 44.1 MB (44105166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2151a4f39c78b2ecbc36299c2154651d21fa2c2555e1d40582e76b4852ec6a8c`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e70080d6082a60048ca786d5834ca53ccf4cc2b3860b6089fa0f1b8e0cbe15`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:3c1aab708f6e57fc4dccafe36baccc7219acfb4ec450f3fb6d370ea89409e906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:f90d1aeb92a5c7b3a4178a3052d8bc27b1f52a811aacb27b619c10b778b9f281
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133890226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbaea59d1b4194257138a6434ec0820a13097dd7e900135e78daf9759fe2407a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:31:40 GMT
ADD file:40e1b0533d9ae91c868834395cbd4b74cf2a47965791be201c03ae764f9da2b0 in / 
# Fri, 07 Oct 2022 20:31:41 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:05:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:05:33 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:05:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:05:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:06:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:06:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:06:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:07:04 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:07:04 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:07:05 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:07:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:07:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:07:05 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:07:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:295ca23427284cb123fd4c132a1ecb521e7f787ac75dadec342f744a343efec4`  
		Last Modified: Fri, 07 Oct 2022 20:33:22 GMT  
		Size: 40.6 MB (40589568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79af4312a7e0fb060724a99077fbd6a3460284520318bbfe874d11e472aed010`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d3d73d17046a044f9f4a45aa0f74afa79387dc1eb634ef96eb39a947b3077d`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b8724b397717c0920f045a0dc9b778426bb5ed5ff17f2ecaece3b27914fe3`  
		Last Modified: Fri, 07 Oct 2022 21:08:49 GMT  
		Size: 4.6 MB (4606973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cf360b4a14d6543edc2e7f35ce87406aa7b82c29e252f8ef911f39dcbc6de2`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0115482cc006f85365a790dc394ead0f59f922046bb77b3509e6f7989b32b2a5`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a360b08917ea13f41e1d042db0163b46c0069b93a5e2995543ab10fa70541e16`  
		Last Modified: Fri, 07 Oct 2022 21:08:54 GMT  
		Size: 47.7 MB (47733932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12deeb3c132385712ac84f6ab3842432f96d231682957f254fdb8400156b3736`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1dc10db1e9a87dda49ac546d7263db2fd5e6163aa17228c7d60f464bf91098`  
		Last Modified: Fri, 07 Oct 2022 21:08:53 GMT  
		Size: 40.0 MB (40021240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64be404ad29c0faf50a4c5855fcbbb8491b2f8fd89ac4df11b3a0b26f990a4da`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921fe8879a2ef55d203b4ad84ee572904a1afb7b195013a82bc3568b85624e2`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c6f2eef8a149e0efd0515ab57a41f84cf06859eab6babb0b349d8d75e1c68544
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142631938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1699df6c42a3ed6b4a8f6e65ec1886dfab6ab4f213eadc8e44b6f79630d5ac01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:51:45 GMT
ADD file:6eb7b065ffe8855d82638de19bd23fba329883c96f01d093e7bc6bdb5da836a3 in / 
# Fri, 07 Oct 2022 20:51:46 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:09:40 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:09:41 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:09:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:10:14 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:10:16 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:10:17 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 07 Oct 2022 21:10:18 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:10:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:10:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:10:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:10:55 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:11:30 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:11:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:11:32 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:11:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:11:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:11:34 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:11:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d45c82139e084eb338a0a2346c4ec4c6d2bfa4acda9194cf6602728b4a3e89f`  
		Last Modified: Fri, 07 Oct 2022 20:53:34 GMT  
		Size: 39.4 MB (39409020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c544deffc3a52cba4e3a2ec48f677586760eb4717c161c4adebcb8ce20402a8`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af07bf98dff8f0d9fa86a18b24151f9803947d9d622097b25bf3f5874b2bd6c9`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0554dfac498a04af357c6a46c1e81c7a38af77e0f18e416c035c3e64f7d9905e`  
		Last Modified: Fri, 07 Oct 2022 21:12:12 GMT  
		Size: 4.4 MB (4433409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f612237e783e94a541b8163f9f2a3d5d66b3b804fdddcd51e7b752f50f7ffaec`  
		Last Modified: Fri, 07 Oct 2022 21:12:11 GMT  
		Size: 2.6 KB (2610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db27487a0c82f6090e67e6b7ea5caddb59f62cf16ac8c91558438a1b0408525`  
		Last Modified: Fri, 07 Oct 2022 21:12:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87b5be864804505c24ba253a53076347702ebd268e3106024a742665fa83dda`  
		Last Modified: Fri, 07 Oct 2022 21:12:17 GMT  
		Size: 53.8 MB (53817534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afd03a0f65e88ab8ba56cc8cd838d009c7fdea1c1491dccdcf631766227e5d4`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ceb4bec32c454301ab7ef00f268ba79aaa6b1ea01012c3167779ff0c90574c`  
		Last Modified: Fri, 07 Oct 2022 21:12:17 GMT  
		Size: 44.1 MB (44105166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2151a4f39c78b2ecbc36299c2154651d21fa2c2555e1d40582e76b4852ec6a8c`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e70080d6082a60048ca786d5834ca53ccf4cc2b3860b6089fa0f1b8e0cbe15`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:c00749f00b317206048b8eaf304ded3941ecaf452b73a8e178b8ea2d1fc29342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:12477b35d174c1a410da24a05c4884693836e2a863521aa339a1298ce48b8369
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157889330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34e66721c05dacebba2911adc611de5a71b95458b5a7208fb961aa3051b5eec2`
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
# Wed, 05 Oct 2022 04:22:08 GMT
ENV MYSQL_VERSION=8.0.30-1debian11
# Wed, 05 Oct 2022 04:22:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 05 Oct 2022 04:22:23 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 05 Oct 2022 04:22:24 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Oct 2022 04:22:24 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 05 Oct 2022 04:22:24 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:22:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:22:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:22:25 GMT
EXPOSE 3306 33060
# Wed, 05 Oct 2022 04:22:25 GMT
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
	-	`sha256:f1363e6677cacb6f7960a756d9b4c0aa8d4c8ec02869cb4a6d9159faa60ecba4`  
		Last Modified: Wed, 05 Oct 2022 04:23:47 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1110efce5dd0e631830f85c1a0c25efbba11b2e55314c04bb4fc0f97a30fdfc`  
		Last Modified: Wed, 05 Oct 2022 04:24:04 GMT  
		Size: 108.0 MB (107963159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fda2bd249a81a6cde8a8959a44831ac82aa8e5ecf3e1d508cf07ae87454330`  
		Last Modified: Wed, 05 Oct 2022 04:23:47 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89080d4312c49459448781df923db9f843c0f978fc5100842de22d34ce9b142`  
		Last Modified: Wed, 05 Oct 2022 04:23:47 GMT  
		Size: 5.4 KB (5382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d74113edbbb66aa319322589f5e5f54f3ac373cc17fb9a2fdd5c3fe2f877345`  
		Last Modified: Wed, 05 Oct 2022 04:23:47 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:3c1aab708f6e57fc4dccafe36baccc7219acfb4ec450f3fb6d370ea89409e906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:f90d1aeb92a5c7b3a4178a3052d8bc27b1f52a811aacb27b619c10b778b9f281
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133890226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbaea59d1b4194257138a6434ec0820a13097dd7e900135e78daf9759fe2407a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:31:40 GMT
ADD file:40e1b0533d9ae91c868834395cbd4b74cf2a47965791be201c03ae764f9da2b0 in / 
# Fri, 07 Oct 2022 20:31:41 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:05:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:05:33 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:05:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:05:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:06:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:06:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:06:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:07:04 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:07:04 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:07:05 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:07:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:07:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:07:05 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:07:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:295ca23427284cb123fd4c132a1ecb521e7f787ac75dadec342f744a343efec4`  
		Last Modified: Fri, 07 Oct 2022 20:33:22 GMT  
		Size: 40.6 MB (40589568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79af4312a7e0fb060724a99077fbd6a3460284520318bbfe874d11e472aed010`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d3d73d17046a044f9f4a45aa0f74afa79387dc1eb634ef96eb39a947b3077d`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b8724b397717c0920f045a0dc9b778426bb5ed5ff17f2ecaece3b27914fe3`  
		Last Modified: Fri, 07 Oct 2022 21:08:49 GMT  
		Size: 4.6 MB (4606973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cf360b4a14d6543edc2e7f35ce87406aa7b82c29e252f8ef911f39dcbc6de2`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0115482cc006f85365a790dc394ead0f59f922046bb77b3509e6f7989b32b2a5`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a360b08917ea13f41e1d042db0163b46c0069b93a5e2995543ab10fa70541e16`  
		Last Modified: Fri, 07 Oct 2022 21:08:54 GMT  
		Size: 47.7 MB (47733932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12deeb3c132385712ac84f6ab3842432f96d231682957f254fdb8400156b3736`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1dc10db1e9a87dda49ac546d7263db2fd5e6163aa17228c7d60f464bf91098`  
		Last Modified: Fri, 07 Oct 2022 21:08:53 GMT  
		Size: 40.0 MB (40021240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64be404ad29c0faf50a4c5855fcbbb8491b2f8fd89ac4df11b3a0b26f990a4da`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921fe8879a2ef55d203b4ad84ee572904a1afb7b195013a82bc3568b85624e2`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c6f2eef8a149e0efd0515ab57a41f84cf06859eab6babb0b349d8d75e1c68544
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142631938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1699df6c42a3ed6b4a8f6e65ec1886dfab6ab4f213eadc8e44b6f79630d5ac01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:51:45 GMT
ADD file:6eb7b065ffe8855d82638de19bd23fba329883c96f01d093e7bc6bdb5da836a3 in / 
# Fri, 07 Oct 2022 20:51:46 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:09:40 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:09:41 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:09:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:10:14 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:10:16 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:10:17 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 07 Oct 2022 21:10:18 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:10:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:10:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:10:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:10:55 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:11:30 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:11:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:11:32 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:11:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:11:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:11:34 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:11:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d45c82139e084eb338a0a2346c4ec4c6d2bfa4acda9194cf6602728b4a3e89f`  
		Last Modified: Fri, 07 Oct 2022 20:53:34 GMT  
		Size: 39.4 MB (39409020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c544deffc3a52cba4e3a2ec48f677586760eb4717c161c4adebcb8ce20402a8`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af07bf98dff8f0d9fa86a18b24151f9803947d9d622097b25bf3f5874b2bd6c9`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0554dfac498a04af357c6a46c1e81c7a38af77e0f18e416c035c3e64f7d9905e`  
		Last Modified: Fri, 07 Oct 2022 21:12:12 GMT  
		Size: 4.4 MB (4433409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f612237e783e94a541b8163f9f2a3d5d66b3b804fdddcd51e7b752f50f7ffaec`  
		Last Modified: Fri, 07 Oct 2022 21:12:11 GMT  
		Size: 2.6 KB (2610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db27487a0c82f6090e67e6b7ea5caddb59f62cf16ac8c91558438a1b0408525`  
		Last Modified: Fri, 07 Oct 2022 21:12:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87b5be864804505c24ba253a53076347702ebd268e3106024a742665fa83dda`  
		Last Modified: Fri, 07 Oct 2022 21:12:17 GMT  
		Size: 53.8 MB (53817534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afd03a0f65e88ab8ba56cc8cd838d009c7fdea1c1491dccdcf631766227e5d4`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ceb4bec32c454301ab7ef00f268ba79aaa6b1ea01012c3167779ff0c90574c`  
		Last Modified: Fri, 07 Oct 2022 21:12:17 GMT  
		Size: 44.1 MB (44105166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2151a4f39c78b2ecbc36299c2154651d21fa2c2555e1d40582e76b4852ec6a8c`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e70080d6082a60048ca786d5834ca53ccf4cc2b3860b6089fa0f1b8e0cbe15`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31`

**does not exist** (yet?)

## `mysql:8.0.31-debian`

**does not exist** (yet?)

## `mysql:8.0.31-oracle`

**does not exist** (yet?)

## `mysql:debian`

```console
$ docker pull mysql@sha256:c00749f00b317206048b8eaf304ded3941ecaf452b73a8e178b8ea2d1fc29342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:12477b35d174c1a410da24a05c4884693836e2a863521aa339a1298ce48b8369
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157889330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34e66721c05dacebba2911adc611de5a71b95458b5a7208fb961aa3051b5eec2`
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
# Wed, 05 Oct 2022 04:22:08 GMT
ENV MYSQL_VERSION=8.0.30-1debian11
# Wed, 05 Oct 2022 04:22:08 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 05 Oct 2022 04:22:23 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 05 Oct 2022 04:22:24 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Oct 2022 04:22:24 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 05 Oct 2022 04:22:24 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:22:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:22:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:22:25 GMT
EXPOSE 3306 33060
# Wed, 05 Oct 2022 04:22:25 GMT
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
	-	`sha256:f1363e6677cacb6f7960a756d9b4c0aa8d4c8ec02869cb4a6d9159faa60ecba4`  
		Last Modified: Wed, 05 Oct 2022 04:23:47 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1110efce5dd0e631830f85c1a0c25efbba11b2e55314c04bb4fc0f97a30fdfc`  
		Last Modified: Wed, 05 Oct 2022 04:24:04 GMT  
		Size: 108.0 MB (107963159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fda2bd249a81a6cde8a8959a44831ac82aa8e5ecf3e1d508cf07ae87454330`  
		Last Modified: Wed, 05 Oct 2022 04:23:47 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89080d4312c49459448781df923db9f843c0f978fc5100842de22d34ce9b142`  
		Last Modified: Wed, 05 Oct 2022 04:23:47 GMT  
		Size: 5.4 KB (5382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d74113edbbb66aa319322589f5e5f54f3ac373cc17fb9a2fdd5c3fe2f877345`  
		Last Modified: Wed, 05 Oct 2022 04:23:47 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:3c1aab708f6e57fc4dccafe36baccc7219acfb4ec450f3fb6d370ea89409e906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:f90d1aeb92a5c7b3a4178a3052d8bc27b1f52a811aacb27b619c10b778b9f281
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133890226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbaea59d1b4194257138a6434ec0820a13097dd7e900135e78daf9759fe2407a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:31:40 GMT
ADD file:40e1b0533d9ae91c868834395cbd4b74cf2a47965791be201c03ae764f9da2b0 in / 
# Fri, 07 Oct 2022 20:31:41 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:05:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:05:33 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:05:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:05:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:06:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:06:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:06:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:07:04 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:07:04 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:07:05 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:07:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:07:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:07:05 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:07:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:295ca23427284cb123fd4c132a1ecb521e7f787ac75dadec342f744a343efec4`  
		Last Modified: Fri, 07 Oct 2022 20:33:22 GMT  
		Size: 40.6 MB (40589568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79af4312a7e0fb060724a99077fbd6a3460284520318bbfe874d11e472aed010`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d3d73d17046a044f9f4a45aa0f74afa79387dc1eb634ef96eb39a947b3077d`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b8724b397717c0920f045a0dc9b778426bb5ed5ff17f2ecaece3b27914fe3`  
		Last Modified: Fri, 07 Oct 2022 21:08:49 GMT  
		Size: 4.6 MB (4606973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cf360b4a14d6543edc2e7f35ce87406aa7b82c29e252f8ef911f39dcbc6de2`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0115482cc006f85365a790dc394ead0f59f922046bb77b3509e6f7989b32b2a5`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a360b08917ea13f41e1d042db0163b46c0069b93a5e2995543ab10fa70541e16`  
		Last Modified: Fri, 07 Oct 2022 21:08:54 GMT  
		Size: 47.7 MB (47733932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12deeb3c132385712ac84f6ab3842432f96d231682957f254fdb8400156b3736`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1dc10db1e9a87dda49ac546d7263db2fd5e6163aa17228c7d60f464bf91098`  
		Last Modified: Fri, 07 Oct 2022 21:08:53 GMT  
		Size: 40.0 MB (40021240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64be404ad29c0faf50a4c5855fcbbb8491b2f8fd89ac4df11b3a0b26f990a4da`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921fe8879a2ef55d203b4ad84ee572904a1afb7b195013a82bc3568b85624e2`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c6f2eef8a149e0efd0515ab57a41f84cf06859eab6babb0b349d8d75e1c68544
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142631938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1699df6c42a3ed6b4a8f6e65ec1886dfab6ab4f213eadc8e44b6f79630d5ac01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:51:45 GMT
ADD file:6eb7b065ffe8855d82638de19bd23fba329883c96f01d093e7bc6bdb5da836a3 in / 
# Fri, 07 Oct 2022 20:51:46 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:09:40 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:09:41 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:09:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:10:14 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:10:16 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:10:17 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 07 Oct 2022 21:10:18 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:10:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:10:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:10:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:10:55 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:11:30 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:11:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:11:32 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:11:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:11:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:11:34 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:11:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d45c82139e084eb338a0a2346c4ec4c6d2bfa4acda9194cf6602728b4a3e89f`  
		Last Modified: Fri, 07 Oct 2022 20:53:34 GMT  
		Size: 39.4 MB (39409020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c544deffc3a52cba4e3a2ec48f677586760eb4717c161c4adebcb8ce20402a8`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af07bf98dff8f0d9fa86a18b24151f9803947d9d622097b25bf3f5874b2bd6c9`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0554dfac498a04af357c6a46c1e81c7a38af77e0f18e416c035c3e64f7d9905e`  
		Last Modified: Fri, 07 Oct 2022 21:12:12 GMT  
		Size: 4.4 MB (4433409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f612237e783e94a541b8163f9f2a3d5d66b3b804fdddcd51e7b752f50f7ffaec`  
		Last Modified: Fri, 07 Oct 2022 21:12:11 GMT  
		Size: 2.6 KB (2610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db27487a0c82f6090e67e6b7ea5caddb59f62cf16ac8c91558438a1b0408525`  
		Last Modified: Fri, 07 Oct 2022 21:12:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87b5be864804505c24ba253a53076347702ebd268e3106024a742665fa83dda`  
		Last Modified: Fri, 07 Oct 2022 21:12:17 GMT  
		Size: 53.8 MB (53817534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afd03a0f65e88ab8ba56cc8cd838d009c7fdea1c1491dccdcf631766227e5d4`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ceb4bec32c454301ab7ef00f268ba79aaa6b1ea01012c3167779ff0c90574c`  
		Last Modified: Fri, 07 Oct 2022 21:12:17 GMT  
		Size: 44.1 MB (44105166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2151a4f39c78b2ecbc36299c2154651d21fa2c2555e1d40582e76b4852ec6a8c`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e70080d6082a60048ca786d5834ca53ccf4cc2b3860b6089fa0f1b8e0cbe15`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:3c1aab708f6e57fc4dccafe36baccc7219acfb4ec450f3fb6d370ea89409e906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:f90d1aeb92a5c7b3a4178a3052d8bc27b1f52a811aacb27b619c10b778b9f281
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133890226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbaea59d1b4194257138a6434ec0820a13097dd7e900135e78daf9759fe2407a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:31:40 GMT
ADD file:40e1b0533d9ae91c868834395cbd4b74cf2a47965791be201c03ae764f9da2b0 in / 
# Fri, 07 Oct 2022 20:31:41 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:05:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:05:33 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:05:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:05:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:06:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:06:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:06:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:07:04 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:07:04 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:07:05 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:07:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:07:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:07:05 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:07:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:295ca23427284cb123fd4c132a1ecb521e7f787ac75dadec342f744a343efec4`  
		Last Modified: Fri, 07 Oct 2022 20:33:22 GMT  
		Size: 40.6 MB (40589568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79af4312a7e0fb060724a99077fbd6a3460284520318bbfe874d11e472aed010`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d3d73d17046a044f9f4a45aa0f74afa79387dc1eb634ef96eb39a947b3077d`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b8724b397717c0920f045a0dc9b778426bb5ed5ff17f2ecaece3b27914fe3`  
		Last Modified: Fri, 07 Oct 2022 21:08:49 GMT  
		Size: 4.6 MB (4606973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cf360b4a14d6543edc2e7f35ce87406aa7b82c29e252f8ef911f39dcbc6de2`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0115482cc006f85365a790dc394ead0f59f922046bb77b3509e6f7989b32b2a5`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a360b08917ea13f41e1d042db0163b46c0069b93a5e2995543ab10fa70541e16`  
		Last Modified: Fri, 07 Oct 2022 21:08:54 GMT  
		Size: 47.7 MB (47733932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12deeb3c132385712ac84f6ab3842432f96d231682957f254fdb8400156b3736`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1dc10db1e9a87dda49ac546d7263db2fd5e6163aa17228c7d60f464bf91098`  
		Last Modified: Fri, 07 Oct 2022 21:08:53 GMT  
		Size: 40.0 MB (40021240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64be404ad29c0faf50a4c5855fcbbb8491b2f8fd89ac4df11b3a0b26f990a4da`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921fe8879a2ef55d203b4ad84ee572904a1afb7b195013a82bc3568b85624e2`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c6f2eef8a149e0efd0515ab57a41f84cf06859eab6babb0b349d8d75e1c68544
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142631938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1699df6c42a3ed6b4a8f6e65ec1886dfab6ab4f213eadc8e44b6f79630d5ac01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:51:45 GMT
ADD file:6eb7b065ffe8855d82638de19bd23fba329883c96f01d093e7bc6bdb5da836a3 in / 
# Fri, 07 Oct 2022 20:51:46 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:09:40 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:09:41 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:09:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:10:14 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:10:16 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:10:17 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 07 Oct 2022 21:10:18 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:10:19 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:10:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:10:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:10:55 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:11:30 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:11:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:11:32 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:11:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:11:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:11:34 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:11:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d45c82139e084eb338a0a2346c4ec4c6d2bfa4acda9194cf6602728b4a3e89f`  
		Last Modified: Fri, 07 Oct 2022 20:53:34 GMT  
		Size: 39.4 MB (39409020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c544deffc3a52cba4e3a2ec48f677586760eb4717c161c4adebcb8ce20402a8`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af07bf98dff8f0d9fa86a18b24151f9803947d9d622097b25bf3f5874b2bd6c9`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0554dfac498a04af357c6a46c1e81c7a38af77e0f18e416c035c3e64f7d9905e`  
		Last Modified: Fri, 07 Oct 2022 21:12:12 GMT  
		Size: 4.4 MB (4433409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f612237e783e94a541b8163f9f2a3d5d66b3b804fdddcd51e7b752f50f7ffaec`  
		Last Modified: Fri, 07 Oct 2022 21:12:11 GMT  
		Size: 2.6 KB (2610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db27487a0c82f6090e67e6b7ea5caddb59f62cf16ac8c91558438a1b0408525`  
		Last Modified: Fri, 07 Oct 2022 21:12:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87b5be864804505c24ba253a53076347702ebd268e3106024a742665fa83dda`  
		Last Modified: Fri, 07 Oct 2022 21:12:17 GMT  
		Size: 53.8 MB (53817534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afd03a0f65e88ab8ba56cc8cd838d009c7fdea1c1491dccdcf631766227e5d4`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ceb4bec32c454301ab7ef00f268ba79aaa6b1ea01012c3167779ff0c90574c`  
		Last Modified: Fri, 07 Oct 2022 21:12:17 GMT  
		Size: 44.1 MB (44105166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2151a4f39c78b2ecbc36299c2154651d21fa2c2555e1d40582e76b4852ec6a8c`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e70080d6082a60048ca786d5834ca53ccf4cc2b3860b6089fa0f1b8e0cbe15`  
		Last Modified: Fri, 07 Oct 2022 21:12:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
