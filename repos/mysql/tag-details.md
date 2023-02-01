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
$ docker pull mysql@sha256:8cf035b14977b26f4a47d98e85949a7dd35e641f88fc24aa4b466b36beecf9d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:6b5917f3cfc5920881d728c19f5e3a035a06257cf5f983b1203962327d21ac66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129975079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be16cf2d832a9a54ce42144e25f5ae7cc66bccf0e003837e7b5eb1a455dc742b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:36 GMT
ADD file:eefc8abcbb6ec3141573da12cc99f3d9592d5a0bd105bb189e0e1db15c0d1bf5 in / 
# Fri, 27 Jan 2023 23:36:37 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:06:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:23:51 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:23:54 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:24:12 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 01 Feb 2023 04:24:13 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:24:13 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 01 Feb 2023 04:24:13 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Wed, 01 Feb 2023 04:24:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:24:32 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:24:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:24:33 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Wed, 01 Feb 2023 04:24:56 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:24:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:24:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:24:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:24:58 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:24:58 GMT
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
	-	`sha256:351a550f260d7de0e214367bed3a1660746ddbf80330881ee0aeba5b5505c2cb`  
		Last Modified: Wed, 01 Feb 2023 04:27:18 GMT  
		Size: 983.7 KB (983714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce196d9d34faa9d0fd3ee95a6db615d2dcf9a01d641373b50ca9060f41c6750`  
		Last Modified: Wed, 01 Feb 2023 04:27:17 GMT  
		Size: 4.5 MB (4542168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17febb6f203083f20aed59a57deb5f1a5e7b24b21166912e82c41686608ae27f`  
		Last Modified: Wed, 01 Feb 2023 04:27:16 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e426841fb4f39098843fbfe51841e7325df410b6abbe5141f6db916832ab7b`  
		Last Modified: Wed, 01 Feb 2023 04:27:16 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda41038b9f8db87281de8e62ff6f6a99413d17be72234806465069152c30296`  
		Last Modified: Wed, 01 Feb 2023 04:27:18 GMT  
		Size: 25.5 MB (25525352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47aac56b41be2f4420a90abd519b0642d7dc0f15ae013f05eb049265312d039`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a90c36973704783547f014c19a92adebbfe0af84a414eb94123a40ae0a8986`  
		Last Modified: Wed, 01 Feb 2023 04:27:23 GMT  
		Size: 48.4 MB (48447571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97091252395b2a7d7d6abfe03cee67308af5b10836f6d1a1d9a290086369e8cf`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fac29d61e98e5bb41d2e3b7897427e7a66ff35d3ecd3cbee0e41d3d8ae142f`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:1a74dd3703a9e08a4f86f2f3ca0fc5c583ed70d14ce51c0810214a49a9356728
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ceeb9aae2f08123530c07c9892ee07fef679cd385dc12de67945100c327c9d2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162697097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdc0da91e4b1905ceb995dd7a40aedb53ff2a547121bebcfc9958a0963e7401c`
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
# Wed, 01 Feb 2023 04:25:01 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:25:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:25:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Feb 2023 04:25:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 04:25:23 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:25:23 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 01 Feb 2023 04:25:23 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Wed, 01 Feb 2023 04:25:24 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Feb 2023 04:25:42 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Feb 2023 04:25:43 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:25:43 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:25:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:25:44 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:25:44 GMT
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
	-	`sha256:ce23bd8e19cbf46dca11c58364da8cae841721eb6ec6e59b5b64366b92b71c60`  
		Last Modified: Wed, 01 Feb 2023 04:27:43 GMT  
		Size: 1.4 MB (1441737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f410a04b48d8f13ee66006c76284a85219773b56a7a3917c7278e76910d15b`  
		Last Modified: Wed, 01 Feb 2023 04:27:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9d2a4035b33745414d5b00e226fd586f1b79b41c922746a2950ec302854714`  
		Last Modified: Wed, 01 Feb 2023 04:27:45 GMT  
		Size: 14.1 MB (14089526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d914f26e38d92043c13c7ac16c4034ee50d83195ac73832cde6ba5cb7c74dd7`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b578ab58d644b756e0807fcff7ca7d3875dd58ce88ae3f3ec826285f18df1e1a`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e9911a3a0f7bf66493311483809b24e311912328abd044d7374e0a1c7005d3`  
		Last Modified: Wed, 01 Feb 2023 04:27:56 GMT  
		Size: 115.8 MB (115833016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5516c1cc32a00e699d90cbafb5aec186382a49ff7862ad1c077ec3623beb1c`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb4433c89ce7ae2f55ea90016bc0c183373fbbb78ab19257b0b753e8cdca160`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:8cf035b14977b26f4a47d98e85949a7dd35e641f88fc24aa4b466b36beecf9d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:6b5917f3cfc5920881d728c19f5e3a035a06257cf5f983b1203962327d21ac66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129975079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be16cf2d832a9a54ce42144e25f5ae7cc66bccf0e003837e7b5eb1a455dc742b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:36 GMT
ADD file:eefc8abcbb6ec3141573da12cc99f3d9592d5a0bd105bb189e0e1db15c0d1bf5 in / 
# Fri, 27 Jan 2023 23:36:37 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:06:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:23:51 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:23:54 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:24:12 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 01 Feb 2023 04:24:13 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:24:13 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 01 Feb 2023 04:24:13 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Wed, 01 Feb 2023 04:24:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:24:32 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:24:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:24:33 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Wed, 01 Feb 2023 04:24:56 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:24:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:24:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:24:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:24:58 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:24:58 GMT
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
	-	`sha256:351a550f260d7de0e214367bed3a1660746ddbf80330881ee0aeba5b5505c2cb`  
		Last Modified: Wed, 01 Feb 2023 04:27:18 GMT  
		Size: 983.7 KB (983714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce196d9d34faa9d0fd3ee95a6db615d2dcf9a01d641373b50ca9060f41c6750`  
		Last Modified: Wed, 01 Feb 2023 04:27:17 GMT  
		Size: 4.5 MB (4542168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17febb6f203083f20aed59a57deb5f1a5e7b24b21166912e82c41686608ae27f`  
		Last Modified: Wed, 01 Feb 2023 04:27:16 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e426841fb4f39098843fbfe51841e7325df410b6abbe5141f6db916832ab7b`  
		Last Modified: Wed, 01 Feb 2023 04:27:16 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda41038b9f8db87281de8e62ff6f6a99413d17be72234806465069152c30296`  
		Last Modified: Wed, 01 Feb 2023 04:27:18 GMT  
		Size: 25.5 MB (25525352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47aac56b41be2f4420a90abd519b0642d7dc0f15ae013f05eb049265312d039`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a90c36973704783547f014c19a92adebbfe0af84a414eb94123a40ae0a8986`  
		Last Modified: Wed, 01 Feb 2023 04:27:23 GMT  
		Size: 48.4 MB (48447571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97091252395b2a7d7d6abfe03cee67308af5b10836f6d1a1d9a290086369e8cf`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fac29d61e98e5bb41d2e3b7897427e7a66ff35d3ecd3cbee0e41d3d8ae142f`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:8cf035b14977b26f4a47d98e85949a7dd35e641f88fc24aa4b466b36beecf9d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:6b5917f3cfc5920881d728c19f5e3a035a06257cf5f983b1203962327d21ac66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129975079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be16cf2d832a9a54ce42144e25f5ae7cc66bccf0e003837e7b5eb1a455dc742b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:36 GMT
ADD file:eefc8abcbb6ec3141573da12cc99f3d9592d5a0bd105bb189e0e1db15c0d1bf5 in / 
# Fri, 27 Jan 2023 23:36:37 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:06:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:23:51 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:23:54 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:24:12 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 01 Feb 2023 04:24:13 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:24:13 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 01 Feb 2023 04:24:13 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Wed, 01 Feb 2023 04:24:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:24:32 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:24:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:24:33 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Wed, 01 Feb 2023 04:24:56 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:24:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:24:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:24:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:24:58 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:24:58 GMT
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
	-	`sha256:351a550f260d7de0e214367bed3a1660746ddbf80330881ee0aeba5b5505c2cb`  
		Last Modified: Wed, 01 Feb 2023 04:27:18 GMT  
		Size: 983.7 KB (983714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce196d9d34faa9d0fd3ee95a6db615d2dcf9a01d641373b50ca9060f41c6750`  
		Last Modified: Wed, 01 Feb 2023 04:27:17 GMT  
		Size: 4.5 MB (4542168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17febb6f203083f20aed59a57deb5f1a5e7b24b21166912e82c41686608ae27f`  
		Last Modified: Wed, 01 Feb 2023 04:27:16 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e426841fb4f39098843fbfe51841e7325df410b6abbe5141f6db916832ab7b`  
		Last Modified: Wed, 01 Feb 2023 04:27:16 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda41038b9f8db87281de8e62ff6f6a99413d17be72234806465069152c30296`  
		Last Modified: Wed, 01 Feb 2023 04:27:18 GMT  
		Size: 25.5 MB (25525352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47aac56b41be2f4420a90abd519b0642d7dc0f15ae013f05eb049265312d039`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a90c36973704783547f014c19a92adebbfe0af84a414eb94123a40ae0a8986`  
		Last Modified: Wed, 01 Feb 2023 04:27:23 GMT  
		Size: 48.4 MB (48447571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97091252395b2a7d7d6abfe03cee67308af5b10836f6d1a1d9a290086369e8cf`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fac29d61e98e5bb41d2e3b7897427e7a66ff35d3ecd3cbee0e41d3d8ae142f`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:1a74dd3703a9e08a4f86f2f3ca0fc5c583ed70d14ce51c0810214a49a9356728
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ceeb9aae2f08123530c07c9892ee07fef679cd385dc12de67945100c327c9d2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162697097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdc0da91e4b1905ceb995dd7a40aedb53ff2a547121bebcfc9958a0963e7401c`
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
# Wed, 01 Feb 2023 04:25:01 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:25:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:25:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Feb 2023 04:25:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 04:25:23 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:25:23 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 01 Feb 2023 04:25:23 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Wed, 01 Feb 2023 04:25:24 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Feb 2023 04:25:42 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Feb 2023 04:25:43 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:25:43 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:25:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:25:44 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:25:44 GMT
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
	-	`sha256:ce23bd8e19cbf46dca11c58364da8cae841721eb6ec6e59b5b64366b92b71c60`  
		Last Modified: Wed, 01 Feb 2023 04:27:43 GMT  
		Size: 1.4 MB (1441737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f410a04b48d8f13ee66006c76284a85219773b56a7a3917c7278e76910d15b`  
		Last Modified: Wed, 01 Feb 2023 04:27:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9d2a4035b33745414d5b00e226fd586f1b79b41c922746a2950ec302854714`  
		Last Modified: Wed, 01 Feb 2023 04:27:45 GMT  
		Size: 14.1 MB (14089526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d914f26e38d92043c13c7ac16c4034ee50d83195ac73832cde6ba5cb7c74dd7`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b578ab58d644b756e0807fcff7ca7d3875dd58ce88ae3f3ec826285f18df1e1a`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e9911a3a0f7bf66493311483809b24e311912328abd044d7374e0a1c7005d3`  
		Last Modified: Wed, 01 Feb 2023 04:27:56 GMT  
		Size: 115.8 MB (115833016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5516c1cc32a00e699d90cbafb5aec186382a49ff7862ad1c077ec3623beb1c`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb4433c89ce7ae2f55ea90016bc0c183373fbbb78ab19257b0b753e8cdca160`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:8cf035b14977b26f4a47d98e85949a7dd35e641f88fc24aa4b466b36beecf9d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:6b5917f3cfc5920881d728c19f5e3a035a06257cf5f983b1203962327d21ac66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129975079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be16cf2d832a9a54ce42144e25f5ae7cc66bccf0e003837e7b5eb1a455dc742b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:36 GMT
ADD file:eefc8abcbb6ec3141573da12cc99f3d9592d5a0bd105bb189e0e1db15c0d1bf5 in / 
# Fri, 27 Jan 2023 23:36:37 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:06:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:23:51 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:23:54 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:24:12 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 01 Feb 2023 04:24:13 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:24:13 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 01 Feb 2023 04:24:13 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Wed, 01 Feb 2023 04:24:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:24:32 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:24:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:24:33 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Wed, 01 Feb 2023 04:24:56 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:24:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:24:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:24:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:24:58 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:24:58 GMT
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
	-	`sha256:351a550f260d7de0e214367bed3a1660746ddbf80330881ee0aeba5b5505c2cb`  
		Last Modified: Wed, 01 Feb 2023 04:27:18 GMT  
		Size: 983.7 KB (983714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce196d9d34faa9d0fd3ee95a6db615d2dcf9a01d641373b50ca9060f41c6750`  
		Last Modified: Wed, 01 Feb 2023 04:27:17 GMT  
		Size: 4.5 MB (4542168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17febb6f203083f20aed59a57deb5f1a5e7b24b21166912e82c41686608ae27f`  
		Last Modified: Wed, 01 Feb 2023 04:27:16 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e426841fb4f39098843fbfe51841e7325df410b6abbe5141f6db916832ab7b`  
		Last Modified: Wed, 01 Feb 2023 04:27:16 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda41038b9f8db87281de8e62ff6f6a99413d17be72234806465069152c30296`  
		Last Modified: Wed, 01 Feb 2023 04:27:18 GMT  
		Size: 25.5 MB (25525352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47aac56b41be2f4420a90abd519b0642d7dc0f15ae013f05eb049265312d039`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a90c36973704783547f014c19a92adebbfe0af84a414eb94123a40ae0a8986`  
		Last Modified: Wed, 01 Feb 2023 04:27:23 GMT  
		Size: 48.4 MB (48447571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97091252395b2a7d7d6abfe03cee67308af5b10836f6d1a1d9a290086369e8cf`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fac29d61e98e5bb41d2e3b7897427e7a66ff35d3ecd3cbee0e41d3d8ae142f`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.41`

```console
$ docker pull mysql@sha256:8cf035b14977b26f4a47d98e85949a7dd35e641f88fc24aa4b466b36beecf9d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.41` - linux; amd64

```console
$ docker pull mysql@sha256:6b5917f3cfc5920881d728c19f5e3a035a06257cf5f983b1203962327d21ac66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129975079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be16cf2d832a9a54ce42144e25f5ae7cc66bccf0e003837e7b5eb1a455dc742b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:36 GMT
ADD file:eefc8abcbb6ec3141573da12cc99f3d9592d5a0bd105bb189e0e1db15c0d1bf5 in / 
# Fri, 27 Jan 2023 23:36:37 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:06:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:23:51 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:23:54 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:24:12 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 01 Feb 2023 04:24:13 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:24:13 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 01 Feb 2023 04:24:13 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Wed, 01 Feb 2023 04:24:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:24:32 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:24:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:24:33 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Wed, 01 Feb 2023 04:24:56 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:24:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:24:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:24:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:24:58 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:24:58 GMT
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
	-	`sha256:351a550f260d7de0e214367bed3a1660746ddbf80330881ee0aeba5b5505c2cb`  
		Last Modified: Wed, 01 Feb 2023 04:27:18 GMT  
		Size: 983.7 KB (983714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce196d9d34faa9d0fd3ee95a6db615d2dcf9a01d641373b50ca9060f41c6750`  
		Last Modified: Wed, 01 Feb 2023 04:27:17 GMT  
		Size: 4.5 MB (4542168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17febb6f203083f20aed59a57deb5f1a5e7b24b21166912e82c41686608ae27f`  
		Last Modified: Wed, 01 Feb 2023 04:27:16 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e426841fb4f39098843fbfe51841e7325df410b6abbe5141f6db916832ab7b`  
		Last Modified: Wed, 01 Feb 2023 04:27:16 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda41038b9f8db87281de8e62ff6f6a99413d17be72234806465069152c30296`  
		Last Modified: Wed, 01 Feb 2023 04:27:18 GMT  
		Size: 25.5 MB (25525352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47aac56b41be2f4420a90abd519b0642d7dc0f15ae013f05eb049265312d039`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a90c36973704783547f014c19a92adebbfe0af84a414eb94123a40ae0a8986`  
		Last Modified: Wed, 01 Feb 2023 04:27:23 GMT  
		Size: 48.4 MB (48447571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97091252395b2a7d7d6abfe03cee67308af5b10836f6d1a1d9a290086369e8cf`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fac29d61e98e5bb41d2e3b7897427e7a66ff35d3ecd3cbee0e41d3d8ae142f`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.41-debian`

```console
$ docker pull mysql@sha256:1a74dd3703a9e08a4f86f2f3ca0fc5c583ed70d14ce51c0810214a49a9356728
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.41-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ceeb9aae2f08123530c07c9892ee07fef679cd385dc12de67945100c327c9d2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162697097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdc0da91e4b1905ceb995dd7a40aedb53ff2a547121bebcfc9958a0963e7401c`
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
# Wed, 01 Feb 2023 04:25:01 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:25:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:25:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Feb 2023 04:25:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 04:25:23 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:25:23 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 01 Feb 2023 04:25:23 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Wed, 01 Feb 2023 04:25:24 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Feb 2023 04:25:42 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Feb 2023 04:25:43 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:25:43 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:25:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:25:44 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:25:44 GMT
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
	-	`sha256:ce23bd8e19cbf46dca11c58364da8cae841721eb6ec6e59b5b64366b92b71c60`  
		Last Modified: Wed, 01 Feb 2023 04:27:43 GMT  
		Size: 1.4 MB (1441737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f410a04b48d8f13ee66006c76284a85219773b56a7a3917c7278e76910d15b`  
		Last Modified: Wed, 01 Feb 2023 04:27:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9d2a4035b33745414d5b00e226fd586f1b79b41c922746a2950ec302854714`  
		Last Modified: Wed, 01 Feb 2023 04:27:45 GMT  
		Size: 14.1 MB (14089526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d914f26e38d92043c13c7ac16c4034ee50d83195ac73832cde6ba5cb7c74dd7`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b578ab58d644b756e0807fcff7ca7d3875dd58ce88ae3f3ec826285f18df1e1a`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e9911a3a0f7bf66493311483809b24e311912328abd044d7374e0a1c7005d3`  
		Last Modified: Wed, 01 Feb 2023 04:27:56 GMT  
		Size: 115.8 MB (115833016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5516c1cc32a00e699d90cbafb5aec186382a49ff7862ad1c077ec3623beb1c`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb4433c89ce7ae2f55ea90016bc0c183373fbbb78ab19257b0b753e8cdca160`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.41-oracle`

```console
$ docker pull mysql@sha256:8cf035b14977b26f4a47d98e85949a7dd35e641f88fc24aa4b466b36beecf9d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.41-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:6b5917f3cfc5920881d728c19f5e3a035a06257cf5f983b1203962327d21ac66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129975079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be16cf2d832a9a54ce42144e25f5ae7cc66bccf0e003837e7b5eb1a455dc742b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:36 GMT
ADD file:eefc8abcbb6ec3141573da12cc99f3d9592d5a0bd105bb189e0e1db15c0d1bf5 in / 
# Fri, 27 Jan 2023 23:36:37 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:06:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:23:51 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:23:54 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:24:12 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 01 Feb 2023 04:24:13 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:24:13 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 01 Feb 2023 04:24:13 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Wed, 01 Feb 2023 04:24:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:24:32 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:24:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:24:33 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Wed, 01 Feb 2023 04:24:56 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:24:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:24:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:24:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:24:58 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:24:58 GMT
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
	-	`sha256:351a550f260d7de0e214367bed3a1660746ddbf80330881ee0aeba5b5505c2cb`  
		Last Modified: Wed, 01 Feb 2023 04:27:18 GMT  
		Size: 983.7 KB (983714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce196d9d34faa9d0fd3ee95a6db615d2dcf9a01d641373b50ca9060f41c6750`  
		Last Modified: Wed, 01 Feb 2023 04:27:17 GMT  
		Size: 4.5 MB (4542168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17febb6f203083f20aed59a57deb5f1a5e7b24b21166912e82c41686608ae27f`  
		Last Modified: Wed, 01 Feb 2023 04:27:16 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e426841fb4f39098843fbfe51841e7325df410b6abbe5141f6db916832ab7b`  
		Last Modified: Wed, 01 Feb 2023 04:27:16 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda41038b9f8db87281de8e62ff6f6a99413d17be72234806465069152c30296`  
		Last Modified: Wed, 01 Feb 2023 04:27:18 GMT  
		Size: 25.5 MB (25525352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47aac56b41be2f4420a90abd519b0642d7dc0f15ae013f05eb049265312d039`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a90c36973704783547f014c19a92adebbfe0af84a414eb94123a40ae0a8986`  
		Last Modified: Wed, 01 Feb 2023 04:27:23 GMT  
		Size: 48.4 MB (48447571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97091252395b2a7d7d6abfe03cee67308af5b10836f6d1a1d9a290086369e8cf`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fac29d61e98e5bb41d2e3b7897427e7a66ff35d3ecd3cbee0e41d3d8ae142f`  
		Last Modified: Wed, 01 Feb 2023 04:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:03b0af22f4df273a2b7bb6320ca305f9e0dcaebe411a1ec75e6adc9fea051aa2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:5084e15154ea2784784ddc05b92cc9f5074c1b2d4dcc815acdd8ad6b98afaeb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152719332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b458cc32b9686508b97ef40043702c18572840f7b2936b14f06500363868ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:21:18 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:21:23 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:21:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 04:21:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:21:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 04:21:49 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:21:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:22:20 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:22:21 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:22:21 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:22:55 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:22:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:22:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:22:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:22:57 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:22:58 GMT
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
	-	`sha256:3898be77c3954d22c2f349e290c066493612a19abcfc8c83e7ba275cc8a62fac`  
		Last Modified: Wed, 01 Feb 2023 04:26:13 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992f720677b1866a4573e0cf0b8ba5a4d0193c7988e72773b0a3f5082bbf409c`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 4.6 MB (4611652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b298d35e4a8f2cbd4b6267c687442dd5a1f9619656379fb0b48d87cd9c48ecd`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a7ae1e6628b2acd04866555f5025df3712a209decb24be0256da88b599c36e`  
		Last Modified: Wed, 01 Feb 2023 04:26:11 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9501ab7b660850b049d420b9e3689078f6a5af4f9c0cfb1d00c86bb2026372e9`  
		Last Modified: Wed, 01 Feb 2023 04:26:18 GMT  
		Size: 56.2 MB (56219492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d00a593dfefa14724dab0ddb74e263abdef9483b694e9b46c75e80635364f3`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a5c1244ef5a2b05ac1fdc05bd84a9988c3351e4d1c520938649de0686e12ad`  
		Last Modified: Wed, 01 Feb 2023 04:26:19 GMT  
		Size: 46.3 MB (46334606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec08e11879d6796aad1aa331ccf9c7523fbdbac20a573a0258036d0ccc379615`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dbf0a1ea0ea5aa7204ad7aecd2c49549497864236ea6c7071ac63d9582ded5`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
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
$ docker pull mysql@sha256:e426ff0829f7154112db90188b72f1c6df89b7b08f0267dd61cb40a73f52249e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:5b6ae6c429fe3c44602dbe8e4ebdf5c8032dd55ef42348b56debd4839eed67c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177752106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f35f77c020077887152d702bf1c8ee24717a2dcb60b11d918304e2e1d8e92b1`
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
# Wed, 01 Feb 2023 04:23:11 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:23:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Feb 2023 04:23:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 04:23:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:23:27 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 04:23:27 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Wed, 01 Feb 2023 04:23:27 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Feb 2023 04:23:43 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Feb 2023 04:23:44 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:23:44 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 01 Feb 2023 04:23:44 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:23:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:23:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:23:45 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:23:45 GMT
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
	-	`sha256:55073b6088ddd1c49ce8b315787bffbb76b9df8815542c17f216663df0337048`  
		Last Modified: Wed, 01 Feb 2023 04:26:44 GMT  
		Size: 1.5 MB (1471344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992a58a5e822d4e74f26952dc6e3ff0d3dd3e46bb574d8606a773260f0e3fa36`  
		Last Modified: Wed, 01 Feb 2023 04:26:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e678974251861a18dd7f9946ab2ca2f8df5d4c6d4a6dfc60ac2c8f60f39ecc`  
		Last Modified: Wed, 01 Feb 2023 04:26:46 GMT  
		Size: 12.7 MB (12662057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f11138713f04620178141d71bd4f423e7a85ea913b6cf6af2b9d87e8a1474a`  
		Last Modified: Wed, 01 Feb 2023 04:26:43 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1038c91480f031ca1f0d220840ed4c2fffcd373b23585dddf6a74b0c9dc57ff9`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5d09a55ff559567fcbac3fa0aaa67b2de8900d68b432d1d44447f4283ff210`  
		Last Modified: Wed, 01 Feb 2023 04:27:01 GMT  
		Size: 127.8 MB (127795777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d76f3aa57a316ba1b23b1efa8236bfef201cf2125a1ed4b25b9560a034b5f`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfac894faa8a253e7de1a31c4a08ab0e6367235330487c14ea97781076573ec`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0851a22955c6ed197f114610146bc4dc92cf620093cf93d14e6728d8880d91fc`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:03b0af22f4df273a2b7bb6320ca305f9e0dcaebe411a1ec75e6adc9fea051aa2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:5084e15154ea2784784ddc05b92cc9f5074c1b2d4dcc815acdd8ad6b98afaeb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152719332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b458cc32b9686508b97ef40043702c18572840f7b2936b14f06500363868ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:21:18 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:21:23 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:21:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 04:21:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:21:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 04:21:49 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:21:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:22:20 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:22:21 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:22:21 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:22:55 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:22:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:22:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:22:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:22:57 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:22:58 GMT
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
	-	`sha256:3898be77c3954d22c2f349e290c066493612a19abcfc8c83e7ba275cc8a62fac`  
		Last Modified: Wed, 01 Feb 2023 04:26:13 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992f720677b1866a4573e0cf0b8ba5a4d0193c7988e72773b0a3f5082bbf409c`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 4.6 MB (4611652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b298d35e4a8f2cbd4b6267c687442dd5a1f9619656379fb0b48d87cd9c48ecd`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a7ae1e6628b2acd04866555f5025df3712a209decb24be0256da88b599c36e`  
		Last Modified: Wed, 01 Feb 2023 04:26:11 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9501ab7b660850b049d420b9e3689078f6a5af4f9c0cfb1d00c86bb2026372e9`  
		Last Modified: Wed, 01 Feb 2023 04:26:18 GMT  
		Size: 56.2 MB (56219492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d00a593dfefa14724dab0ddb74e263abdef9483b694e9b46c75e80635364f3`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a5c1244ef5a2b05ac1fdc05bd84a9988c3351e4d1c520938649de0686e12ad`  
		Last Modified: Wed, 01 Feb 2023 04:26:19 GMT  
		Size: 46.3 MB (46334606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec08e11879d6796aad1aa331ccf9c7523fbdbac20a573a0258036d0ccc379615`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dbf0a1ea0ea5aa7204ad7aecd2c49549497864236ea6c7071ac63d9582ded5`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
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
$ docker pull mysql@sha256:03b0af22f4df273a2b7bb6320ca305f9e0dcaebe411a1ec75e6adc9fea051aa2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:5084e15154ea2784784ddc05b92cc9f5074c1b2d4dcc815acdd8ad6b98afaeb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152719332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b458cc32b9686508b97ef40043702c18572840f7b2936b14f06500363868ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:21:18 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:21:23 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:21:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 04:21:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:21:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 04:21:49 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:21:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:22:20 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:22:21 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:22:21 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:22:55 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:22:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:22:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:22:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:22:57 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:22:58 GMT
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
	-	`sha256:3898be77c3954d22c2f349e290c066493612a19abcfc8c83e7ba275cc8a62fac`  
		Last Modified: Wed, 01 Feb 2023 04:26:13 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992f720677b1866a4573e0cf0b8ba5a4d0193c7988e72773b0a3f5082bbf409c`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 4.6 MB (4611652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b298d35e4a8f2cbd4b6267c687442dd5a1f9619656379fb0b48d87cd9c48ecd`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a7ae1e6628b2acd04866555f5025df3712a209decb24be0256da88b599c36e`  
		Last Modified: Wed, 01 Feb 2023 04:26:11 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9501ab7b660850b049d420b9e3689078f6a5af4f9c0cfb1d00c86bb2026372e9`  
		Last Modified: Wed, 01 Feb 2023 04:26:18 GMT  
		Size: 56.2 MB (56219492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d00a593dfefa14724dab0ddb74e263abdef9483b694e9b46c75e80635364f3`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a5c1244ef5a2b05ac1fdc05bd84a9988c3351e4d1c520938649de0686e12ad`  
		Last Modified: Wed, 01 Feb 2023 04:26:19 GMT  
		Size: 46.3 MB (46334606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec08e11879d6796aad1aa331ccf9c7523fbdbac20a573a0258036d0ccc379615`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dbf0a1ea0ea5aa7204ad7aecd2c49549497864236ea6c7071ac63d9582ded5`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
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
$ docker pull mysql@sha256:e426ff0829f7154112db90188b72f1c6df89b7b08f0267dd61cb40a73f52249e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:5b6ae6c429fe3c44602dbe8e4ebdf5c8032dd55ef42348b56debd4839eed67c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177752106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f35f77c020077887152d702bf1c8ee24717a2dcb60b11d918304e2e1d8e92b1`
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
# Wed, 01 Feb 2023 04:23:11 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:23:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Feb 2023 04:23:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 04:23:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:23:27 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 04:23:27 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Wed, 01 Feb 2023 04:23:27 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Feb 2023 04:23:43 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Feb 2023 04:23:44 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:23:44 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 01 Feb 2023 04:23:44 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:23:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:23:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:23:45 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:23:45 GMT
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
	-	`sha256:55073b6088ddd1c49ce8b315787bffbb76b9df8815542c17f216663df0337048`  
		Last Modified: Wed, 01 Feb 2023 04:26:44 GMT  
		Size: 1.5 MB (1471344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992a58a5e822d4e74f26952dc6e3ff0d3dd3e46bb574d8606a773260f0e3fa36`  
		Last Modified: Wed, 01 Feb 2023 04:26:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e678974251861a18dd7f9946ab2ca2f8df5d4c6d4a6dfc60ac2c8f60f39ecc`  
		Last Modified: Wed, 01 Feb 2023 04:26:46 GMT  
		Size: 12.7 MB (12662057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f11138713f04620178141d71bd4f423e7a85ea913b6cf6af2b9d87e8a1474a`  
		Last Modified: Wed, 01 Feb 2023 04:26:43 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1038c91480f031ca1f0d220840ed4c2fffcd373b23585dddf6a74b0c9dc57ff9`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5d09a55ff559567fcbac3fa0aaa67b2de8900d68b432d1d44447f4283ff210`  
		Last Modified: Wed, 01 Feb 2023 04:27:01 GMT  
		Size: 127.8 MB (127795777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d76f3aa57a316ba1b23b1efa8236bfef201cf2125a1ed4b25b9560a034b5f`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfac894faa8a253e7de1a31c4a08ab0e6367235330487c14ea97781076573ec`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0851a22955c6ed197f114610146bc4dc92cf620093cf93d14e6728d8880d91fc`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:03b0af22f4df273a2b7bb6320ca305f9e0dcaebe411a1ec75e6adc9fea051aa2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:5084e15154ea2784784ddc05b92cc9f5074c1b2d4dcc815acdd8ad6b98afaeb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152719332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b458cc32b9686508b97ef40043702c18572840f7b2936b14f06500363868ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:21:18 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:21:23 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:21:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 04:21:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:21:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 04:21:49 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:21:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:22:20 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:22:21 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:22:21 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:22:55 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:22:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:22:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:22:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:22:57 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:22:58 GMT
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
	-	`sha256:3898be77c3954d22c2f349e290c066493612a19abcfc8c83e7ba275cc8a62fac`  
		Last Modified: Wed, 01 Feb 2023 04:26:13 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992f720677b1866a4573e0cf0b8ba5a4d0193c7988e72773b0a3f5082bbf409c`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 4.6 MB (4611652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b298d35e4a8f2cbd4b6267c687442dd5a1f9619656379fb0b48d87cd9c48ecd`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a7ae1e6628b2acd04866555f5025df3712a209decb24be0256da88b599c36e`  
		Last Modified: Wed, 01 Feb 2023 04:26:11 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9501ab7b660850b049d420b9e3689078f6a5af4f9c0cfb1d00c86bb2026372e9`  
		Last Modified: Wed, 01 Feb 2023 04:26:18 GMT  
		Size: 56.2 MB (56219492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d00a593dfefa14724dab0ddb74e263abdef9483b694e9b46c75e80635364f3`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a5c1244ef5a2b05ac1fdc05bd84a9988c3351e4d1c520938649de0686e12ad`  
		Last Modified: Wed, 01 Feb 2023 04:26:19 GMT  
		Size: 46.3 MB (46334606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec08e11879d6796aad1aa331ccf9c7523fbdbac20a573a0258036d0ccc379615`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dbf0a1ea0ea5aa7204ad7aecd2c49549497864236ea6c7071ac63d9582ded5`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
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
$ docker pull mysql@sha256:03b0af22f4df273a2b7bb6320ca305f9e0dcaebe411a1ec75e6adc9fea051aa2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.32` - linux; amd64

```console
$ docker pull mysql@sha256:5084e15154ea2784784ddc05b92cc9f5074c1b2d4dcc815acdd8ad6b98afaeb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152719332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b458cc32b9686508b97ef40043702c18572840f7b2936b14f06500363868ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:21:18 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:21:23 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:21:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 04:21:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:21:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 04:21:49 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:21:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:22:20 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:22:21 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:22:21 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:22:55 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:22:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:22:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:22:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:22:57 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:22:58 GMT
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
	-	`sha256:3898be77c3954d22c2f349e290c066493612a19abcfc8c83e7ba275cc8a62fac`  
		Last Modified: Wed, 01 Feb 2023 04:26:13 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992f720677b1866a4573e0cf0b8ba5a4d0193c7988e72773b0a3f5082bbf409c`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 4.6 MB (4611652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b298d35e4a8f2cbd4b6267c687442dd5a1f9619656379fb0b48d87cd9c48ecd`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a7ae1e6628b2acd04866555f5025df3712a209decb24be0256da88b599c36e`  
		Last Modified: Wed, 01 Feb 2023 04:26:11 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9501ab7b660850b049d420b9e3689078f6a5af4f9c0cfb1d00c86bb2026372e9`  
		Last Modified: Wed, 01 Feb 2023 04:26:18 GMT  
		Size: 56.2 MB (56219492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d00a593dfefa14724dab0ddb74e263abdef9483b694e9b46c75e80635364f3`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a5c1244ef5a2b05ac1fdc05bd84a9988c3351e4d1c520938649de0686e12ad`  
		Last Modified: Wed, 01 Feb 2023 04:26:19 GMT  
		Size: 46.3 MB (46334606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec08e11879d6796aad1aa331ccf9c7523fbdbac20a573a0258036d0ccc379615`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dbf0a1ea0ea5aa7204ad7aecd2c49549497864236ea6c7071ac63d9582ded5`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
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
$ docker pull mysql@sha256:e426ff0829f7154112db90188b72f1c6df89b7b08f0267dd61cb40a73f52249e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.32-debian` - linux; amd64

```console
$ docker pull mysql@sha256:5b6ae6c429fe3c44602dbe8e4ebdf5c8032dd55ef42348b56debd4839eed67c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177752106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f35f77c020077887152d702bf1c8ee24717a2dcb60b11d918304e2e1d8e92b1`
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
# Wed, 01 Feb 2023 04:23:11 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:23:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Feb 2023 04:23:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 04:23:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:23:27 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 04:23:27 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Wed, 01 Feb 2023 04:23:27 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Feb 2023 04:23:43 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Feb 2023 04:23:44 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:23:44 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 01 Feb 2023 04:23:44 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:23:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:23:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:23:45 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:23:45 GMT
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
	-	`sha256:55073b6088ddd1c49ce8b315787bffbb76b9df8815542c17f216663df0337048`  
		Last Modified: Wed, 01 Feb 2023 04:26:44 GMT  
		Size: 1.5 MB (1471344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992a58a5e822d4e74f26952dc6e3ff0d3dd3e46bb574d8606a773260f0e3fa36`  
		Last Modified: Wed, 01 Feb 2023 04:26:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e678974251861a18dd7f9946ab2ca2f8df5d4c6d4a6dfc60ac2c8f60f39ecc`  
		Last Modified: Wed, 01 Feb 2023 04:26:46 GMT  
		Size: 12.7 MB (12662057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f11138713f04620178141d71bd4f423e7a85ea913b6cf6af2b9d87e8a1474a`  
		Last Modified: Wed, 01 Feb 2023 04:26:43 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1038c91480f031ca1f0d220840ed4c2fffcd373b23585dddf6a74b0c9dc57ff9`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5d09a55ff559567fcbac3fa0aaa67b2de8900d68b432d1d44447f4283ff210`  
		Last Modified: Wed, 01 Feb 2023 04:27:01 GMT  
		Size: 127.8 MB (127795777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d76f3aa57a316ba1b23b1efa8236bfef201cf2125a1ed4b25b9560a034b5f`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfac894faa8a253e7de1a31c4a08ab0e6367235330487c14ea97781076573ec`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0851a22955c6ed197f114610146bc4dc92cf620093cf93d14e6728d8880d91fc`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.32-oracle`

```console
$ docker pull mysql@sha256:03b0af22f4df273a2b7bb6320ca305f9e0dcaebe411a1ec75e6adc9fea051aa2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.32-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:5084e15154ea2784784ddc05b92cc9f5074c1b2d4dcc815acdd8ad6b98afaeb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152719332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b458cc32b9686508b97ef40043702c18572840f7b2936b14f06500363868ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:21:18 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:21:23 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:21:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 04:21:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:21:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 04:21:49 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:21:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:22:20 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:22:21 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:22:21 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:22:55 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:22:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:22:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:22:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:22:57 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:22:58 GMT
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
	-	`sha256:3898be77c3954d22c2f349e290c066493612a19abcfc8c83e7ba275cc8a62fac`  
		Last Modified: Wed, 01 Feb 2023 04:26:13 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992f720677b1866a4573e0cf0b8ba5a4d0193c7988e72773b0a3f5082bbf409c`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 4.6 MB (4611652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b298d35e4a8f2cbd4b6267c687442dd5a1f9619656379fb0b48d87cd9c48ecd`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a7ae1e6628b2acd04866555f5025df3712a209decb24be0256da88b599c36e`  
		Last Modified: Wed, 01 Feb 2023 04:26:11 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9501ab7b660850b049d420b9e3689078f6a5af4f9c0cfb1d00c86bb2026372e9`  
		Last Modified: Wed, 01 Feb 2023 04:26:18 GMT  
		Size: 56.2 MB (56219492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d00a593dfefa14724dab0ddb74e263abdef9483b694e9b46c75e80635364f3`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a5c1244ef5a2b05ac1fdc05bd84a9988c3351e4d1c520938649de0686e12ad`  
		Last Modified: Wed, 01 Feb 2023 04:26:19 GMT  
		Size: 46.3 MB (46334606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec08e11879d6796aad1aa331ccf9c7523fbdbac20a573a0258036d0ccc379615`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dbf0a1ea0ea5aa7204ad7aecd2c49549497864236ea6c7071ac63d9582ded5`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
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
$ docker pull mysql@sha256:e426ff0829f7154112db90188b72f1c6df89b7b08f0267dd61cb40a73f52249e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:5b6ae6c429fe3c44602dbe8e4ebdf5c8032dd55ef42348b56debd4839eed67c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177752106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f35f77c020077887152d702bf1c8ee24717a2dcb60b11d918304e2e1d8e92b1`
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
# Wed, 01 Feb 2023 04:23:11 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:23:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:23:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Feb 2023 04:23:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 04:23:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:23:27 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 04:23:27 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Wed, 01 Feb 2023 04:23:27 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Feb 2023 04:23:43 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Feb 2023 04:23:44 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:23:44 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 01 Feb 2023 04:23:44 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:23:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:23:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:23:45 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:23:45 GMT
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
	-	`sha256:55073b6088ddd1c49ce8b315787bffbb76b9df8815542c17f216663df0337048`  
		Last Modified: Wed, 01 Feb 2023 04:26:44 GMT  
		Size: 1.5 MB (1471344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992a58a5e822d4e74f26952dc6e3ff0d3dd3e46bb574d8606a773260f0e3fa36`  
		Last Modified: Wed, 01 Feb 2023 04:26:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e678974251861a18dd7f9946ab2ca2f8df5d4c6d4a6dfc60ac2c8f60f39ecc`  
		Last Modified: Wed, 01 Feb 2023 04:26:46 GMT  
		Size: 12.7 MB (12662057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f11138713f04620178141d71bd4f423e7a85ea913b6cf6af2b9d87e8a1474a`  
		Last Modified: Wed, 01 Feb 2023 04:26:43 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1038c91480f031ca1f0d220840ed4c2fffcd373b23585dddf6a74b0c9dc57ff9`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5d09a55ff559567fcbac3fa0aaa67b2de8900d68b432d1d44447f4283ff210`  
		Last Modified: Wed, 01 Feb 2023 04:27:01 GMT  
		Size: 127.8 MB (127795777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d76f3aa57a316ba1b23b1efa8236bfef201cf2125a1ed4b25b9560a034b5f`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfac894faa8a253e7de1a31c4a08ab0e6367235330487c14ea97781076573ec`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0851a22955c6ed197f114610146bc4dc92cf620093cf93d14e6728d8880d91fc`  
		Last Modified: Wed, 01 Feb 2023 04:26:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:03b0af22f4df273a2b7bb6320ca305f9e0dcaebe411a1ec75e6adc9fea051aa2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:5084e15154ea2784784ddc05b92cc9f5074c1b2d4dcc815acdd8ad6b98afaeb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152719332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b458cc32b9686508b97ef40043702c18572840f7b2936b14f06500363868ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:21:18 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:21:23 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:21:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 04:21:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:21:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 04:21:49 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:21:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:22:20 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:22:21 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:22:21 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:22:55 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:22:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:22:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:22:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:22:57 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:22:58 GMT
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
	-	`sha256:3898be77c3954d22c2f349e290c066493612a19abcfc8c83e7ba275cc8a62fac`  
		Last Modified: Wed, 01 Feb 2023 04:26:13 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992f720677b1866a4573e0cf0b8ba5a4d0193c7988e72773b0a3f5082bbf409c`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 4.6 MB (4611652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b298d35e4a8f2cbd4b6267c687442dd5a1f9619656379fb0b48d87cd9c48ecd`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a7ae1e6628b2acd04866555f5025df3712a209decb24be0256da88b599c36e`  
		Last Modified: Wed, 01 Feb 2023 04:26:11 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9501ab7b660850b049d420b9e3689078f6a5af4f9c0cfb1d00c86bb2026372e9`  
		Last Modified: Wed, 01 Feb 2023 04:26:18 GMT  
		Size: 56.2 MB (56219492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d00a593dfefa14724dab0ddb74e263abdef9483b694e9b46c75e80635364f3`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a5c1244ef5a2b05ac1fdc05bd84a9988c3351e4d1c520938649de0686e12ad`  
		Last Modified: Wed, 01 Feb 2023 04:26:19 GMT  
		Size: 46.3 MB (46334606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec08e11879d6796aad1aa331ccf9c7523fbdbac20a573a0258036d0ccc379615`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dbf0a1ea0ea5aa7204ad7aecd2c49549497864236ea6c7071ac63d9582ded5`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
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
$ docker pull mysql@sha256:03b0af22f4df273a2b7bb6320ca305f9e0dcaebe411a1ec75e6adc9fea051aa2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:5084e15154ea2784784ddc05b92cc9f5074c1b2d4dcc815acdd8ad6b98afaeb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152719332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b458cc32b9686508b97ef40043702c18572840f7b2936b14f06500363868ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 27 Jan 2023 23:36:12 GMT
ADD file:f2aead35bfc542632b7274d3b1132eb2bb3752d6cb61414febbffb746120622c in / 
# Fri, 27 Jan 2023 23:36:13 GMT
CMD ["/bin/bash"]
# Sat, 28 Jan 2023 00:04:38 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 01 Feb 2023 04:21:18 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:21:23 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:21:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 01 Feb 2023 04:21:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:21:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Feb 2023 04:21:49 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:21:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 01 Feb 2023 04:22:20 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 01 Feb 2023 04:22:21 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 01 Feb 2023 04:22:21 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 01 Feb 2023 04:22:55 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 01 Feb 2023 04:22:57 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:22:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:22:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:22:57 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:22:58 GMT
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
	-	`sha256:3898be77c3954d22c2f349e290c066493612a19abcfc8c83e7ba275cc8a62fac`  
		Last Modified: Wed, 01 Feb 2023 04:26:13 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992f720677b1866a4573e0cf0b8ba5a4d0193c7988e72773b0a3f5082bbf409c`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 4.6 MB (4611652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b298d35e4a8f2cbd4b6267c687442dd5a1f9619656379fb0b48d87cd9c48ecd`  
		Last Modified: Wed, 01 Feb 2023 04:26:12 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a7ae1e6628b2acd04866555f5025df3712a209decb24be0256da88b599c36e`  
		Last Modified: Wed, 01 Feb 2023 04:26:11 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9501ab7b660850b049d420b9e3689078f6a5af4f9c0cfb1d00c86bb2026372e9`  
		Last Modified: Wed, 01 Feb 2023 04:26:18 GMT  
		Size: 56.2 MB (56219492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d00a593dfefa14724dab0ddb74e263abdef9483b694e9b46c75e80635364f3`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a5c1244ef5a2b05ac1fdc05bd84a9988c3351e4d1c520938649de0686e12ad`  
		Last Modified: Wed, 01 Feb 2023 04:26:19 GMT  
		Size: 46.3 MB (46334606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec08e11879d6796aad1aa331ccf9c7523fbdbac20a573a0258036d0ccc379615`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dbf0a1ea0ea5aa7204ad7aecd2c49549497864236ea6c7071ac63d9582ded5`  
		Last Modified: Wed, 01 Feb 2023 04:26:10 GMT  
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
