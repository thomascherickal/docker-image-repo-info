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
$ docker pull mysql@sha256:7fe02bf3592e9ec218e17f0bf39bd3fc7a118c6426e63bea849ef358b798c74b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:d8aa78a2e64fe5d55050c9eb82a056edda57cb5bd9978c8abd93a2cc5a0c1282
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129921235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec14ca3fec4d86d989ea6ac3f66af44da0298438e1082b0f1682dba5c912fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:36 GMT
ADD file:eefc8abcbb6ec3141573da12cc99f3d9592d5a0bd105bb189e0e1db15c0d1bf5 in / 
# Fri, 27 Jan 2023 23:36:37 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:06:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:06:33 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:06:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:06:55 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sat, 28 Jan 2023 00:06:56 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:06:56 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 28 Jan 2023 00:06:56 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Sat, 28 Jan 2023 00:06:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:07:14 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:07:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:07:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Sat, 28 Jan 2023 00:07:39 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:07:40 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:07:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:07:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:07:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:07:41 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:07:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e048d0a387420acfdb05a1ec44ed79aa01be81adcd731b3100359277ca89d08b`  
		Last Modified: Fri, 27 Jan 2023 23:38:26 GMT  
		Size: 50.5 MB (50466577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7847c8a41cb8230f06f790ec1f0ed987fa4b9fea784840951ddc7adda2efe08`  
		Last Modified: Sat, 28 Jan 2023 00:08:54 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c400748dd907cc0ad8565e047359c9c7164407c0ee46463b7e03928b2ba72a70`  
		Last Modified: Sat, 28 Jan 2023 00:08:54 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59c21f62b1f96c3c2adb9e74f8dd2739f1a720d964c5e28110f8a192309323d`  
		Last Modified: Sat, 28 Jan 2023 00:08:53 GMT  
		Size: 4.5 MB (4542101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426e724ab5eb21fa69a123fee2d03329e1c9e9638256006bbc0d4b85ad5ec6c9`  
		Last Modified: Sat, 28 Jan 2023 00:08:52 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc537924e52d943105cc6a151c17b2492abf07558c700823ee579e0b697726b6`  
		Last Modified: Sat, 28 Jan 2023 00:08:52 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa4edfb8fd8f8db7918a3efa8428c072e80a26c726b804998177f0aec27f07f`  
		Last Modified: Sat, 28 Jan 2023 00:08:55 GMT  
		Size: 25.5 MB (25525248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce197f17dcb5ff1f3fc239d57ba39190ccc18d6324364afe512f8061f11cfb`  
		Last Modified: Sat, 28 Jan 2023 00:08:51 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e7bdd9aebc9c3f60792159ce76da2df9a453977d112739f605357c6d01aa53`  
		Last Modified: Sat, 28 Jan 2023 00:09:00 GMT  
		Size: 48.4 MB (48447391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de2e85fdede9323464c34c692606810abfe152d22f8007e05e3419f662a8f5`  
		Last Modified: Sat, 28 Jan 2023 00:08:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006f2ea3576a5de92edb14f65f32d4ba885bc0cb594359eebc32d4cb45a0c5fc`  
		Last Modified: Sat, 28 Jan 2023 00:08:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:6f4fb1b8c2717cbe709e755f83a3d6f52dabe58902569bdaa14d0cc9d4c18d25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:603b9b890043bd774c673060292c818e771135c51d0d2b8b7873151906610220
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162644100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4726a7600c6f5c8b58d26e8a5634a13bdff727ee29eebe5edbf9ebdd00533898`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 Jan 2023 02:35:07 GMT
ADD file:67ceb946e54c26c505b5f9f393d77befbd5e9b3b5c069ca301e314ecc74456b0 in / 
# Wed, 11 Jan 2023 02:35:07 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 06:20:12 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 Jan 2023 06:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:20:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 Jan 2023 06:20:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 Jan 2023 06:20:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 Jan 2023 06:20:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:20:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 Jan 2023 06:20:36 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 17 Jan 2023 21:08:53 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Tue, 17 Jan 2023 21:08:54 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 17 Jan 2023 21:09:16 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 17 Jan 2023 21:09:17 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 Jan 2023 21:09:17 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 17 Jan 2023 21:09:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Jan 2023 21:09:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Jan 2023 21:09:18 GMT
EXPOSE 3306 33060
# Tue, 17 Jan 2023 21:09:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:548fcab5fe888f589dd092c68b813bfd65359878bd1950d6b753f749e82ebd7c`  
		Last Modified: Wed, 11 Jan 2023 02:39:48 GMT  
		Size: 27.1 MB (27140352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702e45a0d0fab46740d0cf404969001dc0537dd564973fa6f31da2a00cfe5ef8`  
		Last Modified: Wed, 11 Jan 2023 06:22:03 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad96d17a23a7cff619709675f8981274e6a4ff7a9fb99590f0a837511e69a50b`  
		Last Modified: Wed, 11 Jan 2023 06:22:03 GMT  
		Size: 4.2 MB (4182274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1832d5509d3dce5314c5ffb58ac35ef7e35c396457e6fab747267312751708cf`  
		Last Modified: Wed, 11 Jan 2023 06:22:02 GMT  
		Size: 1.4 MB (1388883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5a580bc4aa47839f3f325b0a7bd7f927d8f41bb947a8e6d1847048a16c88dc`  
		Last Modified: Wed, 11 Jan 2023 06:22:01 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562f0a131c6cc56e3a6b85245641c4251cb4bc5e5b97f08d5d97209b8c11c38c`  
		Last Modified: Wed, 11 Jan 2023 06:22:04 GMT  
		Size: 14.1 MB (14089400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5760997e25e0fd516f2aab1a32be22ae0a919faa2c2dd36a3ad098d772ca3495`  
		Last Modified: Wed, 11 Jan 2023 06:22:00 GMT  
		Size: 2.5 KB (2543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2459447ebb40538b162dbc50dd435551e3c63d290fc1fb37555ee724a56989a9`  
		Last Modified: Tue, 17 Jan 2023 21:11:22 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b7ab69b071a7139fbe466170a22caead38334834a792630c6a0e9b12f15ef6`  
		Last Modified: Tue, 17 Jan 2023 21:11:37 GMT  
		Size: 115.8 MB (115832999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aad2d01a4e6a079bc797ac021db4938622225182fa24eab797ee661d30134e9`  
		Last Modified: Tue, 17 Jan 2023 21:11:22 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d70cf470197d6c4c9c3f0789a15440b5439ac8536ea8db923608b24b7dfc59`  
		Last Modified: Tue, 17 Jan 2023 21:11:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:7fe02bf3592e9ec218e17f0bf39bd3fc7a118c6426e63bea849ef358b798c74b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:d8aa78a2e64fe5d55050c9eb82a056edda57cb5bd9978c8abd93a2cc5a0c1282
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129921235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec14ca3fec4d86d989ea6ac3f66af44da0298438e1082b0f1682dba5c912fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:36 GMT
ADD file:eefc8abcbb6ec3141573da12cc99f3d9592d5a0bd105bb189e0e1db15c0d1bf5 in / 
# Fri, 27 Jan 2023 23:36:37 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:06:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:06:33 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:06:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:06:55 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sat, 28 Jan 2023 00:06:56 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:06:56 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 28 Jan 2023 00:06:56 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Sat, 28 Jan 2023 00:06:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:07:14 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:07:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:07:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Sat, 28 Jan 2023 00:07:39 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:07:40 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:07:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:07:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:07:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:07:41 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:07:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e048d0a387420acfdb05a1ec44ed79aa01be81adcd731b3100359277ca89d08b`  
		Last Modified: Fri, 27 Jan 2023 23:38:26 GMT  
		Size: 50.5 MB (50466577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7847c8a41cb8230f06f790ec1f0ed987fa4b9fea784840951ddc7adda2efe08`  
		Last Modified: Sat, 28 Jan 2023 00:08:54 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c400748dd907cc0ad8565e047359c9c7164407c0ee46463b7e03928b2ba72a70`  
		Last Modified: Sat, 28 Jan 2023 00:08:54 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59c21f62b1f96c3c2adb9e74f8dd2739f1a720d964c5e28110f8a192309323d`  
		Last Modified: Sat, 28 Jan 2023 00:08:53 GMT  
		Size: 4.5 MB (4542101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426e724ab5eb21fa69a123fee2d03329e1c9e9638256006bbc0d4b85ad5ec6c9`  
		Last Modified: Sat, 28 Jan 2023 00:08:52 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc537924e52d943105cc6a151c17b2492abf07558c700823ee579e0b697726b6`  
		Last Modified: Sat, 28 Jan 2023 00:08:52 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa4edfb8fd8f8db7918a3efa8428c072e80a26c726b804998177f0aec27f07f`  
		Last Modified: Sat, 28 Jan 2023 00:08:55 GMT  
		Size: 25.5 MB (25525248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce197f17dcb5ff1f3fc239d57ba39190ccc18d6324364afe512f8061f11cfb`  
		Last Modified: Sat, 28 Jan 2023 00:08:51 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e7bdd9aebc9c3f60792159ce76da2df9a453977d112739f605357c6d01aa53`  
		Last Modified: Sat, 28 Jan 2023 00:09:00 GMT  
		Size: 48.4 MB (48447391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de2e85fdede9323464c34c692606810abfe152d22f8007e05e3419f662a8f5`  
		Last Modified: Sat, 28 Jan 2023 00:08:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006f2ea3576a5de92edb14f65f32d4ba885bc0cb594359eebc32d4cb45a0c5fc`  
		Last Modified: Sat, 28 Jan 2023 00:08:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:7fe02bf3592e9ec218e17f0bf39bd3fc7a118c6426e63bea849ef358b798c74b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:d8aa78a2e64fe5d55050c9eb82a056edda57cb5bd9978c8abd93a2cc5a0c1282
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129921235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec14ca3fec4d86d989ea6ac3f66af44da0298438e1082b0f1682dba5c912fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:36 GMT
ADD file:eefc8abcbb6ec3141573da12cc99f3d9592d5a0bd105bb189e0e1db15c0d1bf5 in / 
# Fri, 27 Jan 2023 23:36:37 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:06:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:06:33 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:06:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:06:55 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sat, 28 Jan 2023 00:06:56 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:06:56 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 28 Jan 2023 00:06:56 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Sat, 28 Jan 2023 00:06:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:07:14 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:07:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:07:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Sat, 28 Jan 2023 00:07:39 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:07:40 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:07:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:07:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:07:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:07:41 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:07:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e048d0a387420acfdb05a1ec44ed79aa01be81adcd731b3100359277ca89d08b`  
		Last Modified: Fri, 27 Jan 2023 23:38:26 GMT  
		Size: 50.5 MB (50466577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7847c8a41cb8230f06f790ec1f0ed987fa4b9fea784840951ddc7adda2efe08`  
		Last Modified: Sat, 28 Jan 2023 00:08:54 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c400748dd907cc0ad8565e047359c9c7164407c0ee46463b7e03928b2ba72a70`  
		Last Modified: Sat, 28 Jan 2023 00:08:54 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59c21f62b1f96c3c2adb9e74f8dd2739f1a720d964c5e28110f8a192309323d`  
		Last Modified: Sat, 28 Jan 2023 00:08:53 GMT  
		Size: 4.5 MB (4542101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426e724ab5eb21fa69a123fee2d03329e1c9e9638256006bbc0d4b85ad5ec6c9`  
		Last Modified: Sat, 28 Jan 2023 00:08:52 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc537924e52d943105cc6a151c17b2492abf07558c700823ee579e0b697726b6`  
		Last Modified: Sat, 28 Jan 2023 00:08:52 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa4edfb8fd8f8db7918a3efa8428c072e80a26c726b804998177f0aec27f07f`  
		Last Modified: Sat, 28 Jan 2023 00:08:55 GMT  
		Size: 25.5 MB (25525248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce197f17dcb5ff1f3fc239d57ba39190ccc18d6324364afe512f8061f11cfb`  
		Last Modified: Sat, 28 Jan 2023 00:08:51 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e7bdd9aebc9c3f60792159ce76da2df9a453977d112739f605357c6d01aa53`  
		Last Modified: Sat, 28 Jan 2023 00:09:00 GMT  
		Size: 48.4 MB (48447391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de2e85fdede9323464c34c692606810abfe152d22f8007e05e3419f662a8f5`  
		Last Modified: Sat, 28 Jan 2023 00:08:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006f2ea3576a5de92edb14f65f32d4ba885bc0cb594359eebc32d4cb45a0c5fc`  
		Last Modified: Sat, 28 Jan 2023 00:08:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:6f4fb1b8c2717cbe709e755f83a3d6f52dabe58902569bdaa14d0cc9d4c18d25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:603b9b890043bd774c673060292c818e771135c51d0d2b8b7873151906610220
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162644100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4726a7600c6f5c8b58d26e8a5634a13bdff727ee29eebe5edbf9ebdd00533898`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 Jan 2023 02:35:07 GMT
ADD file:67ceb946e54c26c505b5f9f393d77befbd5e9b3b5c069ca301e314ecc74456b0 in / 
# Wed, 11 Jan 2023 02:35:07 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 06:20:12 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 Jan 2023 06:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:20:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 Jan 2023 06:20:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 Jan 2023 06:20:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 Jan 2023 06:20:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:20:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 Jan 2023 06:20:36 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 17 Jan 2023 21:08:53 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Tue, 17 Jan 2023 21:08:54 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 17 Jan 2023 21:09:16 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 17 Jan 2023 21:09:17 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 Jan 2023 21:09:17 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 17 Jan 2023 21:09:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Jan 2023 21:09:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Jan 2023 21:09:18 GMT
EXPOSE 3306 33060
# Tue, 17 Jan 2023 21:09:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:548fcab5fe888f589dd092c68b813bfd65359878bd1950d6b753f749e82ebd7c`  
		Last Modified: Wed, 11 Jan 2023 02:39:48 GMT  
		Size: 27.1 MB (27140352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702e45a0d0fab46740d0cf404969001dc0537dd564973fa6f31da2a00cfe5ef8`  
		Last Modified: Wed, 11 Jan 2023 06:22:03 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad96d17a23a7cff619709675f8981274e6a4ff7a9fb99590f0a837511e69a50b`  
		Last Modified: Wed, 11 Jan 2023 06:22:03 GMT  
		Size: 4.2 MB (4182274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1832d5509d3dce5314c5ffb58ac35ef7e35c396457e6fab747267312751708cf`  
		Last Modified: Wed, 11 Jan 2023 06:22:02 GMT  
		Size: 1.4 MB (1388883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5a580bc4aa47839f3f325b0a7bd7f927d8f41bb947a8e6d1847048a16c88dc`  
		Last Modified: Wed, 11 Jan 2023 06:22:01 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562f0a131c6cc56e3a6b85245641c4251cb4bc5e5b97f08d5d97209b8c11c38c`  
		Last Modified: Wed, 11 Jan 2023 06:22:04 GMT  
		Size: 14.1 MB (14089400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5760997e25e0fd516f2aab1a32be22ae0a919faa2c2dd36a3ad098d772ca3495`  
		Last Modified: Wed, 11 Jan 2023 06:22:00 GMT  
		Size: 2.5 KB (2543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2459447ebb40538b162dbc50dd435551e3c63d290fc1fb37555ee724a56989a9`  
		Last Modified: Tue, 17 Jan 2023 21:11:22 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b7ab69b071a7139fbe466170a22caead38334834a792630c6a0e9b12f15ef6`  
		Last Modified: Tue, 17 Jan 2023 21:11:37 GMT  
		Size: 115.8 MB (115832999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aad2d01a4e6a079bc797ac021db4938622225182fa24eab797ee661d30134e9`  
		Last Modified: Tue, 17 Jan 2023 21:11:22 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d70cf470197d6c4c9c3f0789a15440b5439ac8536ea8db923608b24b7dfc59`  
		Last Modified: Tue, 17 Jan 2023 21:11:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:7fe02bf3592e9ec218e17f0bf39bd3fc7a118c6426e63bea849ef358b798c74b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:d8aa78a2e64fe5d55050c9eb82a056edda57cb5bd9978c8abd93a2cc5a0c1282
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129921235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec14ca3fec4d86d989ea6ac3f66af44da0298438e1082b0f1682dba5c912fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:36 GMT
ADD file:eefc8abcbb6ec3141573da12cc99f3d9592d5a0bd105bb189e0e1db15c0d1bf5 in / 
# Fri, 27 Jan 2023 23:36:37 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:06:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:06:33 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:06:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:06:55 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sat, 28 Jan 2023 00:06:56 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:06:56 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 28 Jan 2023 00:06:56 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Sat, 28 Jan 2023 00:06:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:07:14 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:07:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:07:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Sat, 28 Jan 2023 00:07:39 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:07:40 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:07:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:07:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:07:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:07:41 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:07:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e048d0a387420acfdb05a1ec44ed79aa01be81adcd731b3100359277ca89d08b`  
		Last Modified: Fri, 27 Jan 2023 23:38:26 GMT  
		Size: 50.5 MB (50466577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7847c8a41cb8230f06f790ec1f0ed987fa4b9fea784840951ddc7adda2efe08`  
		Last Modified: Sat, 28 Jan 2023 00:08:54 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c400748dd907cc0ad8565e047359c9c7164407c0ee46463b7e03928b2ba72a70`  
		Last Modified: Sat, 28 Jan 2023 00:08:54 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59c21f62b1f96c3c2adb9e74f8dd2739f1a720d964c5e28110f8a192309323d`  
		Last Modified: Sat, 28 Jan 2023 00:08:53 GMT  
		Size: 4.5 MB (4542101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426e724ab5eb21fa69a123fee2d03329e1c9e9638256006bbc0d4b85ad5ec6c9`  
		Last Modified: Sat, 28 Jan 2023 00:08:52 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc537924e52d943105cc6a151c17b2492abf07558c700823ee579e0b697726b6`  
		Last Modified: Sat, 28 Jan 2023 00:08:52 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa4edfb8fd8f8db7918a3efa8428c072e80a26c726b804998177f0aec27f07f`  
		Last Modified: Sat, 28 Jan 2023 00:08:55 GMT  
		Size: 25.5 MB (25525248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce197f17dcb5ff1f3fc239d57ba39190ccc18d6324364afe512f8061f11cfb`  
		Last Modified: Sat, 28 Jan 2023 00:08:51 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e7bdd9aebc9c3f60792159ce76da2df9a453977d112739f605357c6d01aa53`  
		Last Modified: Sat, 28 Jan 2023 00:09:00 GMT  
		Size: 48.4 MB (48447391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de2e85fdede9323464c34c692606810abfe152d22f8007e05e3419f662a8f5`  
		Last Modified: Sat, 28 Jan 2023 00:08:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006f2ea3576a5de92edb14f65f32d4ba885bc0cb594359eebc32d4cb45a0c5fc`  
		Last Modified: Sat, 28 Jan 2023 00:08:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.41`

```console
$ docker pull mysql@sha256:7fe02bf3592e9ec218e17f0bf39bd3fc7a118c6426e63bea849ef358b798c74b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.41` - linux; amd64

```console
$ docker pull mysql@sha256:d8aa78a2e64fe5d55050c9eb82a056edda57cb5bd9978c8abd93a2cc5a0c1282
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129921235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec14ca3fec4d86d989ea6ac3f66af44da0298438e1082b0f1682dba5c912fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:36 GMT
ADD file:eefc8abcbb6ec3141573da12cc99f3d9592d5a0bd105bb189e0e1db15c0d1bf5 in / 
# Fri, 27 Jan 2023 23:36:37 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:06:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:06:33 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:06:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:06:55 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sat, 28 Jan 2023 00:06:56 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:06:56 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 28 Jan 2023 00:06:56 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Sat, 28 Jan 2023 00:06:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:07:14 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:07:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:07:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Sat, 28 Jan 2023 00:07:39 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:07:40 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:07:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:07:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:07:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:07:41 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:07:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e048d0a387420acfdb05a1ec44ed79aa01be81adcd731b3100359277ca89d08b`  
		Last Modified: Fri, 27 Jan 2023 23:38:26 GMT  
		Size: 50.5 MB (50466577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7847c8a41cb8230f06f790ec1f0ed987fa4b9fea784840951ddc7adda2efe08`  
		Last Modified: Sat, 28 Jan 2023 00:08:54 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c400748dd907cc0ad8565e047359c9c7164407c0ee46463b7e03928b2ba72a70`  
		Last Modified: Sat, 28 Jan 2023 00:08:54 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59c21f62b1f96c3c2adb9e74f8dd2739f1a720d964c5e28110f8a192309323d`  
		Last Modified: Sat, 28 Jan 2023 00:08:53 GMT  
		Size: 4.5 MB (4542101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426e724ab5eb21fa69a123fee2d03329e1c9e9638256006bbc0d4b85ad5ec6c9`  
		Last Modified: Sat, 28 Jan 2023 00:08:52 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc537924e52d943105cc6a151c17b2492abf07558c700823ee579e0b697726b6`  
		Last Modified: Sat, 28 Jan 2023 00:08:52 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa4edfb8fd8f8db7918a3efa8428c072e80a26c726b804998177f0aec27f07f`  
		Last Modified: Sat, 28 Jan 2023 00:08:55 GMT  
		Size: 25.5 MB (25525248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce197f17dcb5ff1f3fc239d57ba39190ccc18d6324364afe512f8061f11cfb`  
		Last Modified: Sat, 28 Jan 2023 00:08:51 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e7bdd9aebc9c3f60792159ce76da2df9a453977d112739f605357c6d01aa53`  
		Last Modified: Sat, 28 Jan 2023 00:09:00 GMT  
		Size: 48.4 MB (48447391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de2e85fdede9323464c34c692606810abfe152d22f8007e05e3419f662a8f5`  
		Last Modified: Sat, 28 Jan 2023 00:08:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006f2ea3576a5de92edb14f65f32d4ba885bc0cb594359eebc32d4cb45a0c5fc`  
		Last Modified: Sat, 28 Jan 2023 00:08:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.41-debian`

```console
$ docker pull mysql@sha256:6f4fb1b8c2717cbe709e755f83a3d6f52dabe58902569bdaa14d0cc9d4c18d25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.41-debian` - linux; amd64

```console
$ docker pull mysql@sha256:603b9b890043bd774c673060292c818e771135c51d0d2b8b7873151906610220
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162644100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4726a7600c6f5c8b58d26e8a5634a13bdff727ee29eebe5edbf9ebdd00533898`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 Jan 2023 02:35:07 GMT
ADD file:67ceb946e54c26c505b5f9f393d77befbd5e9b3b5c069ca301e314ecc74456b0 in / 
# Wed, 11 Jan 2023 02:35:07 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 06:20:12 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 Jan 2023 06:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:20:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 Jan 2023 06:20:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 Jan 2023 06:20:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 Jan 2023 06:20:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:20:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 Jan 2023 06:20:36 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 17 Jan 2023 21:08:53 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Tue, 17 Jan 2023 21:08:54 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 17 Jan 2023 21:09:16 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 17 Jan 2023 21:09:17 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 Jan 2023 21:09:17 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 17 Jan 2023 21:09:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Jan 2023 21:09:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Jan 2023 21:09:18 GMT
EXPOSE 3306 33060
# Tue, 17 Jan 2023 21:09:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:548fcab5fe888f589dd092c68b813bfd65359878bd1950d6b753f749e82ebd7c`  
		Last Modified: Wed, 11 Jan 2023 02:39:48 GMT  
		Size: 27.1 MB (27140352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702e45a0d0fab46740d0cf404969001dc0537dd564973fa6f31da2a00cfe5ef8`  
		Last Modified: Wed, 11 Jan 2023 06:22:03 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad96d17a23a7cff619709675f8981274e6a4ff7a9fb99590f0a837511e69a50b`  
		Last Modified: Wed, 11 Jan 2023 06:22:03 GMT  
		Size: 4.2 MB (4182274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1832d5509d3dce5314c5ffb58ac35ef7e35c396457e6fab747267312751708cf`  
		Last Modified: Wed, 11 Jan 2023 06:22:02 GMT  
		Size: 1.4 MB (1388883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5a580bc4aa47839f3f325b0a7bd7f927d8f41bb947a8e6d1847048a16c88dc`  
		Last Modified: Wed, 11 Jan 2023 06:22:01 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562f0a131c6cc56e3a6b85245641c4251cb4bc5e5b97f08d5d97209b8c11c38c`  
		Last Modified: Wed, 11 Jan 2023 06:22:04 GMT  
		Size: 14.1 MB (14089400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5760997e25e0fd516f2aab1a32be22ae0a919faa2c2dd36a3ad098d772ca3495`  
		Last Modified: Wed, 11 Jan 2023 06:22:00 GMT  
		Size: 2.5 KB (2543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2459447ebb40538b162dbc50dd435551e3c63d290fc1fb37555ee724a56989a9`  
		Last Modified: Tue, 17 Jan 2023 21:11:22 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b7ab69b071a7139fbe466170a22caead38334834a792630c6a0e9b12f15ef6`  
		Last Modified: Tue, 17 Jan 2023 21:11:37 GMT  
		Size: 115.8 MB (115832999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aad2d01a4e6a079bc797ac021db4938622225182fa24eab797ee661d30134e9`  
		Last Modified: Tue, 17 Jan 2023 21:11:22 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d70cf470197d6c4c9c3f0789a15440b5439ac8536ea8db923608b24b7dfc59`  
		Last Modified: Tue, 17 Jan 2023 21:11:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.41-oracle`

```console
$ docker pull mysql@sha256:7fe02bf3592e9ec218e17f0bf39bd3fc7a118c6426e63bea849ef358b798c74b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.41-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:d8aa78a2e64fe5d55050c9eb82a056edda57cb5bd9978c8abd93a2cc5a0c1282
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129921235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec14ca3fec4d86d989ea6ac3f66af44da0298438e1082b0f1682dba5c912fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:36 GMT
ADD file:eefc8abcbb6ec3141573da12cc99f3d9592d5a0bd105bb189e0e1db15c0d1bf5 in / 
# Fri, 27 Jan 2023 23:36:37 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:06:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:06:33 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:06:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:06:55 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sat, 28 Jan 2023 00:06:56 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:06:56 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 28 Jan 2023 00:06:56 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Sat, 28 Jan 2023 00:06:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:07:14 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:07:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:07:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Sat, 28 Jan 2023 00:07:39 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:07:40 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:07:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:07:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:07:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:07:41 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:07:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e048d0a387420acfdb05a1ec44ed79aa01be81adcd731b3100359277ca89d08b`  
		Last Modified: Fri, 27 Jan 2023 23:38:26 GMT  
		Size: 50.5 MB (50466577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7847c8a41cb8230f06f790ec1f0ed987fa4b9fea784840951ddc7adda2efe08`  
		Last Modified: Sat, 28 Jan 2023 00:08:54 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c400748dd907cc0ad8565e047359c9c7164407c0ee46463b7e03928b2ba72a70`  
		Last Modified: Sat, 28 Jan 2023 00:08:54 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59c21f62b1f96c3c2adb9e74f8dd2739f1a720d964c5e28110f8a192309323d`  
		Last Modified: Sat, 28 Jan 2023 00:08:53 GMT  
		Size: 4.5 MB (4542101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426e724ab5eb21fa69a123fee2d03329e1c9e9638256006bbc0d4b85ad5ec6c9`  
		Last Modified: Sat, 28 Jan 2023 00:08:52 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc537924e52d943105cc6a151c17b2492abf07558c700823ee579e0b697726b6`  
		Last Modified: Sat, 28 Jan 2023 00:08:52 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa4edfb8fd8f8db7918a3efa8428c072e80a26c726b804998177f0aec27f07f`  
		Last Modified: Sat, 28 Jan 2023 00:08:55 GMT  
		Size: 25.5 MB (25525248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce197f17dcb5ff1f3fc239d57ba39190ccc18d6324364afe512f8061f11cfb`  
		Last Modified: Sat, 28 Jan 2023 00:08:51 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e7bdd9aebc9c3f60792159ce76da2df9a453977d112739f605357c6d01aa53`  
		Last Modified: Sat, 28 Jan 2023 00:09:00 GMT  
		Size: 48.4 MB (48447391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de2e85fdede9323464c34c692606810abfe152d22f8007e05e3419f662a8f5`  
		Last Modified: Sat, 28 Jan 2023 00:08:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006f2ea3576a5de92edb14f65f32d4ba885bc0cb594359eebc32d4cb45a0c5fc`  
		Last Modified: Sat, 28 Jan 2023 00:08:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:3e81836557ec9ba2e151a7dbcb7ae7de732e63a22babead7afd91731aeaabf21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:cca95ddffb7c92b6c1e8da81b298a870d2f48183bebb8146d63be189ab3e37ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152665582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf3aa69f5f07d1c43c04c21627b32612760eca280ed4fe1529089a17b37b7a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:04:39 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:04:42 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:05:06 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 28 Jan 2023 00:05:07 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:05:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:05:39 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:05:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:05:40 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:06:14 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:06:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:06:15 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:06:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:06:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:06:16 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:06:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:39fbafb6c7ef40878b859fd0e4475c5ebd2ddfa8ed785a588594e8731b7cd0e8`  
		Last Modified: Fri, 27 Jan 2023 23:37:50 GMT  
		Size: 44.6 MB (44561081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e9f8ca4fd737123f9bf9fba4474d86b6e5f85291c5f9e50d2b93a1b7e83d6c`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fcdd923e548acea3ed340c20b76ef2719c0e0e6ba4408539866ba427ef9ffec`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15716fe15a39bcddcd0f7db611807ce9d4e307ee956edb69eaf5ecbac1470960`  
		Last Modified: Sat, 28 Jan 2023 00:08:20 GMT  
		Size: 4.6 MB (4611609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c8bb47c8b937c4bcf1dbebdbfd0e5bf8dd1506a3e5867d8013520b711129cf`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b050c46cac02a277087e65c3221fd4a43580659eee0590540567fd2c841491a4`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e19c22a377370b121755f4ca6da19d43ad931cddba1241fcc0ba69a850e6b8a`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 56.2 MB (56219323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2abd6d528f13cf5649363ca47e3dd5d88e430315c55ee1e826bf233b4b1d26e`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca593545a5782413367c683d2559893e498a32d71d2dec8499f06e3861baf6`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 46.3 MB (46335045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a262a30fc7feee8146227e4a6f8004ced2cfed471ce2f21fac712aa8deb7d08`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1170ff1b1e9d9726b2a806fbf4534ba0e9b7f083aa241b963a394b30107119b`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:f2a4f6141e72932f685e7a672076e3d5c7e143b7521af145b3327243b66fbd80
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.6 MB (151597491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6a0d93ee459e7bbfa6b5fbdad8d936c3d31627a9b39b4903d934f68b714d92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 22:41:06 GMT
ADD file:63b5b4161762e1845c1eb2bb2c967a07179819b4a1f12ab7596d9c6bd15c9cbd in / 
# Fri, 27 Jan 2023 22:41:06 GMT
CMD ["/bin/bash"]
# Fri, 27 Jan 2023 23:09:15 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 01:03:33 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 01:03:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 01:03:57 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 01:03:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:03:59 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 01:04:24 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 01:04:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 01:04:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:04:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 01:04:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 01:04:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 01:04:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 01:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 01:04:56 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 01:04:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26cdabfc8c6a31055d655a58d8a8f9757f43e1ce58451b8b6b02c5dd6e6d482`  
		Last Modified: Fri, 27 Jan 2023 22:42:28 GMT  
		Size: 43.5 MB (43456742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc45082a5180093f9c621428a076fbc28411899fe16d4fedc7cbc3958d407490`  
		Last Modified: Fri, 27 Jan 2023 23:11:07 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a283935394cf9ad112dfadaabd1bdf2343754a3652feb036438b2506fd859370`  
		Last Modified: Wed, 01 Feb 2023 01:05:26 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0b96316a56f812e8603b0490201e0f0f8bd5af4aa6b39f2c33781d4c060ebc`  
		Last Modified: Wed, 01 Feb 2023 01:05:25 GMT  
		Size: 4.5 MB (4470678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aefff8b7fc46c48135277e5eded9718c6b99a57586362b1acaac7dad4659e83`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdb2af2a3a435ab2d3616331ae8e9fba95e23d211b2d97ee3dc2b13cb0c0be1`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157c24da0e9d8a2f8fcaa392b46b72c5be69388be6c21e0e65c528a332da304a`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 55.6 MB (55609254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb89415e30193670069fa6526deeda86bb88de457b70aed510826aa639b2d5cc`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259d0773a9cc657509d539b1f03c4d4ad97c742e5dd220aec9a9d8d1e2534d63`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 47.1 MB (47138134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf77a02adec01c9b3a42a0508ff8eb1507bef1909da4074899de1a841c26108`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642af7c41ad7c8e5582b50d2072b296dd9c209fff84e21865dbf2994d67cf6e`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:36a7e9407344cd1cb4064179962c207cd2afb13bfbb63992f0ca328e4b56b515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c86f3664bddd89bd539049f71c1ffc0816e18d01fad192addfb02d9e2834351c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.7 MB (177699276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33ba092bab95e48e4e7ea71d2f5e5603108185e259e011179aa03b26ad5d5067`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 06:19:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 Jan 2023 06:19:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:19:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 Jan 2023 06:19:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 Jan 2023 06:19:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 Jan 2023 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:19:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 Jan 2023 06:19:45 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 Jan 2023 21:07:31 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Tue, 17 Jan 2023 21:07:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 17 Jan 2023 21:07:48 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 17 Jan 2023 21:07:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 Jan 2023 21:07:49 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 17 Jan 2023 21:07:49 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 17 Jan 2023 21:07:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Jan 2023 21:07:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Jan 2023 21:07:50 GMT
EXPOSE 3306 33060
# Tue, 17 Jan 2023 21:07:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346580bcb1a6e9e1becd3883a38670cdca1f47b7cdbe65121708af5458a0318`  
		Last Modified: Wed, 11 Jan 2023 06:21:26 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec40bb6547aaa95db6bda6d1de84761264c716477d2d8b998856586285b4ec55`  
		Last Modified: Wed, 11 Jan 2023 06:21:27 GMT  
		Size: 4.4 MB (4414919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efef7c7e25176536d7c2c61700c323a83aa93894c4e3f250e6318cc77182410c`  
		Last Modified: Wed, 11 Jan 2023 06:21:25 GMT  
		Size: 1.4 MB (1418481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cd4a9c65ce2ab7c83d934277938ac0b60b14038ed82a23768c5829e04bca7f`  
		Last Modified: Wed, 11 Jan 2023 06:21:25 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4caf695f1e31c50fb977d1da7e28a7de9f4dacc6d937f16b3b2da8b263527ab`  
		Last Modified: Wed, 11 Jan 2023 06:21:28 GMT  
		Size: 12.7 MB (12662003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621837b69253e21538e7e8b097d99a96bbd14ef7c98668c7f1587a5898849f36`  
		Last Modified: Wed, 11 Jan 2023 06:21:25 GMT  
		Size: 2.5 KB (2546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c903d5cfd80f351193456503656367928154b4d6c52beb99423204b56df74`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406689e3dbcc29124df7a749b01725da213b58aea774407bdb102b0d00567b4a`  
		Last Modified: Tue, 17 Jan 2023 21:10:40 GMT  
		Size: 127.8 MB (127795859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4016832f0b21d3dbdb52cbe137c71f532d7f4515eb11a6d50e6590a5621cef82`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4236ef87c29f872eca03df1e079fbb2b174c44258b1ac06d6ccbd10a7c7efc`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedfbe312f9b4e2371da8769a8336c98cc9639575b92216f327fa63b4d034558`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:3e81836557ec9ba2e151a7dbcb7ae7de732e63a22babead7afd91731aeaabf21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:cca95ddffb7c92b6c1e8da81b298a870d2f48183bebb8146d63be189ab3e37ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152665582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf3aa69f5f07d1c43c04c21627b32612760eca280ed4fe1529089a17b37b7a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:04:39 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:04:42 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:05:06 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 28 Jan 2023 00:05:07 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:05:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:05:39 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:05:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:05:40 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:06:14 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:06:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:06:15 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:06:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:06:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:06:16 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:06:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:39fbafb6c7ef40878b859fd0e4475c5ebd2ddfa8ed785a588594e8731b7cd0e8`  
		Last Modified: Fri, 27 Jan 2023 23:37:50 GMT  
		Size: 44.6 MB (44561081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e9f8ca4fd737123f9bf9fba4474d86b6e5f85291c5f9e50d2b93a1b7e83d6c`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fcdd923e548acea3ed340c20b76ef2719c0e0e6ba4408539866ba427ef9ffec`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15716fe15a39bcddcd0f7db611807ce9d4e307ee956edb69eaf5ecbac1470960`  
		Last Modified: Sat, 28 Jan 2023 00:08:20 GMT  
		Size: 4.6 MB (4611609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c8bb47c8b937c4bcf1dbebdbfd0e5bf8dd1506a3e5867d8013520b711129cf`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b050c46cac02a277087e65c3221fd4a43580659eee0590540567fd2c841491a4`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e19c22a377370b121755f4ca6da19d43ad931cddba1241fcc0ba69a850e6b8a`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 56.2 MB (56219323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2abd6d528f13cf5649363ca47e3dd5d88e430315c55ee1e826bf233b4b1d26e`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca593545a5782413367c683d2559893e498a32d71d2dec8499f06e3861baf6`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 46.3 MB (46335045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a262a30fc7feee8146227e4a6f8004ced2cfed471ce2f21fac712aa8deb7d08`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1170ff1b1e9d9726b2a806fbf4534ba0e9b7f083aa241b963a394b30107119b`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:f2a4f6141e72932f685e7a672076e3d5c7e143b7521af145b3327243b66fbd80
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.6 MB (151597491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6a0d93ee459e7bbfa6b5fbdad8d936c3d31627a9b39b4903d934f68b714d92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 22:41:06 GMT
ADD file:63b5b4161762e1845c1eb2bb2c967a07179819b4a1f12ab7596d9c6bd15c9cbd in / 
# Fri, 27 Jan 2023 22:41:06 GMT
CMD ["/bin/bash"]
# Fri, 27 Jan 2023 23:09:15 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 01:03:33 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 01:03:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 01:03:57 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 01:03:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:03:59 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 01:04:24 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 01:04:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 01:04:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:04:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 01:04:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 01:04:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 01:04:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 01:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 01:04:56 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 01:04:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26cdabfc8c6a31055d655a58d8a8f9757f43e1ce58451b8b6b02c5dd6e6d482`  
		Last Modified: Fri, 27 Jan 2023 22:42:28 GMT  
		Size: 43.5 MB (43456742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc45082a5180093f9c621428a076fbc28411899fe16d4fedc7cbc3958d407490`  
		Last Modified: Fri, 27 Jan 2023 23:11:07 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a283935394cf9ad112dfadaabd1bdf2343754a3652feb036438b2506fd859370`  
		Last Modified: Wed, 01 Feb 2023 01:05:26 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0b96316a56f812e8603b0490201e0f0f8bd5af4aa6b39f2c33781d4c060ebc`  
		Last Modified: Wed, 01 Feb 2023 01:05:25 GMT  
		Size: 4.5 MB (4470678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aefff8b7fc46c48135277e5eded9718c6b99a57586362b1acaac7dad4659e83`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdb2af2a3a435ab2d3616331ae8e9fba95e23d211b2d97ee3dc2b13cb0c0be1`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157c24da0e9d8a2f8fcaa392b46b72c5be69388be6c21e0e65c528a332da304a`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 55.6 MB (55609254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb89415e30193670069fa6526deeda86bb88de457b70aed510826aa639b2d5cc`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259d0773a9cc657509d539b1f03c4d4ad97c742e5dd220aec9a9d8d1e2534d63`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 47.1 MB (47138134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf77a02adec01c9b3a42a0508ff8eb1507bef1909da4074899de1a841c26108`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642af7c41ad7c8e5582b50d2072b296dd9c209fff84e21865dbf2994d67cf6e`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:3e81836557ec9ba2e151a7dbcb7ae7de732e63a22babead7afd91731aeaabf21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:cca95ddffb7c92b6c1e8da81b298a870d2f48183bebb8146d63be189ab3e37ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152665582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf3aa69f5f07d1c43c04c21627b32612760eca280ed4fe1529089a17b37b7a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:04:39 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:04:42 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:05:06 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 28 Jan 2023 00:05:07 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:05:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:05:39 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:05:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:05:40 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:06:14 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:06:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:06:15 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:06:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:06:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:06:16 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:06:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:39fbafb6c7ef40878b859fd0e4475c5ebd2ddfa8ed785a588594e8731b7cd0e8`  
		Last Modified: Fri, 27 Jan 2023 23:37:50 GMT  
		Size: 44.6 MB (44561081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e9f8ca4fd737123f9bf9fba4474d86b6e5f85291c5f9e50d2b93a1b7e83d6c`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fcdd923e548acea3ed340c20b76ef2719c0e0e6ba4408539866ba427ef9ffec`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15716fe15a39bcddcd0f7db611807ce9d4e307ee956edb69eaf5ecbac1470960`  
		Last Modified: Sat, 28 Jan 2023 00:08:20 GMT  
		Size: 4.6 MB (4611609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c8bb47c8b937c4bcf1dbebdbfd0e5bf8dd1506a3e5867d8013520b711129cf`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b050c46cac02a277087e65c3221fd4a43580659eee0590540567fd2c841491a4`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e19c22a377370b121755f4ca6da19d43ad931cddba1241fcc0ba69a850e6b8a`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 56.2 MB (56219323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2abd6d528f13cf5649363ca47e3dd5d88e430315c55ee1e826bf233b4b1d26e`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca593545a5782413367c683d2559893e498a32d71d2dec8499f06e3861baf6`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 46.3 MB (46335045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a262a30fc7feee8146227e4a6f8004ced2cfed471ce2f21fac712aa8deb7d08`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1170ff1b1e9d9726b2a806fbf4534ba0e9b7f083aa241b963a394b30107119b`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:f2a4f6141e72932f685e7a672076e3d5c7e143b7521af145b3327243b66fbd80
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.6 MB (151597491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6a0d93ee459e7bbfa6b5fbdad8d936c3d31627a9b39b4903d934f68b714d92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 22:41:06 GMT
ADD file:63b5b4161762e1845c1eb2bb2c967a07179819b4a1f12ab7596d9c6bd15c9cbd in / 
# Fri, 27 Jan 2023 22:41:06 GMT
CMD ["/bin/bash"]
# Fri, 27 Jan 2023 23:09:15 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 01:03:33 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 01:03:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 01:03:57 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 01:03:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:03:59 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 01:04:24 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 01:04:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 01:04:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:04:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 01:04:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 01:04:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 01:04:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 01:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 01:04:56 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 01:04:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26cdabfc8c6a31055d655a58d8a8f9757f43e1ce58451b8b6b02c5dd6e6d482`  
		Last Modified: Fri, 27 Jan 2023 22:42:28 GMT  
		Size: 43.5 MB (43456742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc45082a5180093f9c621428a076fbc28411899fe16d4fedc7cbc3958d407490`  
		Last Modified: Fri, 27 Jan 2023 23:11:07 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a283935394cf9ad112dfadaabd1bdf2343754a3652feb036438b2506fd859370`  
		Last Modified: Wed, 01 Feb 2023 01:05:26 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0b96316a56f812e8603b0490201e0f0f8bd5af4aa6b39f2c33781d4c060ebc`  
		Last Modified: Wed, 01 Feb 2023 01:05:25 GMT  
		Size: 4.5 MB (4470678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aefff8b7fc46c48135277e5eded9718c6b99a57586362b1acaac7dad4659e83`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdb2af2a3a435ab2d3616331ae8e9fba95e23d211b2d97ee3dc2b13cb0c0be1`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157c24da0e9d8a2f8fcaa392b46b72c5be69388be6c21e0e65c528a332da304a`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 55.6 MB (55609254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb89415e30193670069fa6526deeda86bb88de457b70aed510826aa639b2d5cc`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259d0773a9cc657509d539b1f03c4d4ad97c742e5dd220aec9a9d8d1e2534d63`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 47.1 MB (47138134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf77a02adec01c9b3a42a0508ff8eb1507bef1909da4074899de1a841c26108`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642af7c41ad7c8e5582b50d2072b296dd9c209fff84e21865dbf2994d67cf6e`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:36a7e9407344cd1cb4064179962c207cd2afb13bfbb63992f0ca328e4b56b515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c86f3664bddd89bd539049f71c1ffc0816e18d01fad192addfb02d9e2834351c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.7 MB (177699276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33ba092bab95e48e4e7ea71d2f5e5603108185e259e011179aa03b26ad5d5067`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 06:19:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 Jan 2023 06:19:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:19:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 Jan 2023 06:19:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 Jan 2023 06:19:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 Jan 2023 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:19:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 Jan 2023 06:19:45 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 Jan 2023 21:07:31 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Tue, 17 Jan 2023 21:07:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 17 Jan 2023 21:07:48 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 17 Jan 2023 21:07:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 Jan 2023 21:07:49 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 17 Jan 2023 21:07:49 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 17 Jan 2023 21:07:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Jan 2023 21:07:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Jan 2023 21:07:50 GMT
EXPOSE 3306 33060
# Tue, 17 Jan 2023 21:07:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346580bcb1a6e9e1becd3883a38670cdca1f47b7cdbe65121708af5458a0318`  
		Last Modified: Wed, 11 Jan 2023 06:21:26 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec40bb6547aaa95db6bda6d1de84761264c716477d2d8b998856586285b4ec55`  
		Last Modified: Wed, 11 Jan 2023 06:21:27 GMT  
		Size: 4.4 MB (4414919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efef7c7e25176536d7c2c61700c323a83aa93894c4e3f250e6318cc77182410c`  
		Last Modified: Wed, 11 Jan 2023 06:21:25 GMT  
		Size: 1.4 MB (1418481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cd4a9c65ce2ab7c83d934277938ac0b60b14038ed82a23768c5829e04bca7f`  
		Last Modified: Wed, 11 Jan 2023 06:21:25 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4caf695f1e31c50fb977d1da7e28a7de9f4dacc6d937f16b3b2da8b263527ab`  
		Last Modified: Wed, 11 Jan 2023 06:21:28 GMT  
		Size: 12.7 MB (12662003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621837b69253e21538e7e8b097d99a96bbd14ef7c98668c7f1587a5898849f36`  
		Last Modified: Wed, 11 Jan 2023 06:21:25 GMT  
		Size: 2.5 KB (2546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c903d5cfd80f351193456503656367928154b4d6c52beb99423204b56df74`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406689e3dbcc29124df7a749b01725da213b58aea774407bdb102b0d00567b4a`  
		Last Modified: Tue, 17 Jan 2023 21:10:40 GMT  
		Size: 127.8 MB (127795859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4016832f0b21d3dbdb52cbe137c71f532d7f4515eb11a6d50e6590a5621cef82`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4236ef87c29f872eca03df1e079fbb2b174c44258b1ac06d6ccbd10a7c7efc`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedfbe312f9b4e2371da8769a8336c98cc9639575b92216f327fa63b4d034558`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:3e81836557ec9ba2e151a7dbcb7ae7de732e63a22babead7afd91731aeaabf21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:cca95ddffb7c92b6c1e8da81b298a870d2f48183bebb8146d63be189ab3e37ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152665582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf3aa69f5f07d1c43c04c21627b32612760eca280ed4fe1529089a17b37b7a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:04:39 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:04:42 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:05:06 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 28 Jan 2023 00:05:07 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:05:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:05:39 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:05:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:05:40 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:06:14 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:06:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:06:15 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:06:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:06:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:06:16 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:06:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:39fbafb6c7ef40878b859fd0e4475c5ebd2ddfa8ed785a588594e8731b7cd0e8`  
		Last Modified: Fri, 27 Jan 2023 23:37:50 GMT  
		Size: 44.6 MB (44561081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e9f8ca4fd737123f9bf9fba4474d86b6e5f85291c5f9e50d2b93a1b7e83d6c`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fcdd923e548acea3ed340c20b76ef2719c0e0e6ba4408539866ba427ef9ffec`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15716fe15a39bcddcd0f7db611807ce9d4e307ee956edb69eaf5ecbac1470960`  
		Last Modified: Sat, 28 Jan 2023 00:08:20 GMT  
		Size: 4.6 MB (4611609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c8bb47c8b937c4bcf1dbebdbfd0e5bf8dd1506a3e5867d8013520b711129cf`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b050c46cac02a277087e65c3221fd4a43580659eee0590540567fd2c841491a4`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e19c22a377370b121755f4ca6da19d43ad931cddba1241fcc0ba69a850e6b8a`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 56.2 MB (56219323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2abd6d528f13cf5649363ca47e3dd5d88e430315c55ee1e826bf233b4b1d26e`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca593545a5782413367c683d2559893e498a32d71d2dec8499f06e3861baf6`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 46.3 MB (46335045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a262a30fc7feee8146227e4a6f8004ced2cfed471ce2f21fac712aa8deb7d08`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1170ff1b1e9d9726b2a806fbf4534ba0e9b7f083aa241b963a394b30107119b`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:f2a4f6141e72932f685e7a672076e3d5c7e143b7521af145b3327243b66fbd80
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.6 MB (151597491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6a0d93ee459e7bbfa6b5fbdad8d936c3d31627a9b39b4903d934f68b714d92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 22:41:06 GMT
ADD file:63b5b4161762e1845c1eb2bb2c967a07179819b4a1f12ab7596d9c6bd15c9cbd in / 
# Fri, 27 Jan 2023 22:41:06 GMT
CMD ["/bin/bash"]
# Fri, 27 Jan 2023 23:09:15 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 01:03:33 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 01:03:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 01:03:57 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 01:03:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:03:59 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 01:04:24 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 01:04:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 01:04:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:04:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 01:04:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 01:04:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 01:04:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 01:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 01:04:56 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 01:04:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26cdabfc8c6a31055d655a58d8a8f9757f43e1ce58451b8b6b02c5dd6e6d482`  
		Last Modified: Fri, 27 Jan 2023 22:42:28 GMT  
		Size: 43.5 MB (43456742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc45082a5180093f9c621428a076fbc28411899fe16d4fedc7cbc3958d407490`  
		Last Modified: Fri, 27 Jan 2023 23:11:07 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a283935394cf9ad112dfadaabd1bdf2343754a3652feb036438b2506fd859370`  
		Last Modified: Wed, 01 Feb 2023 01:05:26 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0b96316a56f812e8603b0490201e0f0f8bd5af4aa6b39f2c33781d4c060ebc`  
		Last Modified: Wed, 01 Feb 2023 01:05:25 GMT  
		Size: 4.5 MB (4470678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aefff8b7fc46c48135277e5eded9718c6b99a57586362b1acaac7dad4659e83`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdb2af2a3a435ab2d3616331ae8e9fba95e23d211b2d97ee3dc2b13cb0c0be1`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157c24da0e9d8a2f8fcaa392b46b72c5be69388be6c21e0e65c528a332da304a`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 55.6 MB (55609254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb89415e30193670069fa6526deeda86bb88de457b70aed510826aa639b2d5cc`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259d0773a9cc657509d539b1f03c4d4ad97c742e5dd220aec9a9d8d1e2534d63`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 47.1 MB (47138134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf77a02adec01c9b3a42a0508ff8eb1507bef1909da4074899de1a841c26108`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642af7c41ad7c8e5582b50d2072b296dd9c209fff84e21865dbf2994d67cf6e`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.32`

```console
$ docker pull mysql@sha256:3e81836557ec9ba2e151a7dbcb7ae7de732e63a22babead7afd91731aeaabf21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.32` - linux; amd64

```console
$ docker pull mysql@sha256:cca95ddffb7c92b6c1e8da81b298a870d2f48183bebb8146d63be189ab3e37ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152665582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf3aa69f5f07d1c43c04c21627b32612760eca280ed4fe1529089a17b37b7a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:04:39 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:04:42 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:05:06 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 28 Jan 2023 00:05:07 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:05:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:05:39 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:05:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:05:40 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:06:14 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:06:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:06:15 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:06:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:06:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:06:16 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:06:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:39fbafb6c7ef40878b859fd0e4475c5ebd2ddfa8ed785a588594e8731b7cd0e8`  
		Last Modified: Fri, 27 Jan 2023 23:37:50 GMT  
		Size: 44.6 MB (44561081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e9f8ca4fd737123f9bf9fba4474d86b6e5f85291c5f9e50d2b93a1b7e83d6c`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fcdd923e548acea3ed340c20b76ef2719c0e0e6ba4408539866ba427ef9ffec`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15716fe15a39bcddcd0f7db611807ce9d4e307ee956edb69eaf5ecbac1470960`  
		Last Modified: Sat, 28 Jan 2023 00:08:20 GMT  
		Size: 4.6 MB (4611609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c8bb47c8b937c4bcf1dbebdbfd0e5bf8dd1506a3e5867d8013520b711129cf`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b050c46cac02a277087e65c3221fd4a43580659eee0590540567fd2c841491a4`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e19c22a377370b121755f4ca6da19d43ad931cddba1241fcc0ba69a850e6b8a`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 56.2 MB (56219323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2abd6d528f13cf5649363ca47e3dd5d88e430315c55ee1e826bf233b4b1d26e`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca593545a5782413367c683d2559893e498a32d71d2dec8499f06e3861baf6`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 46.3 MB (46335045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a262a30fc7feee8146227e4a6f8004ced2cfed471ce2f21fac712aa8deb7d08`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1170ff1b1e9d9726b2a806fbf4534ba0e9b7f083aa241b963a394b30107119b`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.32` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:f2a4f6141e72932f685e7a672076e3d5c7e143b7521af145b3327243b66fbd80
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.6 MB (151597491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6a0d93ee459e7bbfa6b5fbdad8d936c3d31627a9b39b4903d934f68b714d92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 22:41:06 GMT
ADD file:63b5b4161762e1845c1eb2bb2c967a07179819b4a1f12ab7596d9c6bd15c9cbd in / 
# Fri, 27 Jan 2023 22:41:06 GMT
CMD ["/bin/bash"]
# Fri, 27 Jan 2023 23:09:15 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 01:03:33 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 01:03:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 01:03:57 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 01:03:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:03:59 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 01:04:24 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 01:04:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 01:04:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:04:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 01:04:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 01:04:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 01:04:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 01:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 01:04:56 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 01:04:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26cdabfc8c6a31055d655a58d8a8f9757f43e1ce58451b8b6b02c5dd6e6d482`  
		Last Modified: Fri, 27 Jan 2023 22:42:28 GMT  
		Size: 43.5 MB (43456742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc45082a5180093f9c621428a076fbc28411899fe16d4fedc7cbc3958d407490`  
		Last Modified: Fri, 27 Jan 2023 23:11:07 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a283935394cf9ad112dfadaabd1bdf2343754a3652feb036438b2506fd859370`  
		Last Modified: Wed, 01 Feb 2023 01:05:26 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0b96316a56f812e8603b0490201e0f0f8bd5af4aa6b39f2c33781d4c060ebc`  
		Last Modified: Wed, 01 Feb 2023 01:05:25 GMT  
		Size: 4.5 MB (4470678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aefff8b7fc46c48135277e5eded9718c6b99a57586362b1acaac7dad4659e83`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdb2af2a3a435ab2d3616331ae8e9fba95e23d211b2d97ee3dc2b13cb0c0be1`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157c24da0e9d8a2f8fcaa392b46b72c5be69388be6c21e0e65c528a332da304a`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 55.6 MB (55609254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb89415e30193670069fa6526deeda86bb88de457b70aed510826aa639b2d5cc`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259d0773a9cc657509d539b1f03c4d4ad97c742e5dd220aec9a9d8d1e2534d63`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 47.1 MB (47138134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf77a02adec01c9b3a42a0508ff8eb1507bef1909da4074899de1a841c26108`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642af7c41ad7c8e5582b50d2072b296dd9c209fff84e21865dbf2994d67cf6e`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.32-debian`

```console
$ docker pull mysql@sha256:36a7e9407344cd1cb4064179962c207cd2afb13bfbb63992f0ca328e4b56b515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.32-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c86f3664bddd89bd539049f71c1ffc0816e18d01fad192addfb02d9e2834351c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.7 MB (177699276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33ba092bab95e48e4e7ea71d2f5e5603108185e259e011179aa03b26ad5d5067`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 06:19:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 Jan 2023 06:19:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:19:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 Jan 2023 06:19:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 Jan 2023 06:19:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 Jan 2023 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:19:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 Jan 2023 06:19:45 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 Jan 2023 21:07:31 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Tue, 17 Jan 2023 21:07:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 17 Jan 2023 21:07:48 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 17 Jan 2023 21:07:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 Jan 2023 21:07:49 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 17 Jan 2023 21:07:49 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 17 Jan 2023 21:07:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Jan 2023 21:07:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Jan 2023 21:07:50 GMT
EXPOSE 3306 33060
# Tue, 17 Jan 2023 21:07:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346580bcb1a6e9e1becd3883a38670cdca1f47b7cdbe65121708af5458a0318`  
		Last Modified: Wed, 11 Jan 2023 06:21:26 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec40bb6547aaa95db6bda6d1de84761264c716477d2d8b998856586285b4ec55`  
		Last Modified: Wed, 11 Jan 2023 06:21:27 GMT  
		Size: 4.4 MB (4414919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efef7c7e25176536d7c2c61700c323a83aa93894c4e3f250e6318cc77182410c`  
		Last Modified: Wed, 11 Jan 2023 06:21:25 GMT  
		Size: 1.4 MB (1418481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cd4a9c65ce2ab7c83d934277938ac0b60b14038ed82a23768c5829e04bca7f`  
		Last Modified: Wed, 11 Jan 2023 06:21:25 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4caf695f1e31c50fb977d1da7e28a7de9f4dacc6d937f16b3b2da8b263527ab`  
		Last Modified: Wed, 11 Jan 2023 06:21:28 GMT  
		Size: 12.7 MB (12662003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621837b69253e21538e7e8b097d99a96bbd14ef7c98668c7f1587a5898849f36`  
		Last Modified: Wed, 11 Jan 2023 06:21:25 GMT  
		Size: 2.5 KB (2546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c903d5cfd80f351193456503656367928154b4d6c52beb99423204b56df74`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406689e3dbcc29124df7a749b01725da213b58aea774407bdb102b0d00567b4a`  
		Last Modified: Tue, 17 Jan 2023 21:10:40 GMT  
		Size: 127.8 MB (127795859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4016832f0b21d3dbdb52cbe137c71f532d7f4515eb11a6d50e6590a5621cef82`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4236ef87c29f872eca03df1e079fbb2b174c44258b1ac06d6ccbd10a7c7efc`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedfbe312f9b4e2371da8769a8336c98cc9639575b92216f327fa63b4d034558`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.32-oracle`

```console
$ docker pull mysql@sha256:3e81836557ec9ba2e151a7dbcb7ae7de732e63a22babead7afd91731aeaabf21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.32-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:cca95ddffb7c92b6c1e8da81b298a870d2f48183bebb8146d63be189ab3e37ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152665582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf3aa69f5f07d1c43c04c21627b32612760eca280ed4fe1529089a17b37b7a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:04:39 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:04:42 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:05:06 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 28 Jan 2023 00:05:07 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:05:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:05:39 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:05:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:05:40 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:06:14 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:06:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:06:15 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:06:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:06:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:06:16 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:06:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:39fbafb6c7ef40878b859fd0e4475c5ebd2ddfa8ed785a588594e8731b7cd0e8`  
		Last Modified: Fri, 27 Jan 2023 23:37:50 GMT  
		Size: 44.6 MB (44561081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e9f8ca4fd737123f9bf9fba4474d86b6e5f85291c5f9e50d2b93a1b7e83d6c`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fcdd923e548acea3ed340c20b76ef2719c0e0e6ba4408539866ba427ef9ffec`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15716fe15a39bcddcd0f7db611807ce9d4e307ee956edb69eaf5ecbac1470960`  
		Last Modified: Sat, 28 Jan 2023 00:08:20 GMT  
		Size: 4.6 MB (4611609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c8bb47c8b937c4bcf1dbebdbfd0e5bf8dd1506a3e5867d8013520b711129cf`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b050c46cac02a277087e65c3221fd4a43580659eee0590540567fd2c841491a4`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e19c22a377370b121755f4ca6da19d43ad931cddba1241fcc0ba69a850e6b8a`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 56.2 MB (56219323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2abd6d528f13cf5649363ca47e3dd5d88e430315c55ee1e826bf233b4b1d26e`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca593545a5782413367c683d2559893e498a32d71d2dec8499f06e3861baf6`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 46.3 MB (46335045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a262a30fc7feee8146227e4a6f8004ced2cfed471ce2f21fac712aa8deb7d08`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1170ff1b1e9d9726b2a806fbf4534ba0e9b7f083aa241b963a394b30107119b`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.32-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:f2a4f6141e72932f685e7a672076e3d5c7e143b7521af145b3327243b66fbd80
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.6 MB (151597491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6a0d93ee459e7bbfa6b5fbdad8d936c3d31627a9b39b4903d934f68b714d92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 22:41:06 GMT
ADD file:63b5b4161762e1845c1eb2bb2c967a07179819b4a1f12ab7596d9c6bd15c9cbd in / 
# Fri, 27 Jan 2023 22:41:06 GMT
CMD ["/bin/bash"]
# Fri, 27 Jan 2023 23:09:15 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 01:03:33 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 01:03:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 01:03:57 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 01:03:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:03:59 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 01:04:24 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 01:04:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 01:04:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:04:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 01:04:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 01:04:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 01:04:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 01:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 01:04:56 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 01:04:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26cdabfc8c6a31055d655a58d8a8f9757f43e1ce58451b8b6b02c5dd6e6d482`  
		Last Modified: Fri, 27 Jan 2023 22:42:28 GMT  
		Size: 43.5 MB (43456742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc45082a5180093f9c621428a076fbc28411899fe16d4fedc7cbc3958d407490`  
		Last Modified: Fri, 27 Jan 2023 23:11:07 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a283935394cf9ad112dfadaabd1bdf2343754a3652feb036438b2506fd859370`  
		Last Modified: Wed, 01 Feb 2023 01:05:26 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0b96316a56f812e8603b0490201e0f0f8bd5af4aa6b39f2c33781d4c060ebc`  
		Last Modified: Wed, 01 Feb 2023 01:05:25 GMT  
		Size: 4.5 MB (4470678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aefff8b7fc46c48135277e5eded9718c6b99a57586362b1acaac7dad4659e83`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdb2af2a3a435ab2d3616331ae8e9fba95e23d211b2d97ee3dc2b13cb0c0be1`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157c24da0e9d8a2f8fcaa392b46b72c5be69388be6c21e0e65c528a332da304a`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 55.6 MB (55609254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb89415e30193670069fa6526deeda86bb88de457b70aed510826aa639b2d5cc`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259d0773a9cc657509d539b1f03c4d4ad97c742e5dd220aec9a9d8d1e2534d63`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 47.1 MB (47138134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf77a02adec01c9b3a42a0508ff8eb1507bef1909da4074899de1a841c26108`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642af7c41ad7c8e5582b50d2072b296dd9c209fff84e21865dbf2994d67cf6e`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:36a7e9407344cd1cb4064179962c207cd2afb13bfbb63992f0ca328e4b56b515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:c86f3664bddd89bd539049f71c1ffc0816e18d01fad192addfb02d9e2834351c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.7 MB (177699276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33ba092bab95e48e4e7ea71d2f5e5603108185e259e011179aa03b26ad5d5067`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 06:19:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 Jan 2023 06:19:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:19:28 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 Jan 2023 06:19:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 Jan 2023 06:19:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 Jan 2023 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 06:19:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 Jan 2023 06:19:45 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 Jan 2023 21:07:31 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Tue, 17 Jan 2023 21:07:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 17 Jan 2023 21:07:48 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 17 Jan 2023 21:07:49 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 Jan 2023 21:07:49 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 17 Jan 2023 21:07:49 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 17 Jan 2023 21:07:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 17 Jan 2023 21:07:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Jan 2023 21:07:50 GMT
EXPOSE 3306 33060
# Tue, 17 Jan 2023 21:07:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d346580bcb1a6e9e1becd3883a38670cdca1f47b7cdbe65121708af5458a0318`  
		Last Modified: Wed, 11 Jan 2023 06:21:26 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec40bb6547aaa95db6bda6d1de84761264c716477d2d8b998856586285b4ec55`  
		Last Modified: Wed, 11 Jan 2023 06:21:27 GMT  
		Size: 4.4 MB (4414919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efef7c7e25176536d7c2c61700c323a83aa93894c4e3f250e6318cc77182410c`  
		Last Modified: Wed, 11 Jan 2023 06:21:25 GMT  
		Size: 1.4 MB (1418481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cd4a9c65ce2ab7c83d934277938ac0b60b14038ed82a23768c5829e04bca7f`  
		Last Modified: Wed, 11 Jan 2023 06:21:25 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4caf695f1e31c50fb977d1da7e28a7de9f4dacc6d937f16b3b2da8b263527ab`  
		Last Modified: Wed, 11 Jan 2023 06:21:28 GMT  
		Size: 12.7 MB (12662003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621837b69253e21538e7e8b097d99a96bbd14ef7c98668c7f1587a5898849f36`  
		Last Modified: Wed, 11 Jan 2023 06:21:25 GMT  
		Size: 2.5 KB (2546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c903d5cfd80f351193456503656367928154b4d6c52beb99423204b56df74`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406689e3dbcc29124df7a749b01725da213b58aea774407bdb102b0d00567b4a`  
		Last Modified: Tue, 17 Jan 2023 21:10:40 GMT  
		Size: 127.8 MB (127795859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4016832f0b21d3dbdb52cbe137c71f532d7f4515eb11a6d50e6590a5621cef82`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4236ef87c29f872eca03df1e079fbb2b174c44258b1ac06d6ccbd10a7c7efc`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedfbe312f9b4e2371da8769a8336c98cc9639575b92216f327fa63b4d034558`  
		Last Modified: Tue, 17 Jan 2023 21:10:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:3e81836557ec9ba2e151a7dbcb7ae7de732e63a22babead7afd91731aeaabf21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:cca95ddffb7c92b6c1e8da81b298a870d2f48183bebb8146d63be189ab3e37ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152665582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf3aa69f5f07d1c43c04c21627b32612760eca280ed4fe1529089a17b37b7a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:04:39 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:04:42 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:05:06 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 28 Jan 2023 00:05:07 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:05:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:05:39 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:05:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:05:40 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:06:14 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:06:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:06:15 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:06:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:06:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:06:16 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:06:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:39fbafb6c7ef40878b859fd0e4475c5ebd2ddfa8ed785a588594e8731b7cd0e8`  
		Last Modified: Fri, 27 Jan 2023 23:37:50 GMT  
		Size: 44.6 MB (44561081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e9f8ca4fd737123f9bf9fba4474d86b6e5f85291c5f9e50d2b93a1b7e83d6c`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fcdd923e548acea3ed340c20b76ef2719c0e0e6ba4408539866ba427ef9ffec`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15716fe15a39bcddcd0f7db611807ce9d4e307ee956edb69eaf5ecbac1470960`  
		Last Modified: Sat, 28 Jan 2023 00:08:20 GMT  
		Size: 4.6 MB (4611609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c8bb47c8b937c4bcf1dbebdbfd0e5bf8dd1506a3e5867d8013520b711129cf`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b050c46cac02a277087e65c3221fd4a43580659eee0590540567fd2c841491a4`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e19c22a377370b121755f4ca6da19d43ad931cddba1241fcc0ba69a850e6b8a`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 56.2 MB (56219323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2abd6d528f13cf5649363ca47e3dd5d88e430315c55ee1e826bf233b4b1d26e`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca593545a5782413367c683d2559893e498a32d71d2dec8499f06e3861baf6`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 46.3 MB (46335045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a262a30fc7feee8146227e4a6f8004ced2cfed471ce2f21fac712aa8deb7d08`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1170ff1b1e9d9726b2a806fbf4534ba0e9b7f083aa241b963a394b30107119b`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:f2a4f6141e72932f685e7a672076e3d5c7e143b7521af145b3327243b66fbd80
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.6 MB (151597491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6a0d93ee459e7bbfa6b5fbdad8d936c3d31627a9b39b4903d934f68b714d92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 22:41:06 GMT
ADD file:63b5b4161762e1845c1eb2bb2c967a07179819b4a1f12ab7596d9c6bd15c9cbd in / 
# Fri, 27 Jan 2023 22:41:06 GMT
CMD ["/bin/bash"]
# Fri, 27 Jan 2023 23:09:15 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 01:03:33 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 01:03:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 01:03:57 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 01:03:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:03:59 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 01:04:24 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 01:04:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 01:04:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:04:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 01:04:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 01:04:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 01:04:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 01:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 01:04:56 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 01:04:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26cdabfc8c6a31055d655a58d8a8f9757f43e1ce58451b8b6b02c5dd6e6d482`  
		Last Modified: Fri, 27 Jan 2023 22:42:28 GMT  
		Size: 43.5 MB (43456742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc45082a5180093f9c621428a076fbc28411899fe16d4fedc7cbc3958d407490`  
		Last Modified: Fri, 27 Jan 2023 23:11:07 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a283935394cf9ad112dfadaabd1bdf2343754a3652feb036438b2506fd859370`  
		Last Modified: Wed, 01 Feb 2023 01:05:26 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0b96316a56f812e8603b0490201e0f0f8bd5af4aa6b39f2c33781d4c060ebc`  
		Last Modified: Wed, 01 Feb 2023 01:05:25 GMT  
		Size: 4.5 MB (4470678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aefff8b7fc46c48135277e5eded9718c6b99a57586362b1acaac7dad4659e83`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdb2af2a3a435ab2d3616331ae8e9fba95e23d211b2d97ee3dc2b13cb0c0be1`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157c24da0e9d8a2f8fcaa392b46b72c5be69388be6c21e0e65c528a332da304a`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 55.6 MB (55609254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb89415e30193670069fa6526deeda86bb88de457b70aed510826aa639b2d5cc`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259d0773a9cc657509d539b1f03c4d4ad97c742e5dd220aec9a9d8d1e2534d63`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 47.1 MB (47138134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf77a02adec01c9b3a42a0508ff8eb1507bef1909da4074899de1a841c26108`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642af7c41ad7c8e5582b50d2072b296dd9c209fff84e21865dbf2994d67cf6e`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:3e81836557ec9ba2e151a7dbcb7ae7de732e63a22babead7afd91731aeaabf21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:cca95ddffb7c92b6c1e8da81b298a870d2f48183bebb8146d63be189ab3e37ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152665582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf3aa69f5f07d1c43c04c21627b32612760eca280ed4fe1529089a17b37b7a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 28 Jan 2023 00:04:39 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 Jan 2023 00:04:42 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 Jan 2023 00:05:06 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 28 Jan 2023 00:05:07 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 28 Jan 2023 00:05:07 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:05:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 28 Jan 2023 00:05:39 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 28 Jan 2023 00:05:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 28 Jan 2023 00:05:40 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Sat, 28 Jan 2023 00:06:14 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 28 Jan 2023 00:06:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 28 Jan 2023 00:06:15 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 28 Jan 2023 00:06:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 28 Jan 2023 00:06:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 Jan 2023 00:06:16 GMT
EXPOSE 3306 33060
# Sat, 28 Jan 2023 00:06:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:39fbafb6c7ef40878b859fd0e4475c5ebd2ddfa8ed785a588594e8731b7cd0e8`  
		Last Modified: Fri, 27 Jan 2023 23:37:50 GMT  
		Size: 44.6 MB (44561081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e9f8ca4fd737123f9bf9fba4474d86b6e5f85291c5f9e50d2b93a1b7e83d6c`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fcdd923e548acea3ed340c20b76ef2719c0e0e6ba4408539866ba427ef9ffec`  
		Last Modified: Sat, 28 Jan 2023 00:08:21 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15716fe15a39bcddcd0f7db611807ce9d4e307ee956edb69eaf5ecbac1470960`  
		Last Modified: Sat, 28 Jan 2023 00:08:20 GMT  
		Size: 4.6 MB (4611609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c8bb47c8b937c4bcf1dbebdbfd0e5bf8dd1506a3e5867d8013520b711129cf`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b050c46cac02a277087e65c3221fd4a43580659eee0590540567fd2c841491a4`  
		Last Modified: Sat, 28 Jan 2023 00:08:19 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e19c22a377370b121755f4ca6da19d43ad931cddba1241fcc0ba69a850e6b8a`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 56.2 MB (56219323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2abd6d528f13cf5649363ca47e3dd5d88e430315c55ee1e826bf233b4b1d26e`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca593545a5782413367c683d2559893e498a32d71d2dec8499f06e3861baf6`  
		Last Modified: Sat, 28 Jan 2023 00:08:26 GMT  
		Size: 46.3 MB (46335045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a262a30fc7feee8146227e4a6f8004ced2cfed471ce2f21fac712aa8deb7d08`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1170ff1b1e9d9726b2a806fbf4534ba0e9b7f083aa241b963a394b30107119b`  
		Last Modified: Sat, 28 Jan 2023 00:08:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:f2a4f6141e72932f685e7a672076e3d5c7e143b7521af145b3327243b66fbd80
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.6 MB (151597491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6a0d93ee459e7bbfa6b5fbdad8d936c3d31627a9b39b4903d934f68b714d92`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 22:41:06 GMT
ADD file:63b5b4161762e1845c1eb2bb2c967a07179819b4a1f12ab7596d9c6bd15c9cbd in / 
# Fri, 27 Jan 2023 22:41:06 GMT
CMD ["/bin/bash"]
# Fri, 27 Jan 2023 23:09:15 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 01:03:33 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 01:03:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 01:03:57 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 01:03:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 01:03:58 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:03:59 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 01:04:24 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 01:04:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 01:04:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 01:04:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 01:04:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 01:04:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 01:04:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 01:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 01:04:56 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 01:04:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26cdabfc8c6a31055d655a58d8a8f9757f43e1ce58451b8b6b02c5dd6e6d482`  
		Last Modified: Fri, 27 Jan 2023 22:42:28 GMT  
		Size: 43.5 MB (43456742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc45082a5180093f9c621428a076fbc28411899fe16d4fedc7cbc3958d407490`  
		Last Modified: Fri, 27 Jan 2023 23:11:07 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a283935394cf9ad112dfadaabd1bdf2343754a3652feb036438b2506fd859370`  
		Last Modified: Wed, 01 Feb 2023 01:05:26 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0b96316a56f812e8603b0490201e0f0f8bd5af4aa6b39f2c33781d4c060ebc`  
		Last Modified: Wed, 01 Feb 2023 01:05:25 GMT  
		Size: 4.5 MB (4470678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aefff8b7fc46c48135277e5eded9718c6b99a57586362b1acaac7dad4659e83`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdb2af2a3a435ab2d3616331ae8e9fba95e23d211b2d97ee3dc2b13cb0c0be1`  
		Last Modified: Wed, 01 Feb 2023 01:05:24 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157c24da0e9d8a2f8fcaa392b46b72c5be69388be6c21e0e65c528a332da304a`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 55.6 MB (55609254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb89415e30193670069fa6526deeda86bb88de457b70aed510826aa639b2d5cc`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259d0773a9cc657509d539b1f03c4d4ad97c742e5dd220aec9a9d8d1e2534d63`  
		Last Modified: Wed, 01 Feb 2023 01:05:29 GMT  
		Size: 47.1 MB (47138134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf77a02adec01c9b3a42a0508ff8eb1507bef1909da4074899de1a841c26108`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c642af7c41ad7c8e5582b50d2072b296dd9c209fff84e21865dbf2994d67cf6e`  
		Last Modified: Wed, 01 Feb 2023 01:05:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
