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
$ docker pull mysql@sha256:f5e2d4d7dccdc3f2a1d592bd3f0eb472b2f72f9fb942a84ff5b5cc049fe63a04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:64dc581e69a2e37825c4f669c2c5903f258d8fca529632c73c5e7c8095432c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144333003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14905234a4ed471d6da5b7e09d9e9f62f4d350713e2b0e8c86652ebcbf710238`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:21:18 GMT
ADD file:33b52c7a287bb91adb106cbb8b7e7bd3d38684f4aa9d19b7ef1f1af5e7288aa3 in / 
# Fri, 21 Oct 2022 19:21:18 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:47:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:47:51 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:47:55 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:48:14 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 21 Oct 2022 19:48:15 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:48:15 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 21 Oct 2022 19:48:15 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Fri, 21 Oct 2022 19:48:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:48:34 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:48:35 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:48:35 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Fri, 21 Oct 2022 19:48:59 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:49:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:49:00 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:49:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:49:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:49:00 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:49:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c19d5474d2cf2e83fc2be2ee3116c33e32d707b2ca5688ce2b086a0c318e62bd`  
		Last Modified: Fri, 21 Oct 2022 19:23:18 GMT  
		Size: 49.9 MB (49856127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734cfb67bc8c9872bd458b7c82e7bc3eca010f38a4ccac07d863814eee2f1b07`  
		Last Modified: Fri, 21 Oct 2022 19:50:22 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729529a0299eeb95c68e8bfdbc237b671d751e84bfc592bca377c27cf1e31161`  
		Last Modified: Fri, 21 Oct 2022 19:50:22 GMT  
		Size: 930.2 KB (930221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d3c603a591da29f582821512adaf4197fe52d1aa3ac42491aad2128955d8b4`  
		Last Modified: Fri, 21 Oct 2022 19:50:21 GMT  
		Size: 4.5 MB (4546654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e0fbc2dcba0e8cb13b1616914d09abacc8e4147bf12a3b5ceca138092304e`  
		Last Modified: Fri, 21 Oct 2022 19:50:19 GMT  
		Size: 2.7 KB (2661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7d48a00fea276947ad91562783d98ed45ab5e77fa93552cd0a3ef3a46804d4`  
		Last Modified: Fri, 21 Oct 2022 19:50:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf883b19c2f3cff48bacc06c394c73797b49be19dbebeda4580ed88da02bf8f`  
		Last Modified: Fri, 21 Oct 2022 19:50:21 GMT  
		Size: 25.5 MB (25530033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28356e1795930ab9e9381e3865ad898ca95634fc19e4425e1ae28afcd3c49412`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49abbf373312d0ae94e6305d1eb72750dce128536fd6856d127c48e61aa19086`  
		Last Modified: Fri, 21 Oct 2022 19:50:29 GMT  
		Size: 63.5 MB (63460272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce6621986fd3a5a82e124a82937242e3f839efa4e051f4cb9925e50ee46806a`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d631e923a6f3a6ed2683dbbeda6ad90723ead236157f68e506999448fd6685`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:30b60035d8a8ef0e7afbf93c1971c32628d4057af70ac4af3fd075295c7af6fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:3d1cdc617796d5ca74e8274e3ca7e09fd1fa866c4cc212d50800ecefb91b1d0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162584236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f96dd5bb38e835c3f577df00093874a5e9e3204aa02b2dbdd7d474e930c47d4`
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
# Wed, 19 Oct 2022 19:24:37 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:24:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Oct 2022 19:24:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:24:38 GMT
EXPOSE 3306 33060
# Wed, 19 Oct 2022 19:24:38 GMT
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
	-	`sha256:ae26252a4842291e990d3c88ca2f76dca347fcddb948410700649560f64d9e68`  
		Last Modified: Wed, 19 Oct 2022 19:26:09 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a814758d959bdc1466e7666a47cd5adb692773f19e76102f9082fd83d47518ed`  
		Last Modified: Wed, 19 Oct 2022 19:26:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:f5e2d4d7dccdc3f2a1d592bd3f0eb472b2f72f9fb942a84ff5b5cc049fe63a04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:64dc581e69a2e37825c4f669c2c5903f258d8fca529632c73c5e7c8095432c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144333003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14905234a4ed471d6da5b7e09d9e9f62f4d350713e2b0e8c86652ebcbf710238`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:21:18 GMT
ADD file:33b52c7a287bb91adb106cbb8b7e7bd3d38684f4aa9d19b7ef1f1af5e7288aa3 in / 
# Fri, 21 Oct 2022 19:21:18 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:47:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:47:51 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:47:55 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:48:14 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 21 Oct 2022 19:48:15 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:48:15 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 21 Oct 2022 19:48:15 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Fri, 21 Oct 2022 19:48:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:48:34 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:48:35 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:48:35 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Fri, 21 Oct 2022 19:48:59 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:49:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:49:00 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:49:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:49:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:49:00 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:49:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c19d5474d2cf2e83fc2be2ee3116c33e32d707b2ca5688ce2b086a0c318e62bd`  
		Last Modified: Fri, 21 Oct 2022 19:23:18 GMT  
		Size: 49.9 MB (49856127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734cfb67bc8c9872bd458b7c82e7bc3eca010f38a4ccac07d863814eee2f1b07`  
		Last Modified: Fri, 21 Oct 2022 19:50:22 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729529a0299eeb95c68e8bfdbc237b671d751e84bfc592bca377c27cf1e31161`  
		Last Modified: Fri, 21 Oct 2022 19:50:22 GMT  
		Size: 930.2 KB (930221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d3c603a591da29f582821512adaf4197fe52d1aa3ac42491aad2128955d8b4`  
		Last Modified: Fri, 21 Oct 2022 19:50:21 GMT  
		Size: 4.5 MB (4546654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e0fbc2dcba0e8cb13b1616914d09abacc8e4147bf12a3b5ceca138092304e`  
		Last Modified: Fri, 21 Oct 2022 19:50:19 GMT  
		Size: 2.7 KB (2661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7d48a00fea276947ad91562783d98ed45ab5e77fa93552cd0a3ef3a46804d4`  
		Last Modified: Fri, 21 Oct 2022 19:50:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf883b19c2f3cff48bacc06c394c73797b49be19dbebeda4580ed88da02bf8f`  
		Last Modified: Fri, 21 Oct 2022 19:50:21 GMT  
		Size: 25.5 MB (25530033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28356e1795930ab9e9381e3865ad898ca95634fc19e4425e1ae28afcd3c49412`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49abbf373312d0ae94e6305d1eb72750dce128536fd6856d127c48e61aa19086`  
		Last Modified: Fri, 21 Oct 2022 19:50:29 GMT  
		Size: 63.5 MB (63460272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce6621986fd3a5a82e124a82937242e3f839efa4e051f4cb9925e50ee46806a`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d631e923a6f3a6ed2683dbbeda6ad90723ead236157f68e506999448fd6685`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:f5e2d4d7dccdc3f2a1d592bd3f0eb472b2f72f9fb942a84ff5b5cc049fe63a04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:64dc581e69a2e37825c4f669c2c5903f258d8fca529632c73c5e7c8095432c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144333003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14905234a4ed471d6da5b7e09d9e9f62f4d350713e2b0e8c86652ebcbf710238`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:21:18 GMT
ADD file:33b52c7a287bb91adb106cbb8b7e7bd3d38684f4aa9d19b7ef1f1af5e7288aa3 in / 
# Fri, 21 Oct 2022 19:21:18 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:47:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:47:51 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:47:55 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:48:14 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 21 Oct 2022 19:48:15 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:48:15 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 21 Oct 2022 19:48:15 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Fri, 21 Oct 2022 19:48:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:48:34 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:48:35 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:48:35 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Fri, 21 Oct 2022 19:48:59 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:49:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:49:00 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:49:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:49:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:49:00 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:49:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c19d5474d2cf2e83fc2be2ee3116c33e32d707b2ca5688ce2b086a0c318e62bd`  
		Last Modified: Fri, 21 Oct 2022 19:23:18 GMT  
		Size: 49.9 MB (49856127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734cfb67bc8c9872bd458b7c82e7bc3eca010f38a4ccac07d863814eee2f1b07`  
		Last Modified: Fri, 21 Oct 2022 19:50:22 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729529a0299eeb95c68e8bfdbc237b671d751e84bfc592bca377c27cf1e31161`  
		Last Modified: Fri, 21 Oct 2022 19:50:22 GMT  
		Size: 930.2 KB (930221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d3c603a591da29f582821512adaf4197fe52d1aa3ac42491aad2128955d8b4`  
		Last Modified: Fri, 21 Oct 2022 19:50:21 GMT  
		Size: 4.5 MB (4546654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e0fbc2dcba0e8cb13b1616914d09abacc8e4147bf12a3b5ceca138092304e`  
		Last Modified: Fri, 21 Oct 2022 19:50:19 GMT  
		Size: 2.7 KB (2661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7d48a00fea276947ad91562783d98ed45ab5e77fa93552cd0a3ef3a46804d4`  
		Last Modified: Fri, 21 Oct 2022 19:50:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf883b19c2f3cff48bacc06c394c73797b49be19dbebeda4580ed88da02bf8f`  
		Last Modified: Fri, 21 Oct 2022 19:50:21 GMT  
		Size: 25.5 MB (25530033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28356e1795930ab9e9381e3865ad898ca95634fc19e4425e1ae28afcd3c49412`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49abbf373312d0ae94e6305d1eb72750dce128536fd6856d127c48e61aa19086`  
		Last Modified: Fri, 21 Oct 2022 19:50:29 GMT  
		Size: 63.5 MB (63460272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce6621986fd3a5a82e124a82937242e3f839efa4e051f4cb9925e50ee46806a`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d631e923a6f3a6ed2683dbbeda6ad90723ead236157f68e506999448fd6685`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:30b60035d8a8ef0e7afbf93c1971c32628d4057af70ac4af3fd075295c7af6fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:3d1cdc617796d5ca74e8274e3ca7e09fd1fa866c4cc212d50800ecefb91b1d0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162584236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f96dd5bb38e835c3f577df00093874a5e9e3204aa02b2dbdd7d474e930c47d4`
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
# Wed, 19 Oct 2022 19:24:37 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:24:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Oct 2022 19:24:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:24:38 GMT
EXPOSE 3306 33060
# Wed, 19 Oct 2022 19:24:38 GMT
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
	-	`sha256:ae26252a4842291e990d3c88ca2f76dca347fcddb948410700649560f64d9e68`  
		Last Modified: Wed, 19 Oct 2022 19:26:09 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a814758d959bdc1466e7666a47cd5adb692773f19e76102f9082fd83d47518ed`  
		Last Modified: Wed, 19 Oct 2022 19:26:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:f5e2d4d7dccdc3f2a1d592bd3f0eb472b2f72f9fb942a84ff5b5cc049fe63a04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:64dc581e69a2e37825c4f669c2c5903f258d8fca529632c73c5e7c8095432c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144333003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14905234a4ed471d6da5b7e09d9e9f62f4d350713e2b0e8c86652ebcbf710238`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:21:18 GMT
ADD file:33b52c7a287bb91adb106cbb8b7e7bd3d38684f4aa9d19b7ef1f1af5e7288aa3 in / 
# Fri, 21 Oct 2022 19:21:18 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:47:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:47:51 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:47:55 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:48:14 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 21 Oct 2022 19:48:15 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:48:15 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 21 Oct 2022 19:48:15 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Fri, 21 Oct 2022 19:48:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:48:34 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:48:35 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:48:35 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Fri, 21 Oct 2022 19:48:59 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:49:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:49:00 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:49:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:49:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:49:00 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:49:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c19d5474d2cf2e83fc2be2ee3116c33e32d707b2ca5688ce2b086a0c318e62bd`  
		Last Modified: Fri, 21 Oct 2022 19:23:18 GMT  
		Size: 49.9 MB (49856127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734cfb67bc8c9872bd458b7c82e7bc3eca010f38a4ccac07d863814eee2f1b07`  
		Last Modified: Fri, 21 Oct 2022 19:50:22 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729529a0299eeb95c68e8bfdbc237b671d751e84bfc592bca377c27cf1e31161`  
		Last Modified: Fri, 21 Oct 2022 19:50:22 GMT  
		Size: 930.2 KB (930221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d3c603a591da29f582821512adaf4197fe52d1aa3ac42491aad2128955d8b4`  
		Last Modified: Fri, 21 Oct 2022 19:50:21 GMT  
		Size: 4.5 MB (4546654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e0fbc2dcba0e8cb13b1616914d09abacc8e4147bf12a3b5ceca138092304e`  
		Last Modified: Fri, 21 Oct 2022 19:50:19 GMT  
		Size: 2.7 KB (2661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7d48a00fea276947ad91562783d98ed45ab5e77fa93552cd0a3ef3a46804d4`  
		Last Modified: Fri, 21 Oct 2022 19:50:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf883b19c2f3cff48bacc06c394c73797b49be19dbebeda4580ed88da02bf8f`  
		Last Modified: Fri, 21 Oct 2022 19:50:21 GMT  
		Size: 25.5 MB (25530033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28356e1795930ab9e9381e3865ad898ca95634fc19e4425e1ae28afcd3c49412`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49abbf373312d0ae94e6305d1eb72750dce128536fd6856d127c48e61aa19086`  
		Last Modified: Fri, 21 Oct 2022 19:50:29 GMT  
		Size: 63.5 MB (63460272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce6621986fd3a5a82e124a82937242e3f839efa4e051f4cb9925e50ee46806a`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d631e923a6f3a6ed2683dbbeda6ad90723ead236157f68e506999448fd6685`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40`

```console
$ docker pull mysql@sha256:f5e2d4d7dccdc3f2a1d592bd3f0eb472b2f72f9fb942a84ff5b5cc049fe63a04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40` - linux; amd64

```console
$ docker pull mysql@sha256:64dc581e69a2e37825c4f669c2c5903f258d8fca529632c73c5e7c8095432c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144333003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14905234a4ed471d6da5b7e09d9e9f62f4d350713e2b0e8c86652ebcbf710238`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:21:18 GMT
ADD file:33b52c7a287bb91adb106cbb8b7e7bd3d38684f4aa9d19b7ef1f1af5e7288aa3 in / 
# Fri, 21 Oct 2022 19:21:18 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:47:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:47:51 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:47:55 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:48:14 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 21 Oct 2022 19:48:15 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:48:15 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 21 Oct 2022 19:48:15 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Fri, 21 Oct 2022 19:48:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:48:34 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:48:35 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:48:35 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Fri, 21 Oct 2022 19:48:59 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:49:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:49:00 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:49:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:49:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:49:00 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:49:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c19d5474d2cf2e83fc2be2ee3116c33e32d707b2ca5688ce2b086a0c318e62bd`  
		Last Modified: Fri, 21 Oct 2022 19:23:18 GMT  
		Size: 49.9 MB (49856127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734cfb67bc8c9872bd458b7c82e7bc3eca010f38a4ccac07d863814eee2f1b07`  
		Last Modified: Fri, 21 Oct 2022 19:50:22 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729529a0299eeb95c68e8bfdbc237b671d751e84bfc592bca377c27cf1e31161`  
		Last Modified: Fri, 21 Oct 2022 19:50:22 GMT  
		Size: 930.2 KB (930221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d3c603a591da29f582821512adaf4197fe52d1aa3ac42491aad2128955d8b4`  
		Last Modified: Fri, 21 Oct 2022 19:50:21 GMT  
		Size: 4.5 MB (4546654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e0fbc2dcba0e8cb13b1616914d09abacc8e4147bf12a3b5ceca138092304e`  
		Last Modified: Fri, 21 Oct 2022 19:50:19 GMT  
		Size: 2.7 KB (2661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7d48a00fea276947ad91562783d98ed45ab5e77fa93552cd0a3ef3a46804d4`  
		Last Modified: Fri, 21 Oct 2022 19:50:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf883b19c2f3cff48bacc06c394c73797b49be19dbebeda4580ed88da02bf8f`  
		Last Modified: Fri, 21 Oct 2022 19:50:21 GMT  
		Size: 25.5 MB (25530033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28356e1795930ab9e9381e3865ad898ca95634fc19e4425e1ae28afcd3c49412`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49abbf373312d0ae94e6305d1eb72750dce128536fd6856d127c48e61aa19086`  
		Last Modified: Fri, 21 Oct 2022 19:50:29 GMT  
		Size: 63.5 MB (63460272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce6621986fd3a5a82e124a82937242e3f839efa4e051f4cb9925e50ee46806a`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d631e923a6f3a6ed2683dbbeda6ad90723ead236157f68e506999448fd6685`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40-debian`

```console
$ docker pull mysql@sha256:30b60035d8a8ef0e7afbf93c1971c32628d4057af70ac4af3fd075295c7af6fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40-debian` - linux; amd64

```console
$ docker pull mysql@sha256:3d1cdc617796d5ca74e8274e3ca7e09fd1fa866c4cc212d50800ecefb91b1d0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162584236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f96dd5bb38e835c3f577df00093874a5e9e3204aa02b2dbdd7d474e930c47d4`
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
# Wed, 19 Oct 2022 19:24:37 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:24:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Oct 2022 19:24:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:24:38 GMT
EXPOSE 3306 33060
# Wed, 19 Oct 2022 19:24:38 GMT
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
	-	`sha256:ae26252a4842291e990d3c88ca2f76dca347fcddb948410700649560f64d9e68`  
		Last Modified: Wed, 19 Oct 2022 19:26:09 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a814758d959bdc1466e7666a47cd5adb692773f19e76102f9082fd83d47518ed`  
		Last Modified: Wed, 19 Oct 2022 19:26:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40-oracle`

```console
$ docker pull mysql@sha256:f5e2d4d7dccdc3f2a1d592bd3f0eb472b2f72f9fb942a84ff5b5cc049fe63a04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:64dc581e69a2e37825c4f669c2c5903f258d8fca529632c73c5e7c8095432c04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144333003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14905234a4ed471d6da5b7e09d9e9f62f4d350713e2b0e8c86652ebcbf710238`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:21:18 GMT
ADD file:33b52c7a287bb91adb106cbb8b7e7bd3d38684f4aa9d19b7ef1f1af5e7288aa3 in / 
# Fri, 21 Oct 2022 19:21:18 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:47:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:47:51 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:47:55 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:48:14 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 21 Oct 2022 19:48:15 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:48:15 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 21 Oct 2022 19:48:15 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Fri, 21 Oct 2022 19:48:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:48:34 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:48:35 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:48:35 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Fri, 21 Oct 2022 19:48:59 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:49:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:49:00 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:49:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:49:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:49:00 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:49:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c19d5474d2cf2e83fc2be2ee3116c33e32d707b2ca5688ce2b086a0c318e62bd`  
		Last Modified: Fri, 21 Oct 2022 19:23:18 GMT  
		Size: 49.9 MB (49856127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734cfb67bc8c9872bd458b7c82e7bc3eca010f38a4ccac07d863814eee2f1b07`  
		Last Modified: Fri, 21 Oct 2022 19:50:22 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729529a0299eeb95c68e8bfdbc237b671d751e84bfc592bca377c27cf1e31161`  
		Last Modified: Fri, 21 Oct 2022 19:50:22 GMT  
		Size: 930.2 KB (930221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d3c603a591da29f582821512adaf4197fe52d1aa3ac42491aad2128955d8b4`  
		Last Modified: Fri, 21 Oct 2022 19:50:21 GMT  
		Size: 4.5 MB (4546654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e0fbc2dcba0e8cb13b1616914d09abacc8e4147bf12a3b5ceca138092304e`  
		Last Modified: Fri, 21 Oct 2022 19:50:19 GMT  
		Size: 2.7 KB (2661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7d48a00fea276947ad91562783d98ed45ab5e77fa93552cd0a3ef3a46804d4`  
		Last Modified: Fri, 21 Oct 2022 19:50:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf883b19c2f3cff48bacc06c394c73797b49be19dbebeda4580ed88da02bf8f`  
		Last Modified: Fri, 21 Oct 2022 19:50:21 GMT  
		Size: 25.5 MB (25530033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28356e1795930ab9e9381e3865ad898ca95634fc19e4425e1ae28afcd3c49412`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49abbf373312d0ae94e6305d1eb72750dce128536fd6856d127c48e61aa19086`  
		Last Modified: Fri, 21 Oct 2022 19:50:29 GMT  
		Size: 63.5 MB (63460272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce6621986fd3a5a82e124a82937242e3f839efa4e051f4cb9925e50ee46806a`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d631e923a6f3a6ed2683dbbeda6ad90723ead236157f68e506999448fd6685`  
		Last Modified: Fri, 21 Oct 2022 19:50:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:06314a7a220f6043436cfd72fd9c7f174fd58ef69fe4b788625fa53be4ab66aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:fe2a93f68a7ddef56a39cbc8b3faaf41ca6c910978255119941c1b71899aa6c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157264983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fad08b3c84be3e9164f86153224ab616bf71ee2c79677154c2e5cd3179cccfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:54 GMT
ADD file:66ffe38a497f15c1941fcc4c64fda875cf27856f2ade5128546c10590c5ca84a in / 
# Fri, 21 Oct 2022 19:20:54 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:46:11 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:46:11 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:46:14 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:46:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 19:46:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:46:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:47:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:47:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:47:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:47:43 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:47:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:47:44 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:47:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:47:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:47:45 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:47:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:50cbc88660a5576a306374b5ee70e3e8aeb602409e05ffa41cd4680769ae0574`  
		Last Modified: Fri, 21 Oct 2022 19:22:39 GMT  
		Size: 40.6 MB (40588747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ca853f7184003ce4a998ddf789288fb6bca33039a73cbd4ba03ba525f27bb7`  
		Last Modified: Fri, 21 Oct 2022 19:49:41 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a20476962308f364c624cd515a836f813023b7bff68e93ae6aeac715b0e8f21`  
		Last Modified: Fri, 21 Oct 2022 19:49:42 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3fea56f9fb03595109612dc70a638e205294bcdda1964e39dd3851ee949fff`  
		Last Modified: Fri, 21 Oct 2022 19:49:40 GMT  
		Size: 4.6 MB (4607033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b058249d3104921cd4d5c5885643a97a8be8f9a69124fc9beed35cf791a0813f`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5014a20163fa346756c80c1114d1ea993e9478cdfb6c08da61684a56b3e2af`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906aa7388ee2006b8f4362b5e9e068081be6bfc44a8f3b2bcddd6921cf7d54c7`  
		Last Modified: Fri, 21 Oct 2022 19:49:46 GMT  
		Size: 56.0 MB (56046468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5e2150967eeafa4e4e92254de9f529ea591d2d4b32ac6bf879b2cdb510222`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6b15dcdf4eda4c5061aefe4f754f90946717295e7fa5ea7dbaccff2b4f368f`  
		Last Modified: Fri, 21 Oct 2022 19:49:48 GMT  
		Size: 55.1 MB (55084220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21de4337b977fd518044876a04543776db696d6bc40559290e2dc785f3fa1cd2`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dab154f2aeb6b8b6a8282f9df9d12aea07b392a14b82d9f9d04003f9588863`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:5dae1c4fb603384ad5f68d3a792e5cc1095c23740785261740f00d0739e097b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155562941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7d53e5f7cab773dc36cea9ba5009d948dbffd06acceb29c4ffed2f75f4ad51f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:41:03 GMT
ADD file:2ccafa0c5b388d404f1100108ad9a9cb06c3e4ca4543c4b0f2aadfd9c4b97e45 in / 
# Fri, 21 Oct 2022 19:41:03 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 20:02:14 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 20:02:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 20:02:20 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 20:02:42 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 20:02:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 20:02:44 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 20:02:45 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:02:46 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 20:03:19 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 20:03:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 20:03:20 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:03:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 20:03:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 20:03:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 20:03:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 20:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 20:03:57 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 20:03:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ba2bcb842ee086f4d448ac74f4e172e2568d56d24e6efae9b402c0e37f418943`  
		Last Modified: Fri, 21 Oct 2022 19:42:50 GMT  
		Size: 39.4 MB (39408151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f573f3d8f30de658c99546dfd56922e80e9293938b142d28198865c4c4a9ac`  
		Last Modified: Fri, 21 Oct 2022 20:04:33 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4de9dcca6a477790d74ccaf1a44e93d82058c1abfe8acc7d9949cd166f40e03`  
		Last Modified: Fri, 21 Oct 2022 20:04:34 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3d1d1f0399c6049042613a98e9c464de870d057f8589f496ad644fca5baad8`  
		Last Modified: Fri, 21 Oct 2022 20:04:32 GMT  
		Size: 4.4 MB (4433279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283bc354d9b803601a6cfc1b2c93b8497c0eca55ca6c4180663c547784192ce9`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef2e77bf45616b4d382065d9adcf89ae082529714fb253e1672aed550a3d166`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d13a94caf14e2d057950a534f5c7bb6e3ea40449ac98341a77d3de764270b6`  
		Last Modified: Fri, 21 Oct 2022 20:04:37 GMT  
		Size: 55.4 MB (55421386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c1f1629008ad09afd71e6e8ac0337985cf8bb01382d50dfcbad35efa1789cb`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f892d0f3ede917e6800f61a5c88869e6897dd7a85dd6664d864f9a17b5757c64`  
		Last Modified: Fri, 21 Oct 2022 20:04:39 GMT  
		Size: 55.4 MB (55433315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346b88d5e2639641c57de86ca6641db6b00fdb7908b52bbfce8d5c2809b78039`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998f0dbf65c702dbec59a92b1a9238a7cdc44967a4d67908b9153a401781bf11`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:6da07a43b1ca31cb3e7e3d420de6a91682f0b8f4231888eafb11d86a3806d9e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:e6fb4c622766a92a7f2eda90f5208b863c206511504e77d805971f1944103212
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177571480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ffa4b21891e5a2ed6c1af823d9981d52d3a6d68dff7cc3d544760fb5815215`
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
# Wed, 19 Oct 2022 19:24:29 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:24:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Oct 2022 19:24:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:24:30 GMT
EXPOSE 3306 33060
# Wed, 19 Oct 2022 19:24:30 GMT
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
	-	`sha256:bd5bd9407260ce1a7ee0cd4090756c9dea74c7ff2e0f9f67707bcd3a0afedea5`  
		Last Modified: Wed, 19 Oct 2022 19:25:32 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5227be166f712520b21a76c9ed1e61648494703fa3c3b55d0d3fcaeabe32547f`  
		Last Modified: Wed, 19 Oct 2022 19:25:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:06314a7a220f6043436cfd72fd9c7f174fd58ef69fe4b788625fa53be4ab66aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:fe2a93f68a7ddef56a39cbc8b3faaf41ca6c910978255119941c1b71899aa6c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157264983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fad08b3c84be3e9164f86153224ab616bf71ee2c79677154c2e5cd3179cccfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:54 GMT
ADD file:66ffe38a497f15c1941fcc4c64fda875cf27856f2ade5128546c10590c5ca84a in / 
# Fri, 21 Oct 2022 19:20:54 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:46:11 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:46:11 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:46:14 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:46:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 19:46:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:46:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:47:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:47:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:47:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:47:43 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:47:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:47:44 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:47:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:47:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:47:45 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:47:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:50cbc88660a5576a306374b5ee70e3e8aeb602409e05ffa41cd4680769ae0574`  
		Last Modified: Fri, 21 Oct 2022 19:22:39 GMT  
		Size: 40.6 MB (40588747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ca853f7184003ce4a998ddf789288fb6bca33039a73cbd4ba03ba525f27bb7`  
		Last Modified: Fri, 21 Oct 2022 19:49:41 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a20476962308f364c624cd515a836f813023b7bff68e93ae6aeac715b0e8f21`  
		Last Modified: Fri, 21 Oct 2022 19:49:42 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3fea56f9fb03595109612dc70a638e205294bcdda1964e39dd3851ee949fff`  
		Last Modified: Fri, 21 Oct 2022 19:49:40 GMT  
		Size: 4.6 MB (4607033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b058249d3104921cd4d5c5885643a97a8be8f9a69124fc9beed35cf791a0813f`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5014a20163fa346756c80c1114d1ea993e9478cdfb6c08da61684a56b3e2af`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906aa7388ee2006b8f4362b5e9e068081be6bfc44a8f3b2bcddd6921cf7d54c7`  
		Last Modified: Fri, 21 Oct 2022 19:49:46 GMT  
		Size: 56.0 MB (56046468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5e2150967eeafa4e4e92254de9f529ea591d2d4b32ac6bf879b2cdb510222`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6b15dcdf4eda4c5061aefe4f754f90946717295e7fa5ea7dbaccff2b4f368f`  
		Last Modified: Fri, 21 Oct 2022 19:49:48 GMT  
		Size: 55.1 MB (55084220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21de4337b977fd518044876a04543776db696d6bc40559290e2dc785f3fa1cd2`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dab154f2aeb6b8b6a8282f9df9d12aea07b392a14b82d9f9d04003f9588863`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:5dae1c4fb603384ad5f68d3a792e5cc1095c23740785261740f00d0739e097b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155562941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7d53e5f7cab773dc36cea9ba5009d948dbffd06acceb29c4ffed2f75f4ad51f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:41:03 GMT
ADD file:2ccafa0c5b388d404f1100108ad9a9cb06c3e4ca4543c4b0f2aadfd9c4b97e45 in / 
# Fri, 21 Oct 2022 19:41:03 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 20:02:14 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 20:02:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 20:02:20 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 20:02:42 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 20:02:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 20:02:44 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 20:02:45 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:02:46 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 20:03:19 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 20:03:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 20:03:20 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:03:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 20:03:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 20:03:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 20:03:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 20:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 20:03:57 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 20:03:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ba2bcb842ee086f4d448ac74f4e172e2568d56d24e6efae9b402c0e37f418943`  
		Last Modified: Fri, 21 Oct 2022 19:42:50 GMT  
		Size: 39.4 MB (39408151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f573f3d8f30de658c99546dfd56922e80e9293938b142d28198865c4c4a9ac`  
		Last Modified: Fri, 21 Oct 2022 20:04:33 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4de9dcca6a477790d74ccaf1a44e93d82058c1abfe8acc7d9949cd166f40e03`  
		Last Modified: Fri, 21 Oct 2022 20:04:34 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3d1d1f0399c6049042613a98e9c464de870d057f8589f496ad644fca5baad8`  
		Last Modified: Fri, 21 Oct 2022 20:04:32 GMT  
		Size: 4.4 MB (4433279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283bc354d9b803601a6cfc1b2c93b8497c0eca55ca6c4180663c547784192ce9`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef2e77bf45616b4d382065d9adcf89ae082529714fb253e1672aed550a3d166`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d13a94caf14e2d057950a534f5c7bb6e3ea40449ac98341a77d3de764270b6`  
		Last Modified: Fri, 21 Oct 2022 20:04:37 GMT  
		Size: 55.4 MB (55421386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c1f1629008ad09afd71e6e8ac0337985cf8bb01382d50dfcbad35efa1789cb`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f892d0f3ede917e6800f61a5c88869e6897dd7a85dd6664d864f9a17b5757c64`  
		Last Modified: Fri, 21 Oct 2022 20:04:39 GMT  
		Size: 55.4 MB (55433315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346b88d5e2639641c57de86ca6641db6b00fdb7908b52bbfce8d5c2809b78039`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998f0dbf65c702dbec59a92b1a9238a7cdc44967a4d67908b9153a401781bf11`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:06314a7a220f6043436cfd72fd9c7f174fd58ef69fe4b788625fa53be4ab66aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:fe2a93f68a7ddef56a39cbc8b3faaf41ca6c910978255119941c1b71899aa6c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157264983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fad08b3c84be3e9164f86153224ab616bf71ee2c79677154c2e5cd3179cccfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:54 GMT
ADD file:66ffe38a497f15c1941fcc4c64fda875cf27856f2ade5128546c10590c5ca84a in / 
# Fri, 21 Oct 2022 19:20:54 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:46:11 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:46:11 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:46:14 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:46:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 19:46:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:46:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:47:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:47:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:47:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:47:43 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:47:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:47:44 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:47:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:47:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:47:45 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:47:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:50cbc88660a5576a306374b5ee70e3e8aeb602409e05ffa41cd4680769ae0574`  
		Last Modified: Fri, 21 Oct 2022 19:22:39 GMT  
		Size: 40.6 MB (40588747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ca853f7184003ce4a998ddf789288fb6bca33039a73cbd4ba03ba525f27bb7`  
		Last Modified: Fri, 21 Oct 2022 19:49:41 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a20476962308f364c624cd515a836f813023b7bff68e93ae6aeac715b0e8f21`  
		Last Modified: Fri, 21 Oct 2022 19:49:42 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3fea56f9fb03595109612dc70a638e205294bcdda1964e39dd3851ee949fff`  
		Last Modified: Fri, 21 Oct 2022 19:49:40 GMT  
		Size: 4.6 MB (4607033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b058249d3104921cd4d5c5885643a97a8be8f9a69124fc9beed35cf791a0813f`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5014a20163fa346756c80c1114d1ea993e9478cdfb6c08da61684a56b3e2af`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906aa7388ee2006b8f4362b5e9e068081be6bfc44a8f3b2bcddd6921cf7d54c7`  
		Last Modified: Fri, 21 Oct 2022 19:49:46 GMT  
		Size: 56.0 MB (56046468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5e2150967eeafa4e4e92254de9f529ea591d2d4b32ac6bf879b2cdb510222`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6b15dcdf4eda4c5061aefe4f754f90946717295e7fa5ea7dbaccff2b4f368f`  
		Last Modified: Fri, 21 Oct 2022 19:49:48 GMT  
		Size: 55.1 MB (55084220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21de4337b977fd518044876a04543776db696d6bc40559290e2dc785f3fa1cd2`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dab154f2aeb6b8b6a8282f9df9d12aea07b392a14b82d9f9d04003f9588863`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:5dae1c4fb603384ad5f68d3a792e5cc1095c23740785261740f00d0739e097b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155562941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7d53e5f7cab773dc36cea9ba5009d948dbffd06acceb29c4ffed2f75f4ad51f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:41:03 GMT
ADD file:2ccafa0c5b388d404f1100108ad9a9cb06c3e4ca4543c4b0f2aadfd9c4b97e45 in / 
# Fri, 21 Oct 2022 19:41:03 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 20:02:14 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 20:02:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 20:02:20 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 20:02:42 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 20:02:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 20:02:44 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 20:02:45 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:02:46 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 20:03:19 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 20:03:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 20:03:20 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:03:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 20:03:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 20:03:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 20:03:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 20:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 20:03:57 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 20:03:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ba2bcb842ee086f4d448ac74f4e172e2568d56d24e6efae9b402c0e37f418943`  
		Last Modified: Fri, 21 Oct 2022 19:42:50 GMT  
		Size: 39.4 MB (39408151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f573f3d8f30de658c99546dfd56922e80e9293938b142d28198865c4c4a9ac`  
		Last Modified: Fri, 21 Oct 2022 20:04:33 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4de9dcca6a477790d74ccaf1a44e93d82058c1abfe8acc7d9949cd166f40e03`  
		Last Modified: Fri, 21 Oct 2022 20:04:34 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3d1d1f0399c6049042613a98e9c464de870d057f8589f496ad644fca5baad8`  
		Last Modified: Fri, 21 Oct 2022 20:04:32 GMT  
		Size: 4.4 MB (4433279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283bc354d9b803601a6cfc1b2c93b8497c0eca55ca6c4180663c547784192ce9`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef2e77bf45616b4d382065d9adcf89ae082529714fb253e1672aed550a3d166`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d13a94caf14e2d057950a534f5c7bb6e3ea40449ac98341a77d3de764270b6`  
		Last Modified: Fri, 21 Oct 2022 20:04:37 GMT  
		Size: 55.4 MB (55421386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c1f1629008ad09afd71e6e8ac0337985cf8bb01382d50dfcbad35efa1789cb`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f892d0f3ede917e6800f61a5c88869e6897dd7a85dd6664d864f9a17b5757c64`  
		Last Modified: Fri, 21 Oct 2022 20:04:39 GMT  
		Size: 55.4 MB (55433315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346b88d5e2639641c57de86ca6641db6b00fdb7908b52bbfce8d5c2809b78039`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998f0dbf65c702dbec59a92b1a9238a7cdc44967a4d67908b9153a401781bf11`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:6da07a43b1ca31cb3e7e3d420de6a91682f0b8f4231888eafb11d86a3806d9e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:e6fb4c622766a92a7f2eda90f5208b863c206511504e77d805971f1944103212
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177571480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ffa4b21891e5a2ed6c1af823d9981d52d3a6d68dff7cc3d544760fb5815215`
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
# Wed, 19 Oct 2022 19:24:29 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:24:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Oct 2022 19:24:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:24:30 GMT
EXPOSE 3306 33060
# Wed, 19 Oct 2022 19:24:30 GMT
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
	-	`sha256:bd5bd9407260ce1a7ee0cd4090756c9dea74c7ff2e0f9f67707bcd3a0afedea5`  
		Last Modified: Wed, 19 Oct 2022 19:25:32 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5227be166f712520b21a76c9ed1e61648494703fa3c3b55d0d3fcaeabe32547f`  
		Last Modified: Wed, 19 Oct 2022 19:25:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:06314a7a220f6043436cfd72fd9c7f174fd58ef69fe4b788625fa53be4ab66aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:fe2a93f68a7ddef56a39cbc8b3faaf41ca6c910978255119941c1b71899aa6c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157264983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fad08b3c84be3e9164f86153224ab616bf71ee2c79677154c2e5cd3179cccfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:54 GMT
ADD file:66ffe38a497f15c1941fcc4c64fda875cf27856f2ade5128546c10590c5ca84a in / 
# Fri, 21 Oct 2022 19:20:54 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:46:11 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:46:11 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:46:14 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:46:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 19:46:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:46:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:47:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:47:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:47:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:47:43 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:47:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:47:44 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:47:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:47:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:47:45 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:47:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:50cbc88660a5576a306374b5ee70e3e8aeb602409e05ffa41cd4680769ae0574`  
		Last Modified: Fri, 21 Oct 2022 19:22:39 GMT  
		Size: 40.6 MB (40588747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ca853f7184003ce4a998ddf789288fb6bca33039a73cbd4ba03ba525f27bb7`  
		Last Modified: Fri, 21 Oct 2022 19:49:41 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a20476962308f364c624cd515a836f813023b7bff68e93ae6aeac715b0e8f21`  
		Last Modified: Fri, 21 Oct 2022 19:49:42 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3fea56f9fb03595109612dc70a638e205294bcdda1964e39dd3851ee949fff`  
		Last Modified: Fri, 21 Oct 2022 19:49:40 GMT  
		Size: 4.6 MB (4607033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b058249d3104921cd4d5c5885643a97a8be8f9a69124fc9beed35cf791a0813f`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5014a20163fa346756c80c1114d1ea993e9478cdfb6c08da61684a56b3e2af`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906aa7388ee2006b8f4362b5e9e068081be6bfc44a8f3b2bcddd6921cf7d54c7`  
		Last Modified: Fri, 21 Oct 2022 19:49:46 GMT  
		Size: 56.0 MB (56046468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5e2150967eeafa4e4e92254de9f529ea591d2d4b32ac6bf879b2cdb510222`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6b15dcdf4eda4c5061aefe4f754f90946717295e7fa5ea7dbaccff2b4f368f`  
		Last Modified: Fri, 21 Oct 2022 19:49:48 GMT  
		Size: 55.1 MB (55084220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21de4337b977fd518044876a04543776db696d6bc40559290e2dc785f3fa1cd2`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dab154f2aeb6b8b6a8282f9df9d12aea07b392a14b82d9f9d04003f9588863`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:5dae1c4fb603384ad5f68d3a792e5cc1095c23740785261740f00d0739e097b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155562941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7d53e5f7cab773dc36cea9ba5009d948dbffd06acceb29c4ffed2f75f4ad51f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:41:03 GMT
ADD file:2ccafa0c5b388d404f1100108ad9a9cb06c3e4ca4543c4b0f2aadfd9c4b97e45 in / 
# Fri, 21 Oct 2022 19:41:03 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 20:02:14 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 20:02:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 20:02:20 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 20:02:42 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 20:02:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 20:02:44 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 20:02:45 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:02:46 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 20:03:19 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 20:03:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 20:03:20 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:03:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 20:03:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 20:03:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 20:03:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 20:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 20:03:57 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 20:03:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ba2bcb842ee086f4d448ac74f4e172e2568d56d24e6efae9b402c0e37f418943`  
		Last Modified: Fri, 21 Oct 2022 19:42:50 GMT  
		Size: 39.4 MB (39408151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f573f3d8f30de658c99546dfd56922e80e9293938b142d28198865c4c4a9ac`  
		Last Modified: Fri, 21 Oct 2022 20:04:33 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4de9dcca6a477790d74ccaf1a44e93d82058c1abfe8acc7d9949cd166f40e03`  
		Last Modified: Fri, 21 Oct 2022 20:04:34 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3d1d1f0399c6049042613a98e9c464de870d057f8589f496ad644fca5baad8`  
		Last Modified: Fri, 21 Oct 2022 20:04:32 GMT  
		Size: 4.4 MB (4433279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283bc354d9b803601a6cfc1b2c93b8497c0eca55ca6c4180663c547784192ce9`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef2e77bf45616b4d382065d9adcf89ae082529714fb253e1672aed550a3d166`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d13a94caf14e2d057950a534f5c7bb6e3ea40449ac98341a77d3de764270b6`  
		Last Modified: Fri, 21 Oct 2022 20:04:37 GMT  
		Size: 55.4 MB (55421386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c1f1629008ad09afd71e6e8ac0337985cf8bb01382d50dfcbad35efa1789cb`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f892d0f3ede917e6800f61a5c88869e6897dd7a85dd6664d864f9a17b5757c64`  
		Last Modified: Fri, 21 Oct 2022 20:04:39 GMT  
		Size: 55.4 MB (55433315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346b88d5e2639641c57de86ca6641db6b00fdb7908b52bbfce8d5c2809b78039`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998f0dbf65c702dbec59a92b1a9238a7cdc44967a4d67908b9153a401781bf11`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31`

```console
$ docker pull mysql@sha256:06314a7a220f6043436cfd72fd9c7f174fd58ef69fe4b788625fa53be4ab66aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.31` - linux; amd64

```console
$ docker pull mysql@sha256:fe2a93f68a7ddef56a39cbc8b3faaf41ca6c910978255119941c1b71899aa6c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157264983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fad08b3c84be3e9164f86153224ab616bf71ee2c79677154c2e5cd3179cccfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:54 GMT
ADD file:66ffe38a497f15c1941fcc4c64fda875cf27856f2ade5128546c10590c5ca84a in / 
# Fri, 21 Oct 2022 19:20:54 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:46:11 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:46:11 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:46:14 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:46:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 19:46:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:46:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:47:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:47:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:47:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:47:43 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:47:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:47:44 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:47:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:47:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:47:45 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:47:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:50cbc88660a5576a306374b5ee70e3e8aeb602409e05ffa41cd4680769ae0574`  
		Last Modified: Fri, 21 Oct 2022 19:22:39 GMT  
		Size: 40.6 MB (40588747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ca853f7184003ce4a998ddf789288fb6bca33039a73cbd4ba03ba525f27bb7`  
		Last Modified: Fri, 21 Oct 2022 19:49:41 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a20476962308f364c624cd515a836f813023b7bff68e93ae6aeac715b0e8f21`  
		Last Modified: Fri, 21 Oct 2022 19:49:42 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3fea56f9fb03595109612dc70a638e205294bcdda1964e39dd3851ee949fff`  
		Last Modified: Fri, 21 Oct 2022 19:49:40 GMT  
		Size: 4.6 MB (4607033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b058249d3104921cd4d5c5885643a97a8be8f9a69124fc9beed35cf791a0813f`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5014a20163fa346756c80c1114d1ea993e9478cdfb6c08da61684a56b3e2af`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906aa7388ee2006b8f4362b5e9e068081be6bfc44a8f3b2bcddd6921cf7d54c7`  
		Last Modified: Fri, 21 Oct 2022 19:49:46 GMT  
		Size: 56.0 MB (56046468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5e2150967eeafa4e4e92254de9f529ea591d2d4b32ac6bf879b2cdb510222`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6b15dcdf4eda4c5061aefe4f754f90946717295e7fa5ea7dbaccff2b4f368f`  
		Last Modified: Fri, 21 Oct 2022 19:49:48 GMT  
		Size: 55.1 MB (55084220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21de4337b977fd518044876a04543776db696d6bc40559290e2dc785f3fa1cd2`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dab154f2aeb6b8b6a8282f9df9d12aea07b392a14b82d9f9d04003f9588863`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.31` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:5dae1c4fb603384ad5f68d3a792e5cc1095c23740785261740f00d0739e097b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155562941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7d53e5f7cab773dc36cea9ba5009d948dbffd06acceb29c4ffed2f75f4ad51f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:41:03 GMT
ADD file:2ccafa0c5b388d404f1100108ad9a9cb06c3e4ca4543c4b0f2aadfd9c4b97e45 in / 
# Fri, 21 Oct 2022 19:41:03 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 20:02:14 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 20:02:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 20:02:20 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 20:02:42 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 20:02:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 20:02:44 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 20:02:45 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:02:46 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 20:03:19 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 20:03:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 20:03:20 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:03:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 20:03:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 20:03:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 20:03:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 20:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 20:03:57 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 20:03:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ba2bcb842ee086f4d448ac74f4e172e2568d56d24e6efae9b402c0e37f418943`  
		Last Modified: Fri, 21 Oct 2022 19:42:50 GMT  
		Size: 39.4 MB (39408151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f573f3d8f30de658c99546dfd56922e80e9293938b142d28198865c4c4a9ac`  
		Last Modified: Fri, 21 Oct 2022 20:04:33 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4de9dcca6a477790d74ccaf1a44e93d82058c1abfe8acc7d9949cd166f40e03`  
		Last Modified: Fri, 21 Oct 2022 20:04:34 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3d1d1f0399c6049042613a98e9c464de870d057f8589f496ad644fca5baad8`  
		Last Modified: Fri, 21 Oct 2022 20:04:32 GMT  
		Size: 4.4 MB (4433279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283bc354d9b803601a6cfc1b2c93b8497c0eca55ca6c4180663c547784192ce9`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef2e77bf45616b4d382065d9adcf89ae082529714fb253e1672aed550a3d166`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d13a94caf14e2d057950a534f5c7bb6e3ea40449ac98341a77d3de764270b6`  
		Last Modified: Fri, 21 Oct 2022 20:04:37 GMT  
		Size: 55.4 MB (55421386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c1f1629008ad09afd71e6e8ac0337985cf8bb01382d50dfcbad35efa1789cb`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f892d0f3ede917e6800f61a5c88869e6897dd7a85dd6664d864f9a17b5757c64`  
		Last Modified: Fri, 21 Oct 2022 20:04:39 GMT  
		Size: 55.4 MB (55433315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346b88d5e2639641c57de86ca6641db6b00fdb7908b52bbfce8d5c2809b78039`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998f0dbf65c702dbec59a92b1a9238a7cdc44967a4d67908b9153a401781bf11`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31-debian`

```console
$ docker pull mysql@sha256:6da07a43b1ca31cb3e7e3d420de6a91682f0b8f4231888eafb11d86a3806d9e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.31-debian` - linux; amd64

```console
$ docker pull mysql@sha256:e6fb4c622766a92a7f2eda90f5208b863c206511504e77d805971f1944103212
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177571480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ffa4b21891e5a2ed6c1af823d9981d52d3a6d68dff7cc3d544760fb5815215`
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
# Wed, 19 Oct 2022 19:24:29 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:24:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Oct 2022 19:24:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:24:30 GMT
EXPOSE 3306 33060
# Wed, 19 Oct 2022 19:24:30 GMT
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
	-	`sha256:bd5bd9407260ce1a7ee0cd4090756c9dea74c7ff2e0f9f67707bcd3a0afedea5`  
		Last Modified: Wed, 19 Oct 2022 19:25:32 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5227be166f712520b21a76c9ed1e61648494703fa3c3b55d0d3fcaeabe32547f`  
		Last Modified: Wed, 19 Oct 2022 19:25:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31-oracle`

```console
$ docker pull mysql@sha256:06314a7a220f6043436cfd72fd9c7f174fd58ef69fe4b788625fa53be4ab66aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.31-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:fe2a93f68a7ddef56a39cbc8b3faaf41ca6c910978255119941c1b71899aa6c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157264983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fad08b3c84be3e9164f86153224ab616bf71ee2c79677154c2e5cd3179cccfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:54 GMT
ADD file:66ffe38a497f15c1941fcc4c64fda875cf27856f2ade5128546c10590c5ca84a in / 
# Fri, 21 Oct 2022 19:20:54 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:46:11 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:46:11 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:46:14 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:46:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 19:46:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:46:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:47:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:47:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:47:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:47:43 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:47:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:47:44 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:47:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:47:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:47:45 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:47:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:50cbc88660a5576a306374b5ee70e3e8aeb602409e05ffa41cd4680769ae0574`  
		Last Modified: Fri, 21 Oct 2022 19:22:39 GMT  
		Size: 40.6 MB (40588747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ca853f7184003ce4a998ddf789288fb6bca33039a73cbd4ba03ba525f27bb7`  
		Last Modified: Fri, 21 Oct 2022 19:49:41 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a20476962308f364c624cd515a836f813023b7bff68e93ae6aeac715b0e8f21`  
		Last Modified: Fri, 21 Oct 2022 19:49:42 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3fea56f9fb03595109612dc70a638e205294bcdda1964e39dd3851ee949fff`  
		Last Modified: Fri, 21 Oct 2022 19:49:40 GMT  
		Size: 4.6 MB (4607033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b058249d3104921cd4d5c5885643a97a8be8f9a69124fc9beed35cf791a0813f`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5014a20163fa346756c80c1114d1ea993e9478cdfb6c08da61684a56b3e2af`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906aa7388ee2006b8f4362b5e9e068081be6bfc44a8f3b2bcddd6921cf7d54c7`  
		Last Modified: Fri, 21 Oct 2022 19:49:46 GMT  
		Size: 56.0 MB (56046468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5e2150967eeafa4e4e92254de9f529ea591d2d4b32ac6bf879b2cdb510222`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6b15dcdf4eda4c5061aefe4f754f90946717295e7fa5ea7dbaccff2b4f368f`  
		Last Modified: Fri, 21 Oct 2022 19:49:48 GMT  
		Size: 55.1 MB (55084220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21de4337b977fd518044876a04543776db696d6bc40559290e2dc785f3fa1cd2`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dab154f2aeb6b8b6a8282f9df9d12aea07b392a14b82d9f9d04003f9588863`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.31-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:5dae1c4fb603384ad5f68d3a792e5cc1095c23740785261740f00d0739e097b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155562941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7d53e5f7cab773dc36cea9ba5009d948dbffd06acceb29c4ffed2f75f4ad51f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:41:03 GMT
ADD file:2ccafa0c5b388d404f1100108ad9a9cb06c3e4ca4543c4b0f2aadfd9c4b97e45 in / 
# Fri, 21 Oct 2022 19:41:03 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 20:02:14 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 20:02:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 20:02:20 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 20:02:42 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 20:02:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 20:02:44 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 20:02:45 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:02:46 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 20:03:19 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 20:03:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 20:03:20 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:03:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 20:03:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 20:03:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 20:03:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 20:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 20:03:57 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 20:03:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ba2bcb842ee086f4d448ac74f4e172e2568d56d24e6efae9b402c0e37f418943`  
		Last Modified: Fri, 21 Oct 2022 19:42:50 GMT  
		Size: 39.4 MB (39408151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f573f3d8f30de658c99546dfd56922e80e9293938b142d28198865c4c4a9ac`  
		Last Modified: Fri, 21 Oct 2022 20:04:33 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4de9dcca6a477790d74ccaf1a44e93d82058c1abfe8acc7d9949cd166f40e03`  
		Last Modified: Fri, 21 Oct 2022 20:04:34 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3d1d1f0399c6049042613a98e9c464de870d057f8589f496ad644fca5baad8`  
		Last Modified: Fri, 21 Oct 2022 20:04:32 GMT  
		Size: 4.4 MB (4433279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283bc354d9b803601a6cfc1b2c93b8497c0eca55ca6c4180663c547784192ce9`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef2e77bf45616b4d382065d9adcf89ae082529714fb253e1672aed550a3d166`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d13a94caf14e2d057950a534f5c7bb6e3ea40449ac98341a77d3de764270b6`  
		Last Modified: Fri, 21 Oct 2022 20:04:37 GMT  
		Size: 55.4 MB (55421386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c1f1629008ad09afd71e6e8ac0337985cf8bb01382d50dfcbad35efa1789cb`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f892d0f3ede917e6800f61a5c88869e6897dd7a85dd6664d864f9a17b5757c64`  
		Last Modified: Fri, 21 Oct 2022 20:04:39 GMT  
		Size: 55.4 MB (55433315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346b88d5e2639641c57de86ca6641db6b00fdb7908b52bbfce8d5c2809b78039`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998f0dbf65c702dbec59a92b1a9238a7cdc44967a4d67908b9153a401781bf11`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:6da07a43b1ca31cb3e7e3d420de6a91682f0b8f4231888eafb11d86a3806d9e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:e6fb4c622766a92a7f2eda90f5208b863c206511504e77d805971f1944103212
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177571480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ffa4b21891e5a2ed6c1af823d9981d52d3a6d68dff7cc3d544760fb5815215`
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
# Wed, 19 Oct 2022 19:24:29 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:24:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Oct 2022 19:24:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:24:30 GMT
EXPOSE 3306 33060
# Wed, 19 Oct 2022 19:24:30 GMT
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
	-	`sha256:bd5bd9407260ce1a7ee0cd4090756c9dea74c7ff2e0f9f67707bcd3a0afedea5`  
		Last Modified: Wed, 19 Oct 2022 19:25:32 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5227be166f712520b21a76c9ed1e61648494703fa3c3b55d0d3fcaeabe32547f`  
		Last Modified: Wed, 19 Oct 2022 19:25:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:06314a7a220f6043436cfd72fd9c7f174fd58ef69fe4b788625fa53be4ab66aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:fe2a93f68a7ddef56a39cbc8b3faaf41ca6c910978255119941c1b71899aa6c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157264983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fad08b3c84be3e9164f86153224ab616bf71ee2c79677154c2e5cd3179cccfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:54 GMT
ADD file:66ffe38a497f15c1941fcc4c64fda875cf27856f2ade5128546c10590c5ca84a in / 
# Fri, 21 Oct 2022 19:20:54 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:46:11 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:46:11 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:46:14 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:46:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 19:46:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:46:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:47:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:47:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:47:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:47:43 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:47:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:47:44 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:47:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:47:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:47:45 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:47:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:50cbc88660a5576a306374b5ee70e3e8aeb602409e05ffa41cd4680769ae0574`  
		Last Modified: Fri, 21 Oct 2022 19:22:39 GMT  
		Size: 40.6 MB (40588747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ca853f7184003ce4a998ddf789288fb6bca33039a73cbd4ba03ba525f27bb7`  
		Last Modified: Fri, 21 Oct 2022 19:49:41 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a20476962308f364c624cd515a836f813023b7bff68e93ae6aeac715b0e8f21`  
		Last Modified: Fri, 21 Oct 2022 19:49:42 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3fea56f9fb03595109612dc70a638e205294bcdda1964e39dd3851ee949fff`  
		Last Modified: Fri, 21 Oct 2022 19:49:40 GMT  
		Size: 4.6 MB (4607033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b058249d3104921cd4d5c5885643a97a8be8f9a69124fc9beed35cf791a0813f`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5014a20163fa346756c80c1114d1ea993e9478cdfb6c08da61684a56b3e2af`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906aa7388ee2006b8f4362b5e9e068081be6bfc44a8f3b2bcddd6921cf7d54c7`  
		Last Modified: Fri, 21 Oct 2022 19:49:46 GMT  
		Size: 56.0 MB (56046468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5e2150967eeafa4e4e92254de9f529ea591d2d4b32ac6bf879b2cdb510222`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6b15dcdf4eda4c5061aefe4f754f90946717295e7fa5ea7dbaccff2b4f368f`  
		Last Modified: Fri, 21 Oct 2022 19:49:48 GMT  
		Size: 55.1 MB (55084220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21de4337b977fd518044876a04543776db696d6bc40559290e2dc785f3fa1cd2`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dab154f2aeb6b8b6a8282f9df9d12aea07b392a14b82d9f9d04003f9588863`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:5dae1c4fb603384ad5f68d3a792e5cc1095c23740785261740f00d0739e097b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155562941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7d53e5f7cab773dc36cea9ba5009d948dbffd06acceb29c4ffed2f75f4ad51f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:41:03 GMT
ADD file:2ccafa0c5b388d404f1100108ad9a9cb06c3e4ca4543c4b0f2aadfd9c4b97e45 in / 
# Fri, 21 Oct 2022 19:41:03 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 20:02:14 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 20:02:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 20:02:20 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 20:02:42 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 20:02:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 20:02:44 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 20:02:45 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:02:46 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 20:03:19 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 20:03:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 20:03:20 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:03:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 20:03:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 20:03:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 20:03:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 20:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 20:03:57 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 20:03:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ba2bcb842ee086f4d448ac74f4e172e2568d56d24e6efae9b402c0e37f418943`  
		Last Modified: Fri, 21 Oct 2022 19:42:50 GMT  
		Size: 39.4 MB (39408151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f573f3d8f30de658c99546dfd56922e80e9293938b142d28198865c4c4a9ac`  
		Last Modified: Fri, 21 Oct 2022 20:04:33 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4de9dcca6a477790d74ccaf1a44e93d82058c1abfe8acc7d9949cd166f40e03`  
		Last Modified: Fri, 21 Oct 2022 20:04:34 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3d1d1f0399c6049042613a98e9c464de870d057f8589f496ad644fca5baad8`  
		Last Modified: Fri, 21 Oct 2022 20:04:32 GMT  
		Size: 4.4 MB (4433279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283bc354d9b803601a6cfc1b2c93b8497c0eca55ca6c4180663c547784192ce9`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef2e77bf45616b4d382065d9adcf89ae082529714fb253e1672aed550a3d166`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d13a94caf14e2d057950a534f5c7bb6e3ea40449ac98341a77d3de764270b6`  
		Last Modified: Fri, 21 Oct 2022 20:04:37 GMT  
		Size: 55.4 MB (55421386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c1f1629008ad09afd71e6e8ac0337985cf8bb01382d50dfcbad35efa1789cb`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f892d0f3ede917e6800f61a5c88869e6897dd7a85dd6664d864f9a17b5757c64`  
		Last Modified: Fri, 21 Oct 2022 20:04:39 GMT  
		Size: 55.4 MB (55433315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346b88d5e2639641c57de86ca6641db6b00fdb7908b52bbfce8d5c2809b78039`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998f0dbf65c702dbec59a92b1a9238a7cdc44967a4d67908b9153a401781bf11`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:06314a7a220f6043436cfd72fd9c7f174fd58ef69fe4b788625fa53be4ab66aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:fe2a93f68a7ddef56a39cbc8b3faaf41ca6c910978255119941c1b71899aa6c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157264983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fad08b3c84be3e9164f86153224ab616bf71ee2c79677154c2e5cd3179cccfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:54 GMT
ADD file:66ffe38a497f15c1941fcc4c64fda875cf27856f2ade5128546c10590c5ca84a in / 
# Fri, 21 Oct 2022 19:20:54 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:46:11 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:46:11 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:46:14 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:46:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 19:46:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:46:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:47:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:47:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:47:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:47:43 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:47:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:47:44 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:47:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:47:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:47:45 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:47:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:50cbc88660a5576a306374b5ee70e3e8aeb602409e05ffa41cd4680769ae0574`  
		Last Modified: Fri, 21 Oct 2022 19:22:39 GMT  
		Size: 40.6 MB (40588747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ca853f7184003ce4a998ddf789288fb6bca33039a73cbd4ba03ba525f27bb7`  
		Last Modified: Fri, 21 Oct 2022 19:49:41 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a20476962308f364c624cd515a836f813023b7bff68e93ae6aeac715b0e8f21`  
		Last Modified: Fri, 21 Oct 2022 19:49:42 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3fea56f9fb03595109612dc70a638e205294bcdda1964e39dd3851ee949fff`  
		Last Modified: Fri, 21 Oct 2022 19:49:40 GMT  
		Size: 4.6 MB (4607033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b058249d3104921cd4d5c5885643a97a8be8f9a69124fc9beed35cf791a0813f`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5014a20163fa346756c80c1114d1ea993e9478cdfb6c08da61684a56b3e2af`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906aa7388ee2006b8f4362b5e9e068081be6bfc44a8f3b2bcddd6921cf7d54c7`  
		Last Modified: Fri, 21 Oct 2022 19:49:46 GMT  
		Size: 56.0 MB (56046468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5e2150967eeafa4e4e92254de9f529ea591d2d4b32ac6bf879b2cdb510222`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6b15dcdf4eda4c5061aefe4f754f90946717295e7fa5ea7dbaccff2b4f368f`  
		Last Modified: Fri, 21 Oct 2022 19:49:48 GMT  
		Size: 55.1 MB (55084220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21de4337b977fd518044876a04543776db696d6bc40559290e2dc785f3fa1cd2`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dab154f2aeb6b8b6a8282f9df9d12aea07b392a14b82d9f9d04003f9588863`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:5dae1c4fb603384ad5f68d3a792e5cc1095c23740785261740f00d0739e097b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155562941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7d53e5f7cab773dc36cea9ba5009d948dbffd06acceb29c4ffed2f75f4ad51f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:41:03 GMT
ADD file:2ccafa0c5b388d404f1100108ad9a9cb06c3e4ca4543c4b0f2aadfd9c4b97e45 in / 
# Fri, 21 Oct 2022 19:41:03 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 20:02:14 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 20:02:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 20:02:20 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 20:02:42 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 20:02:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 20:02:44 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 20:02:45 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:02:46 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 20:03:19 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 20:03:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 20:03:20 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:03:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 20:03:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 20:03:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 20:03:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 20:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 20:03:57 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 20:03:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ba2bcb842ee086f4d448ac74f4e172e2568d56d24e6efae9b402c0e37f418943`  
		Last Modified: Fri, 21 Oct 2022 19:42:50 GMT  
		Size: 39.4 MB (39408151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f573f3d8f30de658c99546dfd56922e80e9293938b142d28198865c4c4a9ac`  
		Last Modified: Fri, 21 Oct 2022 20:04:33 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4de9dcca6a477790d74ccaf1a44e93d82058c1abfe8acc7d9949cd166f40e03`  
		Last Modified: Fri, 21 Oct 2022 20:04:34 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3d1d1f0399c6049042613a98e9c464de870d057f8589f496ad644fca5baad8`  
		Last Modified: Fri, 21 Oct 2022 20:04:32 GMT  
		Size: 4.4 MB (4433279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283bc354d9b803601a6cfc1b2c93b8497c0eca55ca6c4180663c547784192ce9`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef2e77bf45616b4d382065d9adcf89ae082529714fb253e1672aed550a3d166`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d13a94caf14e2d057950a534f5c7bb6e3ea40449ac98341a77d3de764270b6`  
		Last Modified: Fri, 21 Oct 2022 20:04:37 GMT  
		Size: 55.4 MB (55421386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c1f1629008ad09afd71e6e8ac0337985cf8bb01382d50dfcbad35efa1789cb`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f892d0f3ede917e6800f61a5c88869e6897dd7a85dd6664d864f9a17b5757c64`  
		Last Modified: Fri, 21 Oct 2022 20:04:39 GMT  
		Size: 55.4 MB (55433315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346b88d5e2639641c57de86ca6641db6b00fdb7908b52bbfce8d5c2809b78039`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998f0dbf65c702dbec59a92b1a9238a7cdc44967a4d67908b9153a401781bf11`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
