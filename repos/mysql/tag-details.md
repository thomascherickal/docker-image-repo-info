<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5-debian`](#mysql5-debian)
-	[`mysql:5-oracle`](#mysql5-oracle)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7-debian`](#mysql57-debian)
-	[`mysql:5.7-oracle`](#mysql57-oracle)
-	[`mysql:5.7.42`](#mysql5742)
-	[`mysql:5.7.42-debian`](#mysql5742-debian)
-	[`mysql:5.7.42-oracle`](#mysql5742-oracle)
-	[`mysql:8`](#mysql8)
-	[`mysql:8-debian`](#mysql8-debian)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0.33`](#mysql8033)
-	[`mysql:8.0.33-debian`](#mysql8033-debian)
-	[`mysql:8.0.33-oracle`](#mysql8033-oracle)
-	[`mysql:debian`](#mysqldebian)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)

## `mysql:5`

```console
$ docker pull mysql@sha256:f57eef421000aaf8332a91ab0b6c96b3c83ed2a981c29e6528b21ce10197cd16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:c4c526804552f6b4e8e124e182f5df4b09bf4bc88cba8a94adbd0a2ccb81dce6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169273935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6675b5cfea17abb655ea8229cbcfa5db9d0b041f839db0c24228c2e18a4bdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 31 Mar 2023 22:29:01 GMT
ADD file:a14b5a8b8b6993aeee5ac6052fdf283560d65365e5bcf133ab21c4756439384a in / 
# Fri, 31 Mar 2023 22:29:01 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 23:23:03 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 31 Mar 2023 23:23:04 GMT
ENV GOSU_VERSION=1.16
# Fri, 31 Mar 2023 23:23:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 31 Mar 2023 23:23:23 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 31 Mar 2023 23:23:25 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 31 Mar 2023 23:23:25 GMT
ENV MYSQL_MAJOR=5.7
# Mon, 17 Apr 2023 22:45:06 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Mon, 17 Apr 2023 22:45:06 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:45:25 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:45:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:45:25 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el7
# Mon, 17 Apr 2023 22:46:08 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:46:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:46:09 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:46:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:46:10 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:46:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e83e8f2e82cc31391cd0cb4f5ba574ba5eb9708fc0f5dcc34fef53b03ef28f31`  
		Last Modified: Fri, 31 Mar 2023 22:30:40 GMT  
		Size: 50.5 MB (50496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f23deb01b847d9dd0fc43ede2d2dacda423b95fdbf64e0ce21a6f542f6a167e`  
		Last Modified: Fri, 31 Mar 2023 23:25:04 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bda3b184ea984d363fc64e635076bcb405620effc23b2eac44f23e662bfd57`  
		Last Modified: Fri, 31 Mar 2023 23:25:05 GMT  
		Size: 983.7 KB (983706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed17edbc6604e6a5d584a08fa036d3d0711dde7676b4a6fe0adeb03b148ba5e7`  
		Last Modified: Fri, 31 Mar 2023 23:25:03 GMT  
		Size: 4.6 MB (4585198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a94a6acfa729dcf5f76be5966ecdc31692840ba7619f81d82d5e6dfc717c03`  
		Last Modified: Fri, 31 Mar 2023 23:25:02 GMT  
		Size: 2.7 KB (2653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f153bd2953e42c4994ce494be0c531c5260eb4d6623c1fd25db3bf99151456e9`  
		Last Modified: Mon, 17 Apr 2023 22:47:59 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab532edfb8133d99946879a0d39b72cdaafb249687f0cb36f2ca2251b051a9c7`  
		Last Modified: Mon, 17 Apr 2023 22:48:01 GMT  
		Size: 25.5 MB (25538322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76bdfe4f3d029057814b330ee6677a548fe964dd5822907d69680050d0003c2`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ffe2f25512b515f08ae407d0cd0e72010857d4ba8a34d0ee47279db49af6d`  
		Last Modified: Mon, 17 Apr 2023 22:48:11 GMT  
		Size: 87.7 MB (87660996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857ada4fbbcc843e4671c9029632651e1d4bd743c2f3326068ffeccb6fd795e0`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c508404c3ce0c3416a1c396965ce8b76f3719b7d2d592bfb6ac3b48f4ea20f`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:11aea01c02f457f6c67e2037caa5e004e015ee94293aac224c0beb13459ee9db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:26504dc8b79b5b0bf60d9e7e043b7a2b1a9895b390382cf7ceab3792d8aa2e34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.8 MB (162758554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f270218b50ff2e08bc03cde8f0ba99dfef35758ef84f3c93e9c64d25b027be5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:16:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 May 2023 04:16:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:16:37 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 04:16:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 04:16:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 04:16:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:16:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 04:16:52 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 23 May 2023 04:16:52 GMT
ENV MYSQL_VERSION=5.7.42-1debian10
# Tue, 23 May 2023 04:16:53 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 May 2023 04:17:12 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 May 2023 04:17:13 GMT
VOLUME [/var/lib/mysql]
# Tue, 23 May 2023 04:17:13 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 23 May 2023 04:17:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 04:17:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 04:17:14 GMT
EXPOSE 3306 33060
# Tue, 23 May 2023 04:17:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ca486d93f7aa513f34a5fadffd81c536ce4ac5de719145803c6829aea16397`  
		Last Modified: Tue, 23 May 2023 04:18:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60f1b29379d4ba9ab2dabb338ac075c86cc37e5fdfcae5ae96dbbd6457cf089`  
		Last Modified: Tue, 23 May 2023 04:18:08 GMT  
		Size: 4.2 MB (4182401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a7f35f9a601ec927d75159dea2103af466efa76425e85420e4478dd4245c24`  
		Last Modified: Tue, 23 May 2023 04:18:08 GMT  
		Size: 1.4 MB (1441855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1256d8a34742417f317fd61b3b0a979ba9899c2a1fe1a41e0af44e91540db169`  
		Last Modified: Tue, 23 May 2023 04:18:07 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec41b788488c21b7d482ff0f0bfbb022be4e32813795b01d9cecafa83a0be8f9`  
		Last Modified: Tue, 23 May 2023 04:18:10 GMT  
		Size: 14.1 MB (14087083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4314d2e9e62de6d9176830e185d701028a984e0c7553787dbe701721a5e5afdb`  
		Last Modified: Tue, 23 May 2023 04:18:05 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c051de3bff5e78a684c15f282bcd6df4cf3867917812ac522b6e71d5c8db794b`  
		Last Modified: Tue, 23 May 2023 04:18:05 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7f78bab28293fb999acd01969a1c1200e3709605dd6b165f2c04dcddc9f413`  
		Last Modified: Tue, 23 May 2023 04:18:20 GMT  
		Size: 115.9 MB (115898446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011807ab1ea4c4daaa35ce94fb51df9b7e3184e9207f6e8522441d2d2053abc1`  
		Last Modified: Tue, 23 May 2023 04:18:05 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5146016c0e9ff625ac285f603f05082728c2895cdf869378f6bcfcf5ed9963d`  
		Last Modified: Tue, 23 May 2023 04:18:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:f57eef421000aaf8332a91ab0b6c96b3c83ed2a981c29e6528b21ce10197cd16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:c4c526804552f6b4e8e124e182f5df4b09bf4bc88cba8a94adbd0a2ccb81dce6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169273935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6675b5cfea17abb655ea8229cbcfa5db9d0b041f839db0c24228c2e18a4bdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 31 Mar 2023 22:29:01 GMT
ADD file:a14b5a8b8b6993aeee5ac6052fdf283560d65365e5bcf133ab21c4756439384a in / 
# Fri, 31 Mar 2023 22:29:01 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 23:23:03 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 31 Mar 2023 23:23:04 GMT
ENV GOSU_VERSION=1.16
# Fri, 31 Mar 2023 23:23:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 31 Mar 2023 23:23:23 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 31 Mar 2023 23:23:25 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 31 Mar 2023 23:23:25 GMT
ENV MYSQL_MAJOR=5.7
# Mon, 17 Apr 2023 22:45:06 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Mon, 17 Apr 2023 22:45:06 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:45:25 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:45:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:45:25 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el7
# Mon, 17 Apr 2023 22:46:08 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:46:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:46:09 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:46:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:46:10 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:46:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e83e8f2e82cc31391cd0cb4f5ba574ba5eb9708fc0f5dcc34fef53b03ef28f31`  
		Last Modified: Fri, 31 Mar 2023 22:30:40 GMT  
		Size: 50.5 MB (50496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f23deb01b847d9dd0fc43ede2d2dacda423b95fdbf64e0ce21a6f542f6a167e`  
		Last Modified: Fri, 31 Mar 2023 23:25:04 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bda3b184ea984d363fc64e635076bcb405620effc23b2eac44f23e662bfd57`  
		Last Modified: Fri, 31 Mar 2023 23:25:05 GMT  
		Size: 983.7 KB (983706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed17edbc6604e6a5d584a08fa036d3d0711dde7676b4a6fe0adeb03b148ba5e7`  
		Last Modified: Fri, 31 Mar 2023 23:25:03 GMT  
		Size: 4.6 MB (4585198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a94a6acfa729dcf5f76be5966ecdc31692840ba7619f81d82d5e6dfc717c03`  
		Last Modified: Fri, 31 Mar 2023 23:25:02 GMT  
		Size: 2.7 KB (2653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f153bd2953e42c4994ce494be0c531c5260eb4d6623c1fd25db3bf99151456e9`  
		Last Modified: Mon, 17 Apr 2023 22:47:59 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab532edfb8133d99946879a0d39b72cdaafb249687f0cb36f2ca2251b051a9c7`  
		Last Modified: Mon, 17 Apr 2023 22:48:01 GMT  
		Size: 25.5 MB (25538322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76bdfe4f3d029057814b330ee6677a548fe964dd5822907d69680050d0003c2`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ffe2f25512b515f08ae407d0cd0e72010857d4ba8a34d0ee47279db49af6d`  
		Last Modified: Mon, 17 Apr 2023 22:48:11 GMT  
		Size: 87.7 MB (87660996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857ada4fbbcc843e4671c9029632651e1d4bd743c2f3326068ffeccb6fd795e0`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c508404c3ce0c3416a1c396965ce8b76f3719b7d2d592bfb6ac3b48f4ea20f`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:f57eef421000aaf8332a91ab0b6c96b3c83ed2a981c29e6528b21ce10197cd16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:c4c526804552f6b4e8e124e182f5df4b09bf4bc88cba8a94adbd0a2ccb81dce6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169273935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6675b5cfea17abb655ea8229cbcfa5db9d0b041f839db0c24228c2e18a4bdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 31 Mar 2023 22:29:01 GMT
ADD file:a14b5a8b8b6993aeee5ac6052fdf283560d65365e5bcf133ab21c4756439384a in / 
# Fri, 31 Mar 2023 22:29:01 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 23:23:03 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 31 Mar 2023 23:23:04 GMT
ENV GOSU_VERSION=1.16
# Fri, 31 Mar 2023 23:23:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 31 Mar 2023 23:23:23 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 31 Mar 2023 23:23:25 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 31 Mar 2023 23:23:25 GMT
ENV MYSQL_MAJOR=5.7
# Mon, 17 Apr 2023 22:45:06 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Mon, 17 Apr 2023 22:45:06 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:45:25 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:45:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:45:25 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el7
# Mon, 17 Apr 2023 22:46:08 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:46:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:46:09 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:46:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:46:10 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:46:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e83e8f2e82cc31391cd0cb4f5ba574ba5eb9708fc0f5dcc34fef53b03ef28f31`  
		Last Modified: Fri, 31 Mar 2023 22:30:40 GMT  
		Size: 50.5 MB (50496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f23deb01b847d9dd0fc43ede2d2dacda423b95fdbf64e0ce21a6f542f6a167e`  
		Last Modified: Fri, 31 Mar 2023 23:25:04 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bda3b184ea984d363fc64e635076bcb405620effc23b2eac44f23e662bfd57`  
		Last Modified: Fri, 31 Mar 2023 23:25:05 GMT  
		Size: 983.7 KB (983706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed17edbc6604e6a5d584a08fa036d3d0711dde7676b4a6fe0adeb03b148ba5e7`  
		Last Modified: Fri, 31 Mar 2023 23:25:03 GMT  
		Size: 4.6 MB (4585198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a94a6acfa729dcf5f76be5966ecdc31692840ba7619f81d82d5e6dfc717c03`  
		Last Modified: Fri, 31 Mar 2023 23:25:02 GMT  
		Size: 2.7 KB (2653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f153bd2953e42c4994ce494be0c531c5260eb4d6623c1fd25db3bf99151456e9`  
		Last Modified: Mon, 17 Apr 2023 22:47:59 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab532edfb8133d99946879a0d39b72cdaafb249687f0cb36f2ca2251b051a9c7`  
		Last Modified: Mon, 17 Apr 2023 22:48:01 GMT  
		Size: 25.5 MB (25538322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76bdfe4f3d029057814b330ee6677a548fe964dd5822907d69680050d0003c2`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ffe2f25512b515f08ae407d0cd0e72010857d4ba8a34d0ee47279db49af6d`  
		Last Modified: Mon, 17 Apr 2023 22:48:11 GMT  
		Size: 87.7 MB (87660996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857ada4fbbcc843e4671c9029632651e1d4bd743c2f3326068ffeccb6fd795e0`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c508404c3ce0c3416a1c396965ce8b76f3719b7d2d592bfb6ac3b48f4ea20f`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:11aea01c02f457f6c67e2037caa5e004e015ee94293aac224c0beb13459ee9db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:26504dc8b79b5b0bf60d9e7e043b7a2b1a9895b390382cf7ceab3792d8aa2e34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.8 MB (162758554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f270218b50ff2e08bc03cde8f0ba99dfef35758ef84f3c93e9c64d25b027be5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:16:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 May 2023 04:16:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:16:37 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 04:16:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 04:16:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 04:16:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:16:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 04:16:52 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 23 May 2023 04:16:52 GMT
ENV MYSQL_VERSION=5.7.42-1debian10
# Tue, 23 May 2023 04:16:53 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 May 2023 04:17:12 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 May 2023 04:17:13 GMT
VOLUME [/var/lib/mysql]
# Tue, 23 May 2023 04:17:13 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 23 May 2023 04:17:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 04:17:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 04:17:14 GMT
EXPOSE 3306 33060
# Tue, 23 May 2023 04:17:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ca486d93f7aa513f34a5fadffd81c536ce4ac5de719145803c6829aea16397`  
		Last Modified: Tue, 23 May 2023 04:18:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60f1b29379d4ba9ab2dabb338ac075c86cc37e5fdfcae5ae96dbbd6457cf089`  
		Last Modified: Tue, 23 May 2023 04:18:08 GMT  
		Size: 4.2 MB (4182401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a7f35f9a601ec927d75159dea2103af466efa76425e85420e4478dd4245c24`  
		Last Modified: Tue, 23 May 2023 04:18:08 GMT  
		Size: 1.4 MB (1441855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1256d8a34742417f317fd61b3b0a979ba9899c2a1fe1a41e0af44e91540db169`  
		Last Modified: Tue, 23 May 2023 04:18:07 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec41b788488c21b7d482ff0f0bfbb022be4e32813795b01d9cecafa83a0be8f9`  
		Last Modified: Tue, 23 May 2023 04:18:10 GMT  
		Size: 14.1 MB (14087083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4314d2e9e62de6d9176830e185d701028a984e0c7553787dbe701721a5e5afdb`  
		Last Modified: Tue, 23 May 2023 04:18:05 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c051de3bff5e78a684c15f282bcd6df4cf3867917812ac522b6e71d5c8db794b`  
		Last Modified: Tue, 23 May 2023 04:18:05 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7f78bab28293fb999acd01969a1c1200e3709605dd6b165f2c04dcddc9f413`  
		Last Modified: Tue, 23 May 2023 04:18:20 GMT  
		Size: 115.9 MB (115898446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011807ab1ea4c4daaa35ce94fb51df9b7e3184e9207f6e8522441d2d2053abc1`  
		Last Modified: Tue, 23 May 2023 04:18:05 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5146016c0e9ff625ac285f603f05082728c2895cdf869378f6bcfcf5ed9963d`  
		Last Modified: Tue, 23 May 2023 04:18:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:f57eef421000aaf8332a91ab0b6c96b3c83ed2a981c29e6528b21ce10197cd16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:c4c526804552f6b4e8e124e182f5df4b09bf4bc88cba8a94adbd0a2ccb81dce6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169273935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6675b5cfea17abb655ea8229cbcfa5db9d0b041f839db0c24228c2e18a4bdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 31 Mar 2023 22:29:01 GMT
ADD file:a14b5a8b8b6993aeee5ac6052fdf283560d65365e5bcf133ab21c4756439384a in / 
# Fri, 31 Mar 2023 22:29:01 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 23:23:03 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 31 Mar 2023 23:23:04 GMT
ENV GOSU_VERSION=1.16
# Fri, 31 Mar 2023 23:23:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 31 Mar 2023 23:23:23 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 31 Mar 2023 23:23:25 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 31 Mar 2023 23:23:25 GMT
ENV MYSQL_MAJOR=5.7
# Mon, 17 Apr 2023 22:45:06 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Mon, 17 Apr 2023 22:45:06 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:45:25 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:45:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:45:25 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el7
# Mon, 17 Apr 2023 22:46:08 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:46:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:46:09 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:46:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:46:10 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:46:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e83e8f2e82cc31391cd0cb4f5ba574ba5eb9708fc0f5dcc34fef53b03ef28f31`  
		Last Modified: Fri, 31 Mar 2023 22:30:40 GMT  
		Size: 50.5 MB (50496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f23deb01b847d9dd0fc43ede2d2dacda423b95fdbf64e0ce21a6f542f6a167e`  
		Last Modified: Fri, 31 Mar 2023 23:25:04 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bda3b184ea984d363fc64e635076bcb405620effc23b2eac44f23e662bfd57`  
		Last Modified: Fri, 31 Mar 2023 23:25:05 GMT  
		Size: 983.7 KB (983706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed17edbc6604e6a5d584a08fa036d3d0711dde7676b4a6fe0adeb03b148ba5e7`  
		Last Modified: Fri, 31 Mar 2023 23:25:03 GMT  
		Size: 4.6 MB (4585198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a94a6acfa729dcf5f76be5966ecdc31692840ba7619f81d82d5e6dfc717c03`  
		Last Modified: Fri, 31 Mar 2023 23:25:02 GMT  
		Size: 2.7 KB (2653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f153bd2953e42c4994ce494be0c531c5260eb4d6623c1fd25db3bf99151456e9`  
		Last Modified: Mon, 17 Apr 2023 22:47:59 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab532edfb8133d99946879a0d39b72cdaafb249687f0cb36f2ca2251b051a9c7`  
		Last Modified: Mon, 17 Apr 2023 22:48:01 GMT  
		Size: 25.5 MB (25538322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76bdfe4f3d029057814b330ee6677a548fe964dd5822907d69680050d0003c2`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ffe2f25512b515f08ae407d0cd0e72010857d4ba8a34d0ee47279db49af6d`  
		Last Modified: Mon, 17 Apr 2023 22:48:11 GMT  
		Size: 87.7 MB (87660996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857ada4fbbcc843e4671c9029632651e1d4bd743c2f3326068ffeccb6fd795e0`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c508404c3ce0c3416a1c396965ce8b76f3719b7d2d592bfb6ac3b48f4ea20f`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.42`

```console
$ docker pull mysql@sha256:f57eef421000aaf8332a91ab0b6c96b3c83ed2a981c29e6528b21ce10197cd16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.42` - linux; amd64

```console
$ docker pull mysql@sha256:c4c526804552f6b4e8e124e182f5df4b09bf4bc88cba8a94adbd0a2ccb81dce6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169273935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6675b5cfea17abb655ea8229cbcfa5db9d0b041f839db0c24228c2e18a4bdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 31 Mar 2023 22:29:01 GMT
ADD file:a14b5a8b8b6993aeee5ac6052fdf283560d65365e5bcf133ab21c4756439384a in / 
# Fri, 31 Mar 2023 22:29:01 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 23:23:03 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 31 Mar 2023 23:23:04 GMT
ENV GOSU_VERSION=1.16
# Fri, 31 Mar 2023 23:23:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 31 Mar 2023 23:23:23 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 31 Mar 2023 23:23:25 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 31 Mar 2023 23:23:25 GMT
ENV MYSQL_MAJOR=5.7
# Mon, 17 Apr 2023 22:45:06 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Mon, 17 Apr 2023 22:45:06 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:45:25 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:45:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:45:25 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el7
# Mon, 17 Apr 2023 22:46:08 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:46:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:46:09 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:46:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:46:10 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:46:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e83e8f2e82cc31391cd0cb4f5ba574ba5eb9708fc0f5dcc34fef53b03ef28f31`  
		Last Modified: Fri, 31 Mar 2023 22:30:40 GMT  
		Size: 50.5 MB (50496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f23deb01b847d9dd0fc43ede2d2dacda423b95fdbf64e0ce21a6f542f6a167e`  
		Last Modified: Fri, 31 Mar 2023 23:25:04 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bda3b184ea984d363fc64e635076bcb405620effc23b2eac44f23e662bfd57`  
		Last Modified: Fri, 31 Mar 2023 23:25:05 GMT  
		Size: 983.7 KB (983706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed17edbc6604e6a5d584a08fa036d3d0711dde7676b4a6fe0adeb03b148ba5e7`  
		Last Modified: Fri, 31 Mar 2023 23:25:03 GMT  
		Size: 4.6 MB (4585198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a94a6acfa729dcf5f76be5966ecdc31692840ba7619f81d82d5e6dfc717c03`  
		Last Modified: Fri, 31 Mar 2023 23:25:02 GMT  
		Size: 2.7 KB (2653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f153bd2953e42c4994ce494be0c531c5260eb4d6623c1fd25db3bf99151456e9`  
		Last Modified: Mon, 17 Apr 2023 22:47:59 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab532edfb8133d99946879a0d39b72cdaafb249687f0cb36f2ca2251b051a9c7`  
		Last Modified: Mon, 17 Apr 2023 22:48:01 GMT  
		Size: 25.5 MB (25538322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76bdfe4f3d029057814b330ee6677a548fe964dd5822907d69680050d0003c2`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ffe2f25512b515f08ae407d0cd0e72010857d4ba8a34d0ee47279db49af6d`  
		Last Modified: Mon, 17 Apr 2023 22:48:11 GMT  
		Size: 87.7 MB (87660996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857ada4fbbcc843e4671c9029632651e1d4bd743c2f3326068ffeccb6fd795e0`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c508404c3ce0c3416a1c396965ce8b76f3719b7d2d592bfb6ac3b48f4ea20f`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.42-debian`

```console
$ docker pull mysql@sha256:11aea01c02f457f6c67e2037caa5e004e015ee94293aac224c0beb13459ee9db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.42-debian` - linux; amd64

```console
$ docker pull mysql@sha256:26504dc8b79b5b0bf60d9e7e043b7a2b1a9895b390382cf7ceab3792d8aa2e34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.8 MB (162758554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f270218b50ff2e08bc03cde8f0ba99dfef35758ef84f3c93e9c64d25b027be5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:16:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 May 2023 04:16:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:16:37 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 04:16:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 04:16:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 04:16:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:16:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 04:16:52 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 23 May 2023 04:16:52 GMT
ENV MYSQL_VERSION=5.7.42-1debian10
# Tue, 23 May 2023 04:16:53 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 May 2023 04:17:12 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 May 2023 04:17:13 GMT
VOLUME [/var/lib/mysql]
# Tue, 23 May 2023 04:17:13 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 23 May 2023 04:17:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 04:17:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 04:17:14 GMT
EXPOSE 3306 33060
# Tue, 23 May 2023 04:17:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ca486d93f7aa513f34a5fadffd81c536ce4ac5de719145803c6829aea16397`  
		Last Modified: Tue, 23 May 2023 04:18:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60f1b29379d4ba9ab2dabb338ac075c86cc37e5fdfcae5ae96dbbd6457cf089`  
		Last Modified: Tue, 23 May 2023 04:18:08 GMT  
		Size: 4.2 MB (4182401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a7f35f9a601ec927d75159dea2103af466efa76425e85420e4478dd4245c24`  
		Last Modified: Tue, 23 May 2023 04:18:08 GMT  
		Size: 1.4 MB (1441855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1256d8a34742417f317fd61b3b0a979ba9899c2a1fe1a41e0af44e91540db169`  
		Last Modified: Tue, 23 May 2023 04:18:07 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec41b788488c21b7d482ff0f0bfbb022be4e32813795b01d9cecafa83a0be8f9`  
		Last Modified: Tue, 23 May 2023 04:18:10 GMT  
		Size: 14.1 MB (14087083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4314d2e9e62de6d9176830e185d701028a984e0c7553787dbe701721a5e5afdb`  
		Last Modified: Tue, 23 May 2023 04:18:05 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c051de3bff5e78a684c15f282bcd6df4cf3867917812ac522b6e71d5c8db794b`  
		Last Modified: Tue, 23 May 2023 04:18:05 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7f78bab28293fb999acd01969a1c1200e3709605dd6b165f2c04dcddc9f413`  
		Last Modified: Tue, 23 May 2023 04:18:20 GMT  
		Size: 115.9 MB (115898446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011807ab1ea4c4daaa35ce94fb51df9b7e3184e9207f6e8522441d2d2053abc1`  
		Last Modified: Tue, 23 May 2023 04:18:05 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5146016c0e9ff625ac285f603f05082728c2895cdf869378f6bcfcf5ed9963d`  
		Last Modified: Tue, 23 May 2023 04:18:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.42-oracle`

```console
$ docker pull mysql@sha256:f57eef421000aaf8332a91ab0b6c96b3c83ed2a981c29e6528b21ce10197cd16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.42-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:c4c526804552f6b4e8e124e182f5df4b09bf4bc88cba8a94adbd0a2ccb81dce6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169273935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6675b5cfea17abb655ea8229cbcfa5db9d0b041f839db0c24228c2e18a4bdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 31 Mar 2023 22:29:01 GMT
ADD file:a14b5a8b8b6993aeee5ac6052fdf283560d65365e5bcf133ab21c4756439384a in / 
# Fri, 31 Mar 2023 22:29:01 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 23:23:03 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 31 Mar 2023 23:23:04 GMT
ENV GOSU_VERSION=1.16
# Fri, 31 Mar 2023 23:23:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 31 Mar 2023 23:23:23 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Fri, 31 Mar 2023 23:23:25 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 31 Mar 2023 23:23:25 GMT
ENV MYSQL_MAJOR=5.7
# Mon, 17 Apr 2023 22:45:06 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Mon, 17 Apr 2023 22:45:06 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:45:25 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:45:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:45:25 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el7
# Mon, 17 Apr 2023 22:46:08 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:46:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:46:09 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:46:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:46:10 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:46:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e83e8f2e82cc31391cd0cb4f5ba574ba5eb9708fc0f5dcc34fef53b03ef28f31`  
		Last Modified: Fri, 31 Mar 2023 22:30:40 GMT  
		Size: 50.5 MB (50496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f23deb01b847d9dd0fc43ede2d2dacda423b95fdbf64e0ce21a6f542f6a167e`  
		Last Modified: Fri, 31 Mar 2023 23:25:04 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bda3b184ea984d363fc64e635076bcb405620effc23b2eac44f23e662bfd57`  
		Last Modified: Fri, 31 Mar 2023 23:25:05 GMT  
		Size: 983.7 KB (983706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed17edbc6604e6a5d584a08fa036d3d0711dde7676b4a6fe0adeb03b148ba5e7`  
		Last Modified: Fri, 31 Mar 2023 23:25:03 GMT  
		Size: 4.6 MB (4585198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a94a6acfa729dcf5f76be5966ecdc31692840ba7619f81d82d5e6dfc717c03`  
		Last Modified: Fri, 31 Mar 2023 23:25:02 GMT  
		Size: 2.7 KB (2653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f153bd2953e42c4994ce494be0c531c5260eb4d6623c1fd25db3bf99151456e9`  
		Last Modified: Mon, 17 Apr 2023 22:47:59 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab532edfb8133d99946879a0d39b72cdaafb249687f0cb36f2ca2251b051a9c7`  
		Last Modified: Mon, 17 Apr 2023 22:48:01 GMT  
		Size: 25.5 MB (25538322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76bdfe4f3d029057814b330ee6677a548fe964dd5822907d69680050d0003c2`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ffe2f25512b515f08ae407d0cd0e72010857d4ba8a34d0ee47279db49af6d`  
		Last Modified: Mon, 17 Apr 2023 22:48:11 GMT  
		Size: 87.7 MB (87660996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857ada4fbbcc843e4671c9029632651e1d4bd743c2f3326068ffeccb6fd795e0`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c508404c3ce0c3416a1c396965ce8b76f3719b7d2d592bfb6ac3b48f4ea20f`  
		Last Modified: Mon, 17 Apr 2023 22:47:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:a43f6e7e7f3a5e5b90f857fbed4e3103ece771b19f0f75880f767cf66bbb6577
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:b45a7c3e6fb15526e8bf62ebb940cd460617e36f46155b8514fd9c9388231817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165315366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8189e588b0e8fcc95b0d764d6f7bdb55b5b41e9249157177d73781058f603ca9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:20:31 GMT
ADD file:61a2085af5116916e7b117c2e7ad7116bdc0282d8fa9ce76191c4101f5e866ff in / 
# Thu, 06 Apr 2023 18:20:32 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:43:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:43:29 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:43:32 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:43:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:43:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:43:58 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:43:23 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:43:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:43:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:43:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:43:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:44:32 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:44:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:44:33 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:44:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:44:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:44:34 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:44:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:328ba678bf27575937f8b9dfbf5b5f39b21941af068f8e5960de8131e289da85`  
		Last Modified: Thu, 06 Apr 2023 18:21:19 GMT  
		Size: 44.6 MB (44563902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f5ff008d73bef1d4c8e1a4c73a7efc7697e8087a950065fb369c83a03df08d`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7054d6d0c7c57672cd9e48e8a92eda15a4f0ae24dc78413fdce3fce3064a77`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b5d4e8750e78990227fa3f3df12b6ccdf3b2486b4248677b7959dd95c0e77b`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 4.6 MB (4608287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc4a7b43bdd822158ae54cac5da309097088de0253879cbb07e31829d8f4561`  
		Last Modified: Thu, 06 Apr 2023 18:45:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0608f8959e036b9e5f55227da2fac404f45e153119063fd042cba4cdcdc9e6c`  
		Last Modified: Mon, 17 Apr 2023 22:46:55 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5823e721608fd3d82b87e136e4cb898d8ffbbf25cedb6dcd2a22c38fe25e038d`  
		Last Modified: Mon, 17 Apr 2023 22:47:02 GMT  
		Size: 58.6 MB (58588139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a564ada930a970424e6b25a29d9d4f706d15f9e6401c21bcef3e841853f7527e`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539565d00e89aa08d29023b1284734fea67d9ff99366188c4ff29d0da6d59187`  
		Last Modified: Mon, 17 Apr 2023 22:47:03 GMT  
		Size: 56.6 MB (56562540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a06843fd5b834a3c6eb03387de3fcac84eb24f940ed1271579d2d76f137e6`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f6d4aa041d96e3ebda9dfafe42be4f7eed49456ba2c492adeffe85f10aad06`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:84dfe3825c21a0ec7e8e858b9ed118846bf096c1e0bc1a07458c04b393f2c7d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169785464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5371f8c3b63eec64a33b35530be5212d6148e0940111b57b689b5ba1ffe808c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:40:07 GMT
ADD file:c798bcae4b9271a204dc37f132bce1f0042c02cb1ad5a2237f56dec227d44438 in / 
# Thu, 06 Apr 2023 18:40:07 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:55:56 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:55:56 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:55:59 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:56:26 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:56:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:56:27 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:39:53 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:39:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:40:25 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:40:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:40:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:40:59 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:41:00 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:41:01 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:41:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:41:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:41:01 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:41:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6425367b44c9c3f59fd1e81f8fa2e9170ca2ef552d63f35a08ef3969ee4ff557`  
		Last Modified: Thu, 06 Apr 2023 18:40:43 GMT  
		Size: 43.5 MB (43477048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cef374d113a386d9e9eb540635c8e0d47e85deb38985982b5aeddc4798f67c7`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1751ddbc0d77eedc43d2aad156c590e2fec2c2f75fde0aef0757c69a0ba49f6d`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41e9e3c6d9abdfec73965f0105ee343f69e0c909c07b665ea81a2642e19365f`  
		Last Modified: Thu, 06 Apr 2023 18:57:58 GMT  
		Size: 4.5 MB (4465472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26e9c11cd2da41af092e3a224bcb367ba5201e02509f5e39bf009085eafe838`  
		Last Modified: Thu, 06 Apr 2023 18:57:57 GMT  
		Size: 2.6 KB (2627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ad8819238aa147cd2a97e255d96d27a755f14f31c8c0f3a0e2a66b0d7fa88`  
		Last Modified: Mon, 17 Apr 2023 22:41:24 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3028a5ad3fd0158e2835500be170a4877a5a73cb87680e42c6d49a9217051e6a`  
		Last Modified: Mon, 17 Apr 2023 22:41:29 GMT  
		Size: 57.9 MB (57858475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41584bf2c82e3943b457046f452be302b74a47ac1b299740871166e772ad4af`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413abbd4b9d17bb93f8402bc56f26c11a4c3d88c274d353b57b0072a682f7fa`  
		Last Modified: Mon, 17 Apr 2023 22:41:30 GMT  
		Size: 63.1 MB (63061793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7c55c30cf5aaea11b0b27ce0a8014a289e3b9032b39013cb6201e35c389924`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038fc84e09b5dcf7a11080675b9b0a54b30f71fc78a3eda72de1a328c1f061f0`  
		Last Modified: Mon, 17 Apr 2023 22:41:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:8997d21bc7a8406c9ea3de932a25306091749e702a37d51aebafcf93beb3db2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:fc3550b4a91253802c92b328a2b064582d63197591e662a08d3e417e7326853b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179701768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11a2cc2219892cd270339bff1627493e4fb6f64c86567c5058da8aba128a1cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:15:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 May 2023 04:15:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:15:47 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 04:15:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 04:15:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 04:16:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:16:03 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 04:16:03 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 23 May 2023 04:16:03 GMT
ENV MYSQL_VERSION=8.0.33-1debian11
# Tue, 23 May 2023 04:16:04 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 May 2023 04:16:19 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 May 2023 04:16:20 GMT
VOLUME [/var/lib/mysql]
# Tue, 23 May 2023 04:16:20 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 23 May 2023 04:16:20 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 23 May 2023 04:16:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 04:16:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 04:16:21 GMT
EXPOSE 3306 33060
# Tue, 23 May 2023 04:16:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460bb444d52dab6a19d68cfcc664add2dd2ebb433465ed374770429b7b85ecf6`  
		Last Modified: Tue, 23 May 2023 04:17:36 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ceec72175ab896b5d2aae94caa4ad5ee8dc1eec8fbf86eda6c93dabc2d2b7b`  
		Last Modified: Tue, 23 May 2023 04:17:37 GMT  
		Size: 4.4 MB (4415030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca6f73d0c4e067456900a23eeda855c5a38bc7527c69a596f138baac0c06a5a`  
		Last Modified: Tue, 23 May 2023 04:17:35 GMT  
		Size: 1.5 MB (1471543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af5e268315b55d1318f7f5e708e8db3da0c9acd1d112b5cce069277aecc4e5`  
		Last Modified: Tue, 23 May 2023 04:17:34 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c12e7f453833e46579664261597f2f95c2a431caf865aadf793d1347ce1307`  
		Last Modified: Tue, 23 May 2023 04:17:37 GMT  
		Size: 12.7 MB (12661298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe8fac55990e5d5c61ee5ba24b86408236dcd4042d2b7802b5686605f8c1773`  
		Last Modified: Tue, 23 May 2023 04:17:34 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c00b032f6190d836908e7deb81e0b799be548829cb670b8e727e1b318695a`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da46d64fa01826465a87b81773db1102a8d174575ef9e512fc1fc36961826247`  
		Last Modified: Tue, 23 May 2023 04:17:50 GMT  
		Size: 129.7 MB (129739276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c38d2a0b5b87053ff6f692215d70e349dfed59ab3e0153ebaf24623092e334e`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d594c6498dbdf44ee78d77d380d5da7b3c336b2d902eaa2d7390ddbebf4e36c`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d10222ee5144f5619674bc5786fd9170447bc57d66081d3081246677f10d4c`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:a43f6e7e7f3a5e5b90f857fbed4e3103ece771b19f0f75880f767cf66bbb6577
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:b45a7c3e6fb15526e8bf62ebb940cd460617e36f46155b8514fd9c9388231817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165315366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8189e588b0e8fcc95b0d764d6f7bdb55b5b41e9249157177d73781058f603ca9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:20:31 GMT
ADD file:61a2085af5116916e7b117c2e7ad7116bdc0282d8fa9ce76191c4101f5e866ff in / 
# Thu, 06 Apr 2023 18:20:32 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:43:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:43:29 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:43:32 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:43:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:43:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:43:58 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:43:23 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:43:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:43:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:43:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:43:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:44:32 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:44:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:44:33 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:44:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:44:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:44:34 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:44:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:328ba678bf27575937f8b9dfbf5b5f39b21941af068f8e5960de8131e289da85`  
		Last Modified: Thu, 06 Apr 2023 18:21:19 GMT  
		Size: 44.6 MB (44563902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f5ff008d73bef1d4c8e1a4c73a7efc7697e8087a950065fb369c83a03df08d`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7054d6d0c7c57672cd9e48e8a92eda15a4f0ae24dc78413fdce3fce3064a77`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b5d4e8750e78990227fa3f3df12b6ccdf3b2486b4248677b7959dd95c0e77b`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 4.6 MB (4608287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc4a7b43bdd822158ae54cac5da309097088de0253879cbb07e31829d8f4561`  
		Last Modified: Thu, 06 Apr 2023 18:45:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0608f8959e036b9e5f55227da2fac404f45e153119063fd042cba4cdcdc9e6c`  
		Last Modified: Mon, 17 Apr 2023 22:46:55 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5823e721608fd3d82b87e136e4cb898d8ffbbf25cedb6dcd2a22c38fe25e038d`  
		Last Modified: Mon, 17 Apr 2023 22:47:02 GMT  
		Size: 58.6 MB (58588139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a564ada930a970424e6b25a29d9d4f706d15f9e6401c21bcef3e841853f7527e`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539565d00e89aa08d29023b1284734fea67d9ff99366188c4ff29d0da6d59187`  
		Last Modified: Mon, 17 Apr 2023 22:47:03 GMT  
		Size: 56.6 MB (56562540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a06843fd5b834a3c6eb03387de3fcac84eb24f940ed1271579d2d76f137e6`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f6d4aa041d96e3ebda9dfafe42be4f7eed49456ba2c492adeffe85f10aad06`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:84dfe3825c21a0ec7e8e858b9ed118846bf096c1e0bc1a07458c04b393f2c7d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169785464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5371f8c3b63eec64a33b35530be5212d6148e0940111b57b689b5ba1ffe808c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:40:07 GMT
ADD file:c798bcae4b9271a204dc37f132bce1f0042c02cb1ad5a2237f56dec227d44438 in / 
# Thu, 06 Apr 2023 18:40:07 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:55:56 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:55:56 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:55:59 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:56:26 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:56:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:56:27 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:39:53 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:39:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:40:25 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:40:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:40:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:40:59 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:41:00 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:41:01 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:41:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:41:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:41:01 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:41:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6425367b44c9c3f59fd1e81f8fa2e9170ca2ef552d63f35a08ef3969ee4ff557`  
		Last Modified: Thu, 06 Apr 2023 18:40:43 GMT  
		Size: 43.5 MB (43477048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cef374d113a386d9e9eb540635c8e0d47e85deb38985982b5aeddc4798f67c7`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1751ddbc0d77eedc43d2aad156c590e2fec2c2f75fde0aef0757c69a0ba49f6d`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41e9e3c6d9abdfec73965f0105ee343f69e0c909c07b665ea81a2642e19365f`  
		Last Modified: Thu, 06 Apr 2023 18:57:58 GMT  
		Size: 4.5 MB (4465472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26e9c11cd2da41af092e3a224bcb367ba5201e02509f5e39bf009085eafe838`  
		Last Modified: Thu, 06 Apr 2023 18:57:57 GMT  
		Size: 2.6 KB (2627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ad8819238aa147cd2a97e255d96d27a755f14f31c8c0f3a0e2a66b0d7fa88`  
		Last Modified: Mon, 17 Apr 2023 22:41:24 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3028a5ad3fd0158e2835500be170a4877a5a73cb87680e42c6d49a9217051e6a`  
		Last Modified: Mon, 17 Apr 2023 22:41:29 GMT  
		Size: 57.9 MB (57858475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41584bf2c82e3943b457046f452be302b74a47ac1b299740871166e772ad4af`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413abbd4b9d17bb93f8402bc56f26c11a4c3d88c274d353b57b0072a682f7fa`  
		Last Modified: Mon, 17 Apr 2023 22:41:30 GMT  
		Size: 63.1 MB (63061793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7c55c30cf5aaea11b0b27ce0a8014a289e3b9032b39013cb6201e35c389924`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038fc84e09b5dcf7a11080675b9b0a54b30f71fc78a3eda72de1a328c1f061f0`  
		Last Modified: Mon, 17 Apr 2023 22:41:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:a43f6e7e7f3a5e5b90f857fbed4e3103ece771b19f0f75880f767cf66bbb6577
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:b45a7c3e6fb15526e8bf62ebb940cd460617e36f46155b8514fd9c9388231817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165315366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8189e588b0e8fcc95b0d764d6f7bdb55b5b41e9249157177d73781058f603ca9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:20:31 GMT
ADD file:61a2085af5116916e7b117c2e7ad7116bdc0282d8fa9ce76191c4101f5e866ff in / 
# Thu, 06 Apr 2023 18:20:32 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:43:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:43:29 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:43:32 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:43:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:43:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:43:58 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:43:23 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:43:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:43:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:43:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:43:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:44:32 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:44:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:44:33 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:44:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:44:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:44:34 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:44:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:328ba678bf27575937f8b9dfbf5b5f39b21941af068f8e5960de8131e289da85`  
		Last Modified: Thu, 06 Apr 2023 18:21:19 GMT  
		Size: 44.6 MB (44563902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f5ff008d73bef1d4c8e1a4c73a7efc7697e8087a950065fb369c83a03df08d`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7054d6d0c7c57672cd9e48e8a92eda15a4f0ae24dc78413fdce3fce3064a77`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b5d4e8750e78990227fa3f3df12b6ccdf3b2486b4248677b7959dd95c0e77b`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 4.6 MB (4608287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc4a7b43bdd822158ae54cac5da309097088de0253879cbb07e31829d8f4561`  
		Last Modified: Thu, 06 Apr 2023 18:45:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0608f8959e036b9e5f55227da2fac404f45e153119063fd042cba4cdcdc9e6c`  
		Last Modified: Mon, 17 Apr 2023 22:46:55 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5823e721608fd3d82b87e136e4cb898d8ffbbf25cedb6dcd2a22c38fe25e038d`  
		Last Modified: Mon, 17 Apr 2023 22:47:02 GMT  
		Size: 58.6 MB (58588139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a564ada930a970424e6b25a29d9d4f706d15f9e6401c21bcef3e841853f7527e`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539565d00e89aa08d29023b1284734fea67d9ff99366188c4ff29d0da6d59187`  
		Last Modified: Mon, 17 Apr 2023 22:47:03 GMT  
		Size: 56.6 MB (56562540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a06843fd5b834a3c6eb03387de3fcac84eb24f940ed1271579d2d76f137e6`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f6d4aa041d96e3ebda9dfafe42be4f7eed49456ba2c492adeffe85f10aad06`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:84dfe3825c21a0ec7e8e858b9ed118846bf096c1e0bc1a07458c04b393f2c7d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169785464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5371f8c3b63eec64a33b35530be5212d6148e0940111b57b689b5ba1ffe808c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:40:07 GMT
ADD file:c798bcae4b9271a204dc37f132bce1f0042c02cb1ad5a2237f56dec227d44438 in / 
# Thu, 06 Apr 2023 18:40:07 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:55:56 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:55:56 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:55:59 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:56:26 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:56:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:56:27 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:39:53 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:39:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:40:25 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:40:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:40:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:40:59 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:41:00 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:41:01 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:41:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:41:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:41:01 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:41:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6425367b44c9c3f59fd1e81f8fa2e9170ca2ef552d63f35a08ef3969ee4ff557`  
		Last Modified: Thu, 06 Apr 2023 18:40:43 GMT  
		Size: 43.5 MB (43477048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cef374d113a386d9e9eb540635c8e0d47e85deb38985982b5aeddc4798f67c7`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1751ddbc0d77eedc43d2aad156c590e2fec2c2f75fde0aef0757c69a0ba49f6d`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41e9e3c6d9abdfec73965f0105ee343f69e0c909c07b665ea81a2642e19365f`  
		Last Modified: Thu, 06 Apr 2023 18:57:58 GMT  
		Size: 4.5 MB (4465472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26e9c11cd2da41af092e3a224bcb367ba5201e02509f5e39bf009085eafe838`  
		Last Modified: Thu, 06 Apr 2023 18:57:57 GMT  
		Size: 2.6 KB (2627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ad8819238aa147cd2a97e255d96d27a755f14f31c8c0f3a0e2a66b0d7fa88`  
		Last Modified: Mon, 17 Apr 2023 22:41:24 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3028a5ad3fd0158e2835500be170a4877a5a73cb87680e42c6d49a9217051e6a`  
		Last Modified: Mon, 17 Apr 2023 22:41:29 GMT  
		Size: 57.9 MB (57858475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41584bf2c82e3943b457046f452be302b74a47ac1b299740871166e772ad4af`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413abbd4b9d17bb93f8402bc56f26c11a4c3d88c274d353b57b0072a682f7fa`  
		Last Modified: Mon, 17 Apr 2023 22:41:30 GMT  
		Size: 63.1 MB (63061793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7c55c30cf5aaea11b0b27ce0a8014a289e3b9032b39013cb6201e35c389924`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038fc84e09b5dcf7a11080675b9b0a54b30f71fc78a3eda72de1a328c1f061f0`  
		Last Modified: Mon, 17 Apr 2023 22:41:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:8997d21bc7a8406c9ea3de932a25306091749e702a37d51aebafcf93beb3db2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:fc3550b4a91253802c92b328a2b064582d63197591e662a08d3e417e7326853b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179701768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11a2cc2219892cd270339bff1627493e4fb6f64c86567c5058da8aba128a1cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:15:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 May 2023 04:15:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:15:47 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 04:15:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 04:15:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 04:16:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:16:03 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 04:16:03 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 23 May 2023 04:16:03 GMT
ENV MYSQL_VERSION=8.0.33-1debian11
# Tue, 23 May 2023 04:16:04 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 May 2023 04:16:19 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 May 2023 04:16:20 GMT
VOLUME [/var/lib/mysql]
# Tue, 23 May 2023 04:16:20 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 23 May 2023 04:16:20 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 23 May 2023 04:16:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 04:16:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 04:16:21 GMT
EXPOSE 3306 33060
# Tue, 23 May 2023 04:16:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460bb444d52dab6a19d68cfcc664add2dd2ebb433465ed374770429b7b85ecf6`  
		Last Modified: Tue, 23 May 2023 04:17:36 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ceec72175ab896b5d2aae94caa4ad5ee8dc1eec8fbf86eda6c93dabc2d2b7b`  
		Last Modified: Tue, 23 May 2023 04:17:37 GMT  
		Size: 4.4 MB (4415030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca6f73d0c4e067456900a23eeda855c5a38bc7527c69a596f138baac0c06a5a`  
		Last Modified: Tue, 23 May 2023 04:17:35 GMT  
		Size: 1.5 MB (1471543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af5e268315b55d1318f7f5e708e8db3da0c9acd1d112b5cce069277aecc4e5`  
		Last Modified: Tue, 23 May 2023 04:17:34 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c12e7f453833e46579664261597f2f95c2a431caf865aadf793d1347ce1307`  
		Last Modified: Tue, 23 May 2023 04:17:37 GMT  
		Size: 12.7 MB (12661298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe8fac55990e5d5c61ee5ba24b86408236dcd4042d2b7802b5686605f8c1773`  
		Last Modified: Tue, 23 May 2023 04:17:34 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c00b032f6190d836908e7deb81e0b799be548829cb670b8e727e1b318695a`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da46d64fa01826465a87b81773db1102a8d174575ef9e512fc1fc36961826247`  
		Last Modified: Tue, 23 May 2023 04:17:50 GMT  
		Size: 129.7 MB (129739276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c38d2a0b5b87053ff6f692215d70e349dfed59ab3e0153ebaf24623092e334e`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d594c6498dbdf44ee78d77d380d5da7b3c336b2d902eaa2d7390ddbebf4e36c`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d10222ee5144f5619674bc5786fd9170447bc57d66081d3081246677f10d4c`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:a43f6e7e7f3a5e5b90f857fbed4e3103ece771b19f0f75880f767cf66bbb6577
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:b45a7c3e6fb15526e8bf62ebb940cd460617e36f46155b8514fd9c9388231817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165315366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8189e588b0e8fcc95b0d764d6f7bdb55b5b41e9249157177d73781058f603ca9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:20:31 GMT
ADD file:61a2085af5116916e7b117c2e7ad7116bdc0282d8fa9ce76191c4101f5e866ff in / 
# Thu, 06 Apr 2023 18:20:32 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:43:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:43:29 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:43:32 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:43:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:43:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:43:58 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:43:23 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:43:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:43:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:43:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:43:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:44:32 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:44:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:44:33 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:44:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:44:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:44:34 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:44:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:328ba678bf27575937f8b9dfbf5b5f39b21941af068f8e5960de8131e289da85`  
		Last Modified: Thu, 06 Apr 2023 18:21:19 GMT  
		Size: 44.6 MB (44563902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f5ff008d73bef1d4c8e1a4c73a7efc7697e8087a950065fb369c83a03df08d`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7054d6d0c7c57672cd9e48e8a92eda15a4f0ae24dc78413fdce3fce3064a77`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b5d4e8750e78990227fa3f3df12b6ccdf3b2486b4248677b7959dd95c0e77b`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 4.6 MB (4608287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc4a7b43bdd822158ae54cac5da309097088de0253879cbb07e31829d8f4561`  
		Last Modified: Thu, 06 Apr 2023 18:45:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0608f8959e036b9e5f55227da2fac404f45e153119063fd042cba4cdcdc9e6c`  
		Last Modified: Mon, 17 Apr 2023 22:46:55 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5823e721608fd3d82b87e136e4cb898d8ffbbf25cedb6dcd2a22c38fe25e038d`  
		Last Modified: Mon, 17 Apr 2023 22:47:02 GMT  
		Size: 58.6 MB (58588139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a564ada930a970424e6b25a29d9d4f706d15f9e6401c21bcef3e841853f7527e`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539565d00e89aa08d29023b1284734fea67d9ff99366188c4ff29d0da6d59187`  
		Last Modified: Mon, 17 Apr 2023 22:47:03 GMT  
		Size: 56.6 MB (56562540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a06843fd5b834a3c6eb03387de3fcac84eb24f940ed1271579d2d76f137e6`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f6d4aa041d96e3ebda9dfafe42be4f7eed49456ba2c492adeffe85f10aad06`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:84dfe3825c21a0ec7e8e858b9ed118846bf096c1e0bc1a07458c04b393f2c7d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169785464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5371f8c3b63eec64a33b35530be5212d6148e0940111b57b689b5ba1ffe808c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:40:07 GMT
ADD file:c798bcae4b9271a204dc37f132bce1f0042c02cb1ad5a2237f56dec227d44438 in / 
# Thu, 06 Apr 2023 18:40:07 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:55:56 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:55:56 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:55:59 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:56:26 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:56:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:56:27 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:39:53 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:39:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:40:25 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:40:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:40:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:40:59 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:41:00 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:41:01 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:41:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:41:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:41:01 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:41:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6425367b44c9c3f59fd1e81f8fa2e9170ca2ef552d63f35a08ef3969ee4ff557`  
		Last Modified: Thu, 06 Apr 2023 18:40:43 GMT  
		Size: 43.5 MB (43477048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cef374d113a386d9e9eb540635c8e0d47e85deb38985982b5aeddc4798f67c7`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1751ddbc0d77eedc43d2aad156c590e2fec2c2f75fde0aef0757c69a0ba49f6d`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41e9e3c6d9abdfec73965f0105ee343f69e0c909c07b665ea81a2642e19365f`  
		Last Modified: Thu, 06 Apr 2023 18:57:58 GMT  
		Size: 4.5 MB (4465472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26e9c11cd2da41af092e3a224bcb367ba5201e02509f5e39bf009085eafe838`  
		Last Modified: Thu, 06 Apr 2023 18:57:57 GMT  
		Size: 2.6 KB (2627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ad8819238aa147cd2a97e255d96d27a755f14f31c8c0f3a0e2a66b0d7fa88`  
		Last Modified: Mon, 17 Apr 2023 22:41:24 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3028a5ad3fd0158e2835500be170a4877a5a73cb87680e42c6d49a9217051e6a`  
		Last Modified: Mon, 17 Apr 2023 22:41:29 GMT  
		Size: 57.9 MB (57858475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41584bf2c82e3943b457046f452be302b74a47ac1b299740871166e772ad4af`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413abbd4b9d17bb93f8402bc56f26c11a4c3d88c274d353b57b0072a682f7fa`  
		Last Modified: Mon, 17 Apr 2023 22:41:30 GMT  
		Size: 63.1 MB (63061793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7c55c30cf5aaea11b0b27ce0a8014a289e3b9032b39013cb6201e35c389924`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038fc84e09b5dcf7a11080675b9b0a54b30f71fc78a3eda72de1a328c1f061f0`  
		Last Modified: Mon, 17 Apr 2023 22:41:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.33`

```console
$ docker pull mysql@sha256:a43f6e7e7f3a5e5b90f857fbed4e3103ece771b19f0f75880f767cf66bbb6577
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.33` - linux; amd64

```console
$ docker pull mysql@sha256:b45a7c3e6fb15526e8bf62ebb940cd460617e36f46155b8514fd9c9388231817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165315366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8189e588b0e8fcc95b0d764d6f7bdb55b5b41e9249157177d73781058f603ca9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:20:31 GMT
ADD file:61a2085af5116916e7b117c2e7ad7116bdc0282d8fa9ce76191c4101f5e866ff in / 
# Thu, 06 Apr 2023 18:20:32 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:43:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:43:29 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:43:32 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:43:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:43:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:43:58 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:43:23 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:43:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:43:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:43:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:43:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:44:32 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:44:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:44:33 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:44:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:44:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:44:34 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:44:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:328ba678bf27575937f8b9dfbf5b5f39b21941af068f8e5960de8131e289da85`  
		Last Modified: Thu, 06 Apr 2023 18:21:19 GMT  
		Size: 44.6 MB (44563902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f5ff008d73bef1d4c8e1a4c73a7efc7697e8087a950065fb369c83a03df08d`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7054d6d0c7c57672cd9e48e8a92eda15a4f0ae24dc78413fdce3fce3064a77`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b5d4e8750e78990227fa3f3df12b6ccdf3b2486b4248677b7959dd95c0e77b`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 4.6 MB (4608287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc4a7b43bdd822158ae54cac5da309097088de0253879cbb07e31829d8f4561`  
		Last Modified: Thu, 06 Apr 2023 18:45:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0608f8959e036b9e5f55227da2fac404f45e153119063fd042cba4cdcdc9e6c`  
		Last Modified: Mon, 17 Apr 2023 22:46:55 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5823e721608fd3d82b87e136e4cb898d8ffbbf25cedb6dcd2a22c38fe25e038d`  
		Last Modified: Mon, 17 Apr 2023 22:47:02 GMT  
		Size: 58.6 MB (58588139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a564ada930a970424e6b25a29d9d4f706d15f9e6401c21bcef3e841853f7527e`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539565d00e89aa08d29023b1284734fea67d9ff99366188c4ff29d0da6d59187`  
		Last Modified: Mon, 17 Apr 2023 22:47:03 GMT  
		Size: 56.6 MB (56562540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a06843fd5b834a3c6eb03387de3fcac84eb24f940ed1271579d2d76f137e6`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f6d4aa041d96e3ebda9dfafe42be4f7eed49456ba2c492adeffe85f10aad06`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.33` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:84dfe3825c21a0ec7e8e858b9ed118846bf096c1e0bc1a07458c04b393f2c7d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169785464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5371f8c3b63eec64a33b35530be5212d6148e0940111b57b689b5ba1ffe808c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:40:07 GMT
ADD file:c798bcae4b9271a204dc37f132bce1f0042c02cb1ad5a2237f56dec227d44438 in / 
# Thu, 06 Apr 2023 18:40:07 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:55:56 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:55:56 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:55:59 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:56:26 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:56:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:56:27 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:39:53 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:39:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:40:25 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:40:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:40:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:40:59 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:41:00 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:41:01 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:41:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:41:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:41:01 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:41:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6425367b44c9c3f59fd1e81f8fa2e9170ca2ef552d63f35a08ef3969ee4ff557`  
		Last Modified: Thu, 06 Apr 2023 18:40:43 GMT  
		Size: 43.5 MB (43477048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cef374d113a386d9e9eb540635c8e0d47e85deb38985982b5aeddc4798f67c7`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1751ddbc0d77eedc43d2aad156c590e2fec2c2f75fde0aef0757c69a0ba49f6d`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41e9e3c6d9abdfec73965f0105ee343f69e0c909c07b665ea81a2642e19365f`  
		Last Modified: Thu, 06 Apr 2023 18:57:58 GMT  
		Size: 4.5 MB (4465472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26e9c11cd2da41af092e3a224bcb367ba5201e02509f5e39bf009085eafe838`  
		Last Modified: Thu, 06 Apr 2023 18:57:57 GMT  
		Size: 2.6 KB (2627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ad8819238aa147cd2a97e255d96d27a755f14f31c8c0f3a0e2a66b0d7fa88`  
		Last Modified: Mon, 17 Apr 2023 22:41:24 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3028a5ad3fd0158e2835500be170a4877a5a73cb87680e42c6d49a9217051e6a`  
		Last Modified: Mon, 17 Apr 2023 22:41:29 GMT  
		Size: 57.9 MB (57858475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41584bf2c82e3943b457046f452be302b74a47ac1b299740871166e772ad4af`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413abbd4b9d17bb93f8402bc56f26c11a4c3d88c274d353b57b0072a682f7fa`  
		Last Modified: Mon, 17 Apr 2023 22:41:30 GMT  
		Size: 63.1 MB (63061793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7c55c30cf5aaea11b0b27ce0a8014a289e3b9032b39013cb6201e35c389924`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038fc84e09b5dcf7a11080675b9b0a54b30f71fc78a3eda72de1a328c1f061f0`  
		Last Modified: Mon, 17 Apr 2023 22:41:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.33-debian`

```console
$ docker pull mysql@sha256:8997d21bc7a8406c9ea3de932a25306091749e702a37d51aebafcf93beb3db2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.33-debian` - linux; amd64

```console
$ docker pull mysql@sha256:fc3550b4a91253802c92b328a2b064582d63197591e662a08d3e417e7326853b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179701768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11a2cc2219892cd270339bff1627493e4fb6f64c86567c5058da8aba128a1cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:15:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 May 2023 04:15:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:15:47 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 04:15:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 04:15:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 04:16:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:16:03 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 04:16:03 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 23 May 2023 04:16:03 GMT
ENV MYSQL_VERSION=8.0.33-1debian11
# Tue, 23 May 2023 04:16:04 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 May 2023 04:16:19 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 May 2023 04:16:20 GMT
VOLUME [/var/lib/mysql]
# Tue, 23 May 2023 04:16:20 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 23 May 2023 04:16:20 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 23 May 2023 04:16:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 04:16:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 04:16:21 GMT
EXPOSE 3306 33060
# Tue, 23 May 2023 04:16:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460bb444d52dab6a19d68cfcc664add2dd2ebb433465ed374770429b7b85ecf6`  
		Last Modified: Tue, 23 May 2023 04:17:36 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ceec72175ab896b5d2aae94caa4ad5ee8dc1eec8fbf86eda6c93dabc2d2b7b`  
		Last Modified: Tue, 23 May 2023 04:17:37 GMT  
		Size: 4.4 MB (4415030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca6f73d0c4e067456900a23eeda855c5a38bc7527c69a596f138baac0c06a5a`  
		Last Modified: Tue, 23 May 2023 04:17:35 GMT  
		Size: 1.5 MB (1471543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af5e268315b55d1318f7f5e708e8db3da0c9acd1d112b5cce069277aecc4e5`  
		Last Modified: Tue, 23 May 2023 04:17:34 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c12e7f453833e46579664261597f2f95c2a431caf865aadf793d1347ce1307`  
		Last Modified: Tue, 23 May 2023 04:17:37 GMT  
		Size: 12.7 MB (12661298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe8fac55990e5d5c61ee5ba24b86408236dcd4042d2b7802b5686605f8c1773`  
		Last Modified: Tue, 23 May 2023 04:17:34 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c00b032f6190d836908e7deb81e0b799be548829cb670b8e727e1b318695a`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da46d64fa01826465a87b81773db1102a8d174575ef9e512fc1fc36961826247`  
		Last Modified: Tue, 23 May 2023 04:17:50 GMT  
		Size: 129.7 MB (129739276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c38d2a0b5b87053ff6f692215d70e349dfed59ab3e0153ebaf24623092e334e`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d594c6498dbdf44ee78d77d380d5da7b3c336b2d902eaa2d7390ddbebf4e36c`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d10222ee5144f5619674bc5786fd9170447bc57d66081d3081246677f10d4c`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.33-oracle`

```console
$ docker pull mysql@sha256:a43f6e7e7f3a5e5b90f857fbed4e3103ece771b19f0f75880f767cf66bbb6577
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.33-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:b45a7c3e6fb15526e8bf62ebb940cd460617e36f46155b8514fd9c9388231817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165315366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8189e588b0e8fcc95b0d764d6f7bdb55b5b41e9249157177d73781058f603ca9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:20:31 GMT
ADD file:61a2085af5116916e7b117c2e7ad7116bdc0282d8fa9ce76191c4101f5e866ff in / 
# Thu, 06 Apr 2023 18:20:32 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:43:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:43:29 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:43:32 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:43:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:43:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:43:58 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:43:23 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:43:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:43:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:43:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:43:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:44:32 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:44:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:44:33 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:44:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:44:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:44:34 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:44:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:328ba678bf27575937f8b9dfbf5b5f39b21941af068f8e5960de8131e289da85`  
		Last Modified: Thu, 06 Apr 2023 18:21:19 GMT  
		Size: 44.6 MB (44563902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f5ff008d73bef1d4c8e1a4c73a7efc7697e8087a950065fb369c83a03df08d`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7054d6d0c7c57672cd9e48e8a92eda15a4f0ae24dc78413fdce3fce3064a77`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b5d4e8750e78990227fa3f3df12b6ccdf3b2486b4248677b7959dd95c0e77b`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 4.6 MB (4608287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc4a7b43bdd822158ae54cac5da309097088de0253879cbb07e31829d8f4561`  
		Last Modified: Thu, 06 Apr 2023 18:45:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0608f8959e036b9e5f55227da2fac404f45e153119063fd042cba4cdcdc9e6c`  
		Last Modified: Mon, 17 Apr 2023 22:46:55 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5823e721608fd3d82b87e136e4cb898d8ffbbf25cedb6dcd2a22c38fe25e038d`  
		Last Modified: Mon, 17 Apr 2023 22:47:02 GMT  
		Size: 58.6 MB (58588139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a564ada930a970424e6b25a29d9d4f706d15f9e6401c21bcef3e841853f7527e`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539565d00e89aa08d29023b1284734fea67d9ff99366188c4ff29d0da6d59187`  
		Last Modified: Mon, 17 Apr 2023 22:47:03 GMT  
		Size: 56.6 MB (56562540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a06843fd5b834a3c6eb03387de3fcac84eb24f940ed1271579d2d76f137e6`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f6d4aa041d96e3ebda9dfafe42be4f7eed49456ba2c492adeffe85f10aad06`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.33-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:84dfe3825c21a0ec7e8e858b9ed118846bf096c1e0bc1a07458c04b393f2c7d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169785464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5371f8c3b63eec64a33b35530be5212d6148e0940111b57b689b5ba1ffe808c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:40:07 GMT
ADD file:c798bcae4b9271a204dc37f132bce1f0042c02cb1ad5a2237f56dec227d44438 in / 
# Thu, 06 Apr 2023 18:40:07 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:55:56 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:55:56 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:55:59 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:56:26 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:56:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:56:27 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:39:53 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:39:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:40:25 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:40:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:40:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:40:59 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:41:00 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:41:01 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:41:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:41:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:41:01 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:41:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6425367b44c9c3f59fd1e81f8fa2e9170ca2ef552d63f35a08ef3969ee4ff557`  
		Last Modified: Thu, 06 Apr 2023 18:40:43 GMT  
		Size: 43.5 MB (43477048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cef374d113a386d9e9eb540635c8e0d47e85deb38985982b5aeddc4798f67c7`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1751ddbc0d77eedc43d2aad156c590e2fec2c2f75fde0aef0757c69a0ba49f6d`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41e9e3c6d9abdfec73965f0105ee343f69e0c909c07b665ea81a2642e19365f`  
		Last Modified: Thu, 06 Apr 2023 18:57:58 GMT  
		Size: 4.5 MB (4465472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26e9c11cd2da41af092e3a224bcb367ba5201e02509f5e39bf009085eafe838`  
		Last Modified: Thu, 06 Apr 2023 18:57:57 GMT  
		Size: 2.6 KB (2627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ad8819238aa147cd2a97e255d96d27a755f14f31c8c0f3a0e2a66b0d7fa88`  
		Last Modified: Mon, 17 Apr 2023 22:41:24 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3028a5ad3fd0158e2835500be170a4877a5a73cb87680e42c6d49a9217051e6a`  
		Last Modified: Mon, 17 Apr 2023 22:41:29 GMT  
		Size: 57.9 MB (57858475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41584bf2c82e3943b457046f452be302b74a47ac1b299740871166e772ad4af`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413abbd4b9d17bb93f8402bc56f26c11a4c3d88c274d353b57b0072a682f7fa`  
		Last Modified: Mon, 17 Apr 2023 22:41:30 GMT  
		Size: 63.1 MB (63061793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7c55c30cf5aaea11b0b27ce0a8014a289e3b9032b39013cb6201e35c389924`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038fc84e09b5dcf7a11080675b9b0a54b30f71fc78a3eda72de1a328c1f061f0`  
		Last Modified: Mon, 17 Apr 2023 22:41:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:8997d21bc7a8406c9ea3de932a25306091749e702a37d51aebafcf93beb3db2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:fc3550b4a91253802c92b328a2b064582d63197591e662a08d3e417e7326853b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179701768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e11a2cc2219892cd270339bff1627493e4fb6f64c86567c5058da8aba128a1cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:15:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 May 2023 04:15:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:15:47 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 04:15:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 04:15:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 04:16:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:16:03 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 04:16:03 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 23 May 2023 04:16:03 GMT
ENV MYSQL_VERSION=8.0.33-1debian11
# Tue, 23 May 2023 04:16:04 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 May 2023 04:16:19 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 May 2023 04:16:20 GMT
VOLUME [/var/lib/mysql]
# Tue, 23 May 2023 04:16:20 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 23 May 2023 04:16:20 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 23 May 2023 04:16:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 04:16:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 04:16:21 GMT
EXPOSE 3306 33060
# Tue, 23 May 2023 04:16:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460bb444d52dab6a19d68cfcc664add2dd2ebb433465ed374770429b7b85ecf6`  
		Last Modified: Tue, 23 May 2023 04:17:36 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ceec72175ab896b5d2aae94caa4ad5ee8dc1eec8fbf86eda6c93dabc2d2b7b`  
		Last Modified: Tue, 23 May 2023 04:17:37 GMT  
		Size: 4.4 MB (4415030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca6f73d0c4e067456900a23eeda855c5a38bc7527c69a596f138baac0c06a5a`  
		Last Modified: Tue, 23 May 2023 04:17:35 GMT  
		Size: 1.5 MB (1471543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37af5e268315b55d1318f7f5e708e8db3da0c9acd1d112b5cce069277aecc4e5`  
		Last Modified: Tue, 23 May 2023 04:17:34 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c12e7f453833e46579664261597f2f95c2a431caf865aadf793d1347ce1307`  
		Last Modified: Tue, 23 May 2023 04:17:37 GMT  
		Size: 12.7 MB (12661298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe8fac55990e5d5c61ee5ba24b86408236dcd4042d2b7802b5686605f8c1773`  
		Last Modified: Tue, 23 May 2023 04:17:34 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c00b032f6190d836908e7deb81e0b799be548829cb670b8e727e1b318695a`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da46d64fa01826465a87b81773db1102a8d174575ef9e512fc1fc36961826247`  
		Last Modified: Tue, 23 May 2023 04:17:50 GMT  
		Size: 129.7 MB (129739276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c38d2a0b5b87053ff6f692215d70e349dfed59ab3e0153ebaf24623092e334e`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d594c6498dbdf44ee78d77d380d5da7b3c336b2d902eaa2d7390ddbebf4e36c`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d10222ee5144f5619674bc5786fd9170447bc57d66081d3081246677f10d4c`  
		Last Modified: Tue, 23 May 2023 04:17:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:a43f6e7e7f3a5e5b90f857fbed4e3103ece771b19f0f75880f767cf66bbb6577
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:b45a7c3e6fb15526e8bf62ebb940cd460617e36f46155b8514fd9c9388231817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165315366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8189e588b0e8fcc95b0d764d6f7bdb55b5b41e9249157177d73781058f603ca9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:20:31 GMT
ADD file:61a2085af5116916e7b117c2e7ad7116bdc0282d8fa9ce76191c4101f5e866ff in / 
# Thu, 06 Apr 2023 18:20:32 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:43:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:43:29 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:43:32 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:43:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:43:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:43:58 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:43:23 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:43:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:43:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:43:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:43:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:44:32 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:44:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:44:33 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:44:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:44:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:44:34 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:44:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:328ba678bf27575937f8b9dfbf5b5f39b21941af068f8e5960de8131e289da85`  
		Last Modified: Thu, 06 Apr 2023 18:21:19 GMT  
		Size: 44.6 MB (44563902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f5ff008d73bef1d4c8e1a4c73a7efc7697e8087a950065fb369c83a03df08d`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7054d6d0c7c57672cd9e48e8a92eda15a4f0ae24dc78413fdce3fce3064a77`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b5d4e8750e78990227fa3f3df12b6ccdf3b2486b4248677b7959dd95c0e77b`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 4.6 MB (4608287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc4a7b43bdd822158ae54cac5da309097088de0253879cbb07e31829d8f4561`  
		Last Modified: Thu, 06 Apr 2023 18:45:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0608f8959e036b9e5f55227da2fac404f45e153119063fd042cba4cdcdc9e6c`  
		Last Modified: Mon, 17 Apr 2023 22:46:55 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5823e721608fd3d82b87e136e4cb898d8ffbbf25cedb6dcd2a22c38fe25e038d`  
		Last Modified: Mon, 17 Apr 2023 22:47:02 GMT  
		Size: 58.6 MB (58588139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a564ada930a970424e6b25a29d9d4f706d15f9e6401c21bcef3e841853f7527e`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539565d00e89aa08d29023b1284734fea67d9ff99366188c4ff29d0da6d59187`  
		Last Modified: Mon, 17 Apr 2023 22:47:03 GMT  
		Size: 56.6 MB (56562540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a06843fd5b834a3c6eb03387de3fcac84eb24f940ed1271579d2d76f137e6`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f6d4aa041d96e3ebda9dfafe42be4f7eed49456ba2c492adeffe85f10aad06`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:84dfe3825c21a0ec7e8e858b9ed118846bf096c1e0bc1a07458c04b393f2c7d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169785464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5371f8c3b63eec64a33b35530be5212d6148e0940111b57b689b5ba1ffe808c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:40:07 GMT
ADD file:c798bcae4b9271a204dc37f132bce1f0042c02cb1ad5a2237f56dec227d44438 in / 
# Thu, 06 Apr 2023 18:40:07 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:55:56 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:55:56 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:55:59 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:56:26 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:56:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:56:27 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:39:53 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:39:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:40:25 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:40:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:40:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:40:59 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:41:00 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:41:01 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:41:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:41:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:41:01 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:41:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6425367b44c9c3f59fd1e81f8fa2e9170ca2ef552d63f35a08ef3969ee4ff557`  
		Last Modified: Thu, 06 Apr 2023 18:40:43 GMT  
		Size: 43.5 MB (43477048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cef374d113a386d9e9eb540635c8e0d47e85deb38985982b5aeddc4798f67c7`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1751ddbc0d77eedc43d2aad156c590e2fec2c2f75fde0aef0757c69a0ba49f6d`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41e9e3c6d9abdfec73965f0105ee343f69e0c909c07b665ea81a2642e19365f`  
		Last Modified: Thu, 06 Apr 2023 18:57:58 GMT  
		Size: 4.5 MB (4465472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26e9c11cd2da41af092e3a224bcb367ba5201e02509f5e39bf009085eafe838`  
		Last Modified: Thu, 06 Apr 2023 18:57:57 GMT  
		Size: 2.6 KB (2627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ad8819238aa147cd2a97e255d96d27a755f14f31c8c0f3a0e2a66b0d7fa88`  
		Last Modified: Mon, 17 Apr 2023 22:41:24 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3028a5ad3fd0158e2835500be170a4877a5a73cb87680e42c6d49a9217051e6a`  
		Last Modified: Mon, 17 Apr 2023 22:41:29 GMT  
		Size: 57.9 MB (57858475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41584bf2c82e3943b457046f452be302b74a47ac1b299740871166e772ad4af`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413abbd4b9d17bb93f8402bc56f26c11a4c3d88c274d353b57b0072a682f7fa`  
		Last Modified: Mon, 17 Apr 2023 22:41:30 GMT  
		Size: 63.1 MB (63061793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7c55c30cf5aaea11b0b27ce0a8014a289e3b9032b39013cb6201e35c389924`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038fc84e09b5dcf7a11080675b9b0a54b30f71fc78a3eda72de1a328c1f061f0`  
		Last Modified: Mon, 17 Apr 2023 22:41:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:a43f6e7e7f3a5e5b90f857fbed4e3103ece771b19f0f75880f767cf66bbb6577
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:b45a7c3e6fb15526e8bf62ebb940cd460617e36f46155b8514fd9c9388231817
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165315366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8189e588b0e8fcc95b0d764d6f7bdb55b5b41e9249157177d73781058f603ca9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:20:31 GMT
ADD file:61a2085af5116916e7b117c2e7ad7116bdc0282d8fa9ce76191c4101f5e866ff in / 
# Thu, 06 Apr 2023 18:20:32 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:43:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:43:29 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:43:32 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:43:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:43:58 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:43:58 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:43:23 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:43:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:43:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:43:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:43:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:44:32 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:44:33 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:44:33 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:44:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:44:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:44:34 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:44:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:328ba678bf27575937f8b9dfbf5b5f39b21941af068f8e5960de8131e289da85`  
		Last Modified: Thu, 06 Apr 2023 18:21:19 GMT  
		Size: 44.6 MB (44563902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f5ff008d73bef1d4c8e1a4c73a7efc7697e8087a950065fb369c83a03df08d`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7054d6d0c7c57672cd9e48e8a92eda15a4f0ae24dc78413fdce3fce3064a77`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b5d4e8750e78990227fa3f3df12b6ccdf3b2486b4248677b7959dd95c0e77b`  
		Last Modified: Thu, 06 Apr 2023 18:45:41 GMT  
		Size: 4.6 MB (4608287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc4a7b43bdd822158ae54cac5da309097088de0253879cbb07e31829d8f4561`  
		Last Modified: Thu, 06 Apr 2023 18:45:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0608f8959e036b9e5f55227da2fac404f45e153119063fd042cba4cdcdc9e6c`  
		Last Modified: Mon, 17 Apr 2023 22:46:55 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5823e721608fd3d82b87e136e4cb898d8ffbbf25cedb6dcd2a22c38fe25e038d`  
		Last Modified: Mon, 17 Apr 2023 22:47:02 GMT  
		Size: 58.6 MB (58588139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a564ada930a970424e6b25a29d9d4f706d15f9e6401c21bcef3e841853f7527e`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539565d00e89aa08d29023b1284734fea67d9ff99366188c4ff29d0da6d59187`  
		Last Modified: Mon, 17 Apr 2023 22:47:03 GMT  
		Size: 56.6 MB (56562540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a06843fd5b834a3c6eb03387de3fcac84eb24f940ed1271579d2d76f137e6`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f6d4aa041d96e3ebda9dfafe42be4f7eed49456ba2c492adeffe85f10aad06`  
		Last Modified: Mon, 17 Apr 2023 22:46:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:84dfe3825c21a0ec7e8e858b9ed118846bf096c1e0bc1a07458c04b393f2c7d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169785464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5371f8c3b63eec64a33b35530be5212d6148e0940111b57b689b5ba1ffe808c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 06 Apr 2023 18:40:07 GMT
ADD file:c798bcae4b9271a204dc37f132bce1f0042c02cb1ad5a2237f56dec227d44438 in / 
# Thu, 06 Apr 2023 18:40:07 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:55:56 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 06 Apr 2023 18:55:56 GMT
ENV GOSU_VERSION=1.16
# Thu, 06 Apr 2023 18:55:59 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 06 Apr 2023 18:56:26 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:56:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 06 Apr 2023 18:56:27 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 17 Apr 2023 22:39:53 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:39:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Mon, 17 Apr 2023 22:40:25 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Mon, 17 Apr 2023 22:40:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Mon, 17 Apr 2023 22:40:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Mon, 17 Apr 2023 22:40:59 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Mon, 17 Apr 2023 22:41:00 GMT
VOLUME [/var/lib/mysql]
# Mon, 17 Apr 2023 22:41:01 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Mon, 17 Apr 2023 22:41:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 17 Apr 2023 22:41:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 22:41:01 GMT
EXPOSE 3306 33060
# Mon, 17 Apr 2023 22:41:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6425367b44c9c3f59fd1e81f8fa2e9170ca2ef552d63f35a08ef3969ee4ff557`  
		Last Modified: Thu, 06 Apr 2023 18:40:43 GMT  
		Size: 43.5 MB (43477048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cef374d113a386d9e9eb540635c8e0d47e85deb38985982b5aeddc4798f67c7`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1751ddbc0d77eedc43d2aad156c590e2fec2c2f75fde0aef0757c69a0ba49f6d`  
		Last Modified: Thu, 06 Apr 2023 18:57:59 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41e9e3c6d9abdfec73965f0105ee343f69e0c909c07b665ea81a2642e19365f`  
		Last Modified: Thu, 06 Apr 2023 18:57:58 GMT  
		Size: 4.5 MB (4465472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26e9c11cd2da41af092e3a224bcb367ba5201e02509f5e39bf009085eafe838`  
		Last Modified: Thu, 06 Apr 2023 18:57:57 GMT  
		Size: 2.6 KB (2627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:949ad8819238aa147cd2a97e255d96d27a755f14f31c8c0f3a0e2a66b0d7fa88`  
		Last Modified: Mon, 17 Apr 2023 22:41:24 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3028a5ad3fd0158e2835500be170a4877a5a73cb87680e42c6d49a9217051e6a`  
		Last Modified: Mon, 17 Apr 2023 22:41:29 GMT  
		Size: 57.9 MB (57858475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41584bf2c82e3943b457046f452be302b74a47ac1b299740871166e772ad4af`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f413abbd4b9d17bb93f8402bc56f26c11a4c3d88c274d353b57b0072a682f7fa`  
		Last Modified: Mon, 17 Apr 2023 22:41:30 GMT  
		Size: 63.1 MB (63061793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7c55c30cf5aaea11b0b27ce0a8014a289e3b9032b39013cb6201e35c389924`  
		Last Modified: Mon, 17 Apr 2023 22:41:22 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038fc84e09b5dcf7a11080675b9b0a54b30f71fc78a3eda72de1a328c1f061f0`  
		Last Modified: Mon, 17 Apr 2023 22:41:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
