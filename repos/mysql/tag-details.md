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
$ docker pull mysql@sha256:d6eb81d0d1d275bf111d36217a5499edacc65dae26d6eddcc286bd347626c386
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c5ba2bb0a388f5a942c2e57573c46d728420759f56667fd182ba87f1529446a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.8 MB (162760668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b50a7c7212c73512d40453f183228802e175a8b3b58e3665d3787efde78fbb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:32 GMT
ADD file:2818e508d01da2188fb234b38fb19aa1ea9eeeae92d361ecdf49318d949f51a9 in / 
# Mon, 12 Jun 2023 23:21:32 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:06:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jun 2023 07:06:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:07:00 GMT
ENV GOSU_VERSION=1.16
# Tue, 13 Jun 2023 07:07:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jun 2023 07:07:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jun 2023 07:07:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:07:15 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 13 Jun 2023 07:07:16 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 13 Jun 2023 07:07:16 GMT
ENV MYSQL_VERSION=5.7.42-1debian10
# Tue, 13 Jun 2023 07:07:16 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Jun 2023 07:07:34 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 13 Jun 2023 07:07:35 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jun 2023 07:07:35 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 13 Jun 2023 07:07:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 07:07:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:07:36 GMT
EXPOSE 3306 33060
# Tue, 13 Jun 2023 07:07:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8b91b88d557765cd8c6802668755a3f6dc4337b6ce15a17e4857139e5fc964f3`  
		Last Modified: Mon, 12 Jun 2023 23:27:09 GMT  
		Size: 27.1 MB (27138450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1aeca2c9fbf2100ffc22b3bfe6f2b5c7f1de7ed27c0b122663da75432ff97e`  
		Last Modified: Tue, 13 Jun 2023 07:08:32 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1328249caf09a7fc1a4a64e2546b4f85d37d952dcbed579d64dc254dd5fed9`  
		Last Modified: Tue, 13 Jun 2023 07:08:31 GMT  
		Size: 4.2 MB (4182342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a3600e7a67a8c00083b943cbea50beae4db2ef2904892f8f61c1d02ef124b9`  
		Last Modified: Tue, 13 Jun 2023 07:08:31 GMT  
		Size: 1.4 MB (1441847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db640288c92352c0d9d5d7f5a668a8b5464949b0192518064424ac8e566db1c4`  
		Last Modified: Tue, 13 Jun 2023 07:08:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5720c8c171eeba38399539c920a4e647e62439357cb060b68597b8d5cdfec764`  
		Last Modified: Tue, 13 Jun 2023 07:08:33 GMT  
		Size: 14.1 MB (14089564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fae3f80815695c631160e31ede4a5c55794b99420d6a3b1623bc9b6c0b23fb8`  
		Last Modified: Tue, 13 Jun 2023 07:08:28 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666445987696f03c0ad687ed75d8d91f232fa203b0615364e0d4945c24b6d1a2`  
		Last Modified: Tue, 13 Jun 2023 07:08:28 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d70e247cb2fc90b9c8859a7738c258c6c184dd43b4383b24a01ddde3c02ba23`  
		Last Modified: Tue, 13 Jun 2023 07:08:43 GMT  
		Size: 115.9 MB (115898280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1959a8ae768d2ca49266734c3c2fb6401779c0679d79b0b92f26cd592754e5`  
		Last Modified: Tue, 13 Jun 2023 07:08:28 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c553533f68faaf92f715ee5ff1ffaae402012d4f15e5b2878a0e98a781197346`  
		Last Modified: Tue, 13 Jun 2023 07:08:29 GMT  
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
$ docker pull mysql@sha256:d6eb81d0d1d275bf111d36217a5499edacc65dae26d6eddcc286bd347626c386
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c5ba2bb0a388f5a942c2e57573c46d728420759f56667fd182ba87f1529446a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.8 MB (162760668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b50a7c7212c73512d40453f183228802e175a8b3b58e3665d3787efde78fbb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:32 GMT
ADD file:2818e508d01da2188fb234b38fb19aa1ea9eeeae92d361ecdf49318d949f51a9 in / 
# Mon, 12 Jun 2023 23:21:32 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:06:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jun 2023 07:06:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:07:00 GMT
ENV GOSU_VERSION=1.16
# Tue, 13 Jun 2023 07:07:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jun 2023 07:07:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jun 2023 07:07:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:07:15 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 13 Jun 2023 07:07:16 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 13 Jun 2023 07:07:16 GMT
ENV MYSQL_VERSION=5.7.42-1debian10
# Tue, 13 Jun 2023 07:07:16 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Jun 2023 07:07:34 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 13 Jun 2023 07:07:35 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jun 2023 07:07:35 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 13 Jun 2023 07:07:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 07:07:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:07:36 GMT
EXPOSE 3306 33060
# Tue, 13 Jun 2023 07:07:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8b91b88d557765cd8c6802668755a3f6dc4337b6ce15a17e4857139e5fc964f3`  
		Last Modified: Mon, 12 Jun 2023 23:27:09 GMT  
		Size: 27.1 MB (27138450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1aeca2c9fbf2100ffc22b3bfe6f2b5c7f1de7ed27c0b122663da75432ff97e`  
		Last Modified: Tue, 13 Jun 2023 07:08:32 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1328249caf09a7fc1a4a64e2546b4f85d37d952dcbed579d64dc254dd5fed9`  
		Last Modified: Tue, 13 Jun 2023 07:08:31 GMT  
		Size: 4.2 MB (4182342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a3600e7a67a8c00083b943cbea50beae4db2ef2904892f8f61c1d02ef124b9`  
		Last Modified: Tue, 13 Jun 2023 07:08:31 GMT  
		Size: 1.4 MB (1441847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db640288c92352c0d9d5d7f5a668a8b5464949b0192518064424ac8e566db1c4`  
		Last Modified: Tue, 13 Jun 2023 07:08:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5720c8c171eeba38399539c920a4e647e62439357cb060b68597b8d5cdfec764`  
		Last Modified: Tue, 13 Jun 2023 07:08:33 GMT  
		Size: 14.1 MB (14089564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fae3f80815695c631160e31ede4a5c55794b99420d6a3b1623bc9b6c0b23fb8`  
		Last Modified: Tue, 13 Jun 2023 07:08:28 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666445987696f03c0ad687ed75d8d91f232fa203b0615364e0d4945c24b6d1a2`  
		Last Modified: Tue, 13 Jun 2023 07:08:28 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d70e247cb2fc90b9c8859a7738c258c6c184dd43b4383b24a01ddde3c02ba23`  
		Last Modified: Tue, 13 Jun 2023 07:08:43 GMT  
		Size: 115.9 MB (115898280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1959a8ae768d2ca49266734c3c2fb6401779c0679d79b0b92f26cd592754e5`  
		Last Modified: Tue, 13 Jun 2023 07:08:28 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c553533f68faaf92f715ee5ff1ffaae402012d4f15e5b2878a0e98a781197346`  
		Last Modified: Tue, 13 Jun 2023 07:08:29 GMT  
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
$ docker pull mysql@sha256:d6eb81d0d1d275bf111d36217a5499edacc65dae26d6eddcc286bd347626c386
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.42-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c5ba2bb0a388f5a942c2e57573c46d728420759f56667fd182ba87f1529446a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.8 MB (162760668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b50a7c7212c73512d40453f183228802e175a8b3b58e3665d3787efde78fbb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:32 GMT
ADD file:2818e508d01da2188fb234b38fb19aa1ea9eeeae92d361ecdf49318d949f51a9 in / 
# Mon, 12 Jun 2023 23:21:32 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:06:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jun 2023 07:06:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:07:00 GMT
ENV GOSU_VERSION=1.16
# Tue, 13 Jun 2023 07:07:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jun 2023 07:07:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jun 2023 07:07:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:07:15 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 13 Jun 2023 07:07:16 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 13 Jun 2023 07:07:16 GMT
ENV MYSQL_VERSION=5.7.42-1debian10
# Tue, 13 Jun 2023 07:07:16 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Jun 2023 07:07:34 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 13 Jun 2023 07:07:35 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jun 2023 07:07:35 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 13 Jun 2023 07:07:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 07:07:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:07:36 GMT
EXPOSE 3306 33060
# Tue, 13 Jun 2023 07:07:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8b91b88d557765cd8c6802668755a3f6dc4337b6ce15a17e4857139e5fc964f3`  
		Last Modified: Mon, 12 Jun 2023 23:27:09 GMT  
		Size: 27.1 MB (27138450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1aeca2c9fbf2100ffc22b3bfe6f2b5c7f1de7ed27c0b122663da75432ff97e`  
		Last Modified: Tue, 13 Jun 2023 07:08:32 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1328249caf09a7fc1a4a64e2546b4f85d37d952dcbed579d64dc254dd5fed9`  
		Last Modified: Tue, 13 Jun 2023 07:08:31 GMT  
		Size: 4.2 MB (4182342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a3600e7a67a8c00083b943cbea50beae4db2ef2904892f8f61c1d02ef124b9`  
		Last Modified: Tue, 13 Jun 2023 07:08:31 GMT  
		Size: 1.4 MB (1441847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db640288c92352c0d9d5d7f5a668a8b5464949b0192518064424ac8e566db1c4`  
		Last Modified: Tue, 13 Jun 2023 07:08:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5720c8c171eeba38399539c920a4e647e62439357cb060b68597b8d5cdfec764`  
		Last Modified: Tue, 13 Jun 2023 07:08:33 GMT  
		Size: 14.1 MB (14089564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fae3f80815695c631160e31ede4a5c55794b99420d6a3b1623bc9b6c0b23fb8`  
		Last Modified: Tue, 13 Jun 2023 07:08:28 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666445987696f03c0ad687ed75d8d91f232fa203b0615364e0d4945c24b6d1a2`  
		Last Modified: Tue, 13 Jun 2023 07:08:28 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d70e247cb2fc90b9c8859a7738c258c6c184dd43b4383b24a01ddde3c02ba23`  
		Last Modified: Tue, 13 Jun 2023 07:08:43 GMT  
		Size: 115.9 MB (115898280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1959a8ae768d2ca49266734c3c2fb6401779c0679d79b0b92f26cd592754e5`  
		Last Modified: Tue, 13 Jun 2023 07:08:28 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c553533f68faaf92f715ee5ff1ffaae402012d4f15e5b2878a0e98a781197346`  
		Last Modified: Tue, 13 Jun 2023 07:08:29 GMT  
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
$ docker pull mysql@sha256:4bae98614cd6ad1aecbdd32ff1b37b93fb0ee22b069469e7bc9679bacef1abd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:1717a37c2adc7772b569eb727bb198b6792f7d50c2adb4839ba637b5c9d88f42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165659693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71276df4a871c5c09ff8411247609cc9683d85290f9dc9b1871dd6e366a28f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sun, 04 Jun 2023 17:54:32 GMT
ADD file:39d09c6c7c3a0f64981f5cbcb12cc8f0128979c3d4b91d74c84fe62aca5ea87e in / 
# Sun, 04 Jun 2023 17:54:32 GMT
CMD ["/bin/bash"]
# Sun, 04 Jun 2023 18:53:08 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sun, 04 Jun 2023 18:53:08 GMT
ENV GOSU_VERSION=1.16
# Sun, 04 Jun 2023 18:53:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 04 Jun 2023 18:53:38 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_MAJOR=8.0
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sun, 04 Jun 2023 18:54:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sun, 04 Jun 2023 18:54:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sun, 04 Jun 2023 18:54:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:54:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sun, 04 Jun 2023 18:54:53 GMT
VOLUME [/var/lib/mysql]
# Sun, 04 Jun 2023 18:54:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sun, 04 Jun 2023 18:54:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sun, 04 Jun 2023 18:54:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 04 Jun 2023 18:54:53 GMT
EXPOSE 3306 33060
# Sun, 04 Jun 2023 18:54:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3e0c3751e6482e67b70ffad144b2cb9aec9be672df2642a322e875e51b748aeb`  
		Last Modified: Sun, 04 Jun 2023 17:55:32 GMT  
		Size: 44.9 MB (44872720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7914193c6f0e6bf32545a75c783e4f919ef1fd267a806876c5d2f72da6c4be54`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4b3f820487ae4bd2869d410c4e4dc497042a73306e0ba99071b261e33190c1`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 982.8 KB (982825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63683b304e3d24e14589c48906cad17ead6bdf22ecf67b6291c12f5bc1544ec3`  
		Last Modified: Sun, 04 Jun 2023 18:55:21 GMT  
		Size: 4.6 MB (4614163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad9069836bd68adbe6be6e2c3aab749575e961266cd5ca27831330c21bb80d7`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90cd4c0e5df7a54d89ca2140cf329f530b89fe8c79de8873c66cfada8f5de6`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892e565e2cf01a43d9d6d4b4053893b1b1ea7c36b5b77965eabe762292eb491b`  
		Last Modified: Sun, 04 Jun 2023 18:55:26 GMT  
		Size: 58.6 MB (58610758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73057d123da0d3d34811ea0383a736c549907f639c24ab1bf576813c3ad40ba8`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1a3c0ec34ee20aec3f319f1f72ab7e94a9171b755be01adc71c30b19406ecb`  
		Last Modified: Sun, 04 Jun 2023 18:55:28 GMT  
		Size: 56.6 MB (56569548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fe8dc4ffe938cf78e257d45b0831df9a5053470ebed1d6978a85d061cb6dad`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807488ae889657196a0f63400133a21d65d2ed24ecb1a05faed222acdbeac0d`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a1e67f2bd2f3e36f387146ce6e6de3eb6d318aaec480a64d5a3a1506abf85275
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170106612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3077e10c878f57a4beaa0255cb581855b32118f5c2a8eef0b2c21373644541f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Jun 2023 22:40:44 GMT
ADD file:ae7c6036695430900f5ff735197e9c0281881b97faaea00e40263ca539fe7fff in / 
# Fri, 02 Jun 2023 22:40:45 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 22:58:57 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 02 Jun 2023 22:58:57 GMT
ENV GOSU_VERSION=1.16
# Fri, 02 Jun 2023 22:59:01 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Jun 2023 22:59:24 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 02 Jun 2023 22:59:54 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 02 Jun 2023 22:59:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 02 Jun 2023 22:59:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 23:00:28 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 02 Jun 2023 23:00:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Jun 2023 23:00:29 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 02 Jun 2023 23:00:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 02 Jun 2023 23:00:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 23:00:30 GMT
EXPOSE 3306 33060
# Fri, 02 Jun 2023 23:00:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ae143351a4fc570e80462825e827f3afbbabc4488aeae617542d42b521e5248`  
		Last Modified: Fri, 02 Jun 2023 22:41:37 GMT  
		Size: 43.8 MB (43787831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093b9ff06d4876e70f2620f141826cb4539ec8d199cca617013af6beea55bdc3`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf4f7b0363a59d4c3b6b8d9512406253633fbde87965376d96c2442a4d5d1ed`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8614746438f21c27808fe28de1009dc4791c5851e4ca822fc157f54970923c5`  
		Last Modified: Fri, 02 Jun 2023 23:00:44 GMT  
		Size: 4.5 MB (4456832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5aab2c5597c573d9d6efaf363a1e8e5672c55662832d2b559b4e263a763d1`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3e9a25efeb16879304ef4e09266c7562be10d36aebceda5acc9306165a433c`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1388739c015dac6d48f069dd3244dbe9016951625da6a8b94e5fb61b1fba9ff`  
		Last Modified: Fri, 02 Jun 2023 23:00:48 GMT  
		Size: 57.9 MB (57878613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a7da0e25e17bcf1d323a8477e936e2a1b2b569d07401d2dd4738828be7905b`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b0d0608a32def0b1d2c00a2ae8125fa493b15ccaa671ba53adf2364ca189c4`  
		Last Modified: Fri, 02 Jun 2023 23:00:49 GMT  
		Size: 63.1 MB (63060665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4191a53ea864946096ec2cba1542292cb1bf95072cae75675b26fae50a2bf64`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36880be7ebcb33b29760e2c596f17ac2f79e8bbc6b0f07a8b3ace99ed4a67d`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:ee1e7bf1a6c7f7fc26abbbed04b6e0ab6f202b48c50ef8f418324901420b207e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:8dd2269034dd8680a2d90403977c9604bbaeb0e30364d105340a50241245785c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179716143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7faa2f9a3fde46c5e8c2d1b5c8d0fb9372a5707162e3b2826fe59478a54cce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:06:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jun 2023 07:06:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:06:17 GMT
ENV GOSU_VERSION=1.16
# Tue, 13 Jun 2023 07:06:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jun 2023 07:06:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jun 2023 07:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:06:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 13 Jun 2023 07:06:32 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 13 Jun 2023 07:06:32 GMT
ENV MYSQL_VERSION=8.0.33-1debian11
# Tue, 13 Jun 2023 07:06:33 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Jun 2023 07:06:47 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 13 Jun 2023 07:06:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jun 2023 07:06:48 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 13 Jun 2023 07:06:48 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 13 Jun 2023 07:06:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 07:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:06:49 GMT
EXPOSE 3306 33060
# Tue, 13 Jun 2023 07:06:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe03a6bd2ae95b6630c019ae5bf8e7351c8f27095d7fa0fb9a0deb3a6a56d515`  
		Last Modified: Tue, 13 Jun 2023 07:07:58 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe98fd0054daa6f38d2c1aaeff6b257d29ba86de74067a273764fb9801b4df9`  
		Last Modified: Tue, 13 Jun 2023 07:07:59 GMT  
		Size: 4.4 MB (4414989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b46f788fa0e3949eb16f96da627627fef28391e6788017828fdc59d85e1e47`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 1.5 MB (1471490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a574d9be7097a3158569d7be3fe8f58245d2a1160a02322df42cc21ed4da6305`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32a1a43aaf90ecca1eaecc5cbdade060ae64eb3ad5c0164d3f7fdfa6df36c22`  
		Last Modified: Tue, 13 Jun 2023 07:07:59 GMT  
		Size: 12.7 MB (12662026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1168cde172f4894d8388f45337512f3c50e31b0052297b85690542a846df34f6`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db9de6fbb6e12066dfb465bb744c8874637465cb32df5af3b7bdc1853d1f07e`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7597d1f876243f8e8f404c3f283ef6cbbdba1f7a9e6dd0382d87b0c52a1c7286`  
		Last Modified: Tue, 13 Jun 2023 07:08:13 GMT  
		Size: 129.7 MB (129739199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90525318623af863af49636e05796881027a61b6c6f6f673755105a58f6e1ff`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569dbc33ff4adc1218e4182f4ef79c728b2ece52f04ab884388496922b9c38f5`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765dd48ed85e84d520ae837a9e4fa93353bff6066721a0b41e484f1baeaa4194`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:4bae98614cd6ad1aecbdd32ff1b37b93fb0ee22b069469e7bc9679bacef1abd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1717a37c2adc7772b569eb727bb198b6792f7d50c2adb4839ba637b5c9d88f42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165659693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71276df4a871c5c09ff8411247609cc9683d85290f9dc9b1871dd6e366a28f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sun, 04 Jun 2023 17:54:32 GMT
ADD file:39d09c6c7c3a0f64981f5cbcb12cc8f0128979c3d4b91d74c84fe62aca5ea87e in / 
# Sun, 04 Jun 2023 17:54:32 GMT
CMD ["/bin/bash"]
# Sun, 04 Jun 2023 18:53:08 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sun, 04 Jun 2023 18:53:08 GMT
ENV GOSU_VERSION=1.16
# Sun, 04 Jun 2023 18:53:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 04 Jun 2023 18:53:38 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_MAJOR=8.0
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sun, 04 Jun 2023 18:54:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sun, 04 Jun 2023 18:54:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sun, 04 Jun 2023 18:54:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:54:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sun, 04 Jun 2023 18:54:53 GMT
VOLUME [/var/lib/mysql]
# Sun, 04 Jun 2023 18:54:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sun, 04 Jun 2023 18:54:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sun, 04 Jun 2023 18:54:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 04 Jun 2023 18:54:53 GMT
EXPOSE 3306 33060
# Sun, 04 Jun 2023 18:54:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3e0c3751e6482e67b70ffad144b2cb9aec9be672df2642a322e875e51b748aeb`  
		Last Modified: Sun, 04 Jun 2023 17:55:32 GMT  
		Size: 44.9 MB (44872720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7914193c6f0e6bf32545a75c783e4f919ef1fd267a806876c5d2f72da6c4be54`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4b3f820487ae4bd2869d410c4e4dc497042a73306e0ba99071b261e33190c1`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 982.8 KB (982825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63683b304e3d24e14589c48906cad17ead6bdf22ecf67b6291c12f5bc1544ec3`  
		Last Modified: Sun, 04 Jun 2023 18:55:21 GMT  
		Size: 4.6 MB (4614163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad9069836bd68adbe6be6e2c3aab749575e961266cd5ca27831330c21bb80d7`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90cd4c0e5df7a54d89ca2140cf329f530b89fe8c79de8873c66cfada8f5de6`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892e565e2cf01a43d9d6d4b4053893b1b1ea7c36b5b77965eabe762292eb491b`  
		Last Modified: Sun, 04 Jun 2023 18:55:26 GMT  
		Size: 58.6 MB (58610758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73057d123da0d3d34811ea0383a736c549907f639c24ab1bf576813c3ad40ba8`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1a3c0ec34ee20aec3f319f1f72ab7e94a9171b755be01adc71c30b19406ecb`  
		Last Modified: Sun, 04 Jun 2023 18:55:28 GMT  
		Size: 56.6 MB (56569548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fe8dc4ffe938cf78e257d45b0831df9a5053470ebed1d6978a85d061cb6dad`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807488ae889657196a0f63400133a21d65d2ed24ecb1a05faed222acdbeac0d`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a1e67f2bd2f3e36f387146ce6e6de3eb6d318aaec480a64d5a3a1506abf85275
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170106612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3077e10c878f57a4beaa0255cb581855b32118f5c2a8eef0b2c21373644541f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Jun 2023 22:40:44 GMT
ADD file:ae7c6036695430900f5ff735197e9c0281881b97faaea00e40263ca539fe7fff in / 
# Fri, 02 Jun 2023 22:40:45 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 22:58:57 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 02 Jun 2023 22:58:57 GMT
ENV GOSU_VERSION=1.16
# Fri, 02 Jun 2023 22:59:01 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Jun 2023 22:59:24 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 02 Jun 2023 22:59:54 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 02 Jun 2023 22:59:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 02 Jun 2023 22:59:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 23:00:28 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 02 Jun 2023 23:00:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Jun 2023 23:00:29 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 02 Jun 2023 23:00:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 02 Jun 2023 23:00:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 23:00:30 GMT
EXPOSE 3306 33060
# Fri, 02 Jun 2023 23:00:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ae143351a4fc570e80462825e827f3afbbabc4488aeae617542d42b521e5248`  
		Last Modified: Fri, 02 Jun 2023 22:41:37 GMT  
		Size: 43.8 MB (43787831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093b9ff06d4876e70f2620f141826cb4539ec8d199cca617013af6beea55bdc3`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf4f7b0363a59d4c3b6b8d9512406253633fbde87965376d96c2442a4d5d1ed`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8614746438f21c27808fe28de1009dc4791c5851e4ca822fc157f54970923c5`  
		Last Modified: Fri, 02 Jun 2023 23:00:44 GMT  
		Size: 4.5 MB (4456832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5aab2c5597c573d9d6efaf363a1e8e5672c55662832d2b559b4e263a763d1`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3e9a25efeb16879304ef4e09266c7562be10d36aebceda5acc9306165a433c`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1388739c015dac6d48f069dd3244dbe9016951625da6a8b94e5fb61b1fba9ff`  
		Last Modified: Fri, 02 Jun 2023 23:00:48 GMT  
		Size: 57.9 MB (57878613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a7da0e25e17bcf1d323a8477e936e2a1b2b569d07401d2dd4738828be7905b`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b0d0608a32def0b1d2c00a2ae8125fa493b15ccaa671ba53adf2364ca189c4`  
		Last Modified: Fri, 02 Jun 2023 23:00:49 GMT  
		Size: 63.1 MB (63060665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4191a53ea864946096ec2cba1542292cb1bf95072cae75675b26fae50a2bf64`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36880be7ebcb33b29760e2c596f17ac2f79e8bbc6b0f07a8b3ace99ed4a67d`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:4bae98614cd6ad1aecbdd32ff1b37b93fb0ee22b069469e7bc9679bacef1abd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:1717a37c2adc7772b569eb727bb198b6792f7d50c2adb4839ba637b5c9d88f42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165659693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71276df4a871c5c09ff8411247609cc9683d85290f9dc9b1871dd6e366a28f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sun, 04 Jun 2023 17:54:32 GMT
ADD file:39d09c6c7c3a0f64981f5cbcb12cc8f0128979c3d4b91d74c84fe62aca5ea87e in / 
# Sun, 04 Jun 2023 17:54:32 GMT
CMD ["/bin/bash"]
# Sun, 04 Jun 2023 18:53:08 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sun, 04 Jun 2023 18:53:08 GMT
ENV GOSU_VERSION=1.16
# Sun, 04 Jun 2023 18:53:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 04 Jun 2023 18:53:38 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_MAJOR=8.0
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sun, 04 Jun 2023 18:54:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sun, 04 Jun 2023 18:54:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sun, 04 Jun 2023 18:54:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:54:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sun, 04 Jun 2023 18:54:53 GMT
VOLUME [/var/lib/mysql]
# Sun, 04 Jun 2023 18:54:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sun, 04 Jun 2023 18:54:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sun, 04 Jun 2023 18:54:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 04 Jun 2023 18:54:53 GMT
EXPOSE 3306 33060
# Sun, 04 Jun 2023 18:54:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3e0c3751e6482e67b70ffad144b2cb9aec9be672df2642a322e875e51b748aeb`  
		Last Modified: Sun, 04 Jun 2023 17:55:32 GMT  
		Size: 44.9 MB (44872720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7914193c6f0e6bf32545a75c783e4f919ef1fd267a806876c5d2f72da6c4be54`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4b3f820487ae4bd2869d410c4e4dc497042a73306e0ba99071b261e33190c1`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 982.8 KB (982825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63683b304e3d24e14589c48906cad17ead6bdf22ecf67b6291c12f5bc1544ec3`  
		Last Modified: Sun, 04 Jun 2023 18:55:21 GMT  
		Size: 4.6 MB (4614163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad9069836bd68adbe6be6e2c3aab749575e961266cd5ca27831330c21bb80d7`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90cd4c0e5df7a54d89ca2140cf329f530b89fe8c79de8873c66cfada8f5de6`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892e565e2cf01a43d9d6d4b4053893b1b1ea7c36b5b77965eabe762292eb491b`  
		Last Modified: Sun, 04 Jun 2023 18:55:26 GMT  
		Size: 58.6 MB (58610758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73057d123da0d3d34811ea0383a736c549907f639c24ab1bf576813c3ad40ba8`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1a3c0ec34ee20aec3f319f1f72ab7e94a9171b755be01adc71c30b19406ecb`  
		Last Modified: Sun, 04 Jun 2023 18:55:28 GMT  
		Size: 56.6 MB (56569548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fe8dc4ffe938cf78e257d45b0831df9a5053470ebed1d6978a85d061cb6dad`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807488ae889657196a0f63400133a21d65d2ed24ecb1a05faed222acdbeac0d`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a1e67f2bd2f3e36f387146ce6e6de3eb6d318aaec480a64d5a3a1506abf85275
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170106612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3077e10c878f57a4beaa0255cb581855b32118f5c2a8eef0b2c21373644541f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Jun 2023 22:40:44 GMT
ADD file:ae7c6036695430900f5ff735197e9c0281881b97faaea00e40263ca539fe7fff in / 
# Fri, 02 Jun 2023 22:40:45 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 22:58:57 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 02 Jun 2023 22:58:57 GMT
ENV GOSU_VERSION=1.16
# Fri, 02 Jun 2023 22:59:01 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Jun 2023 22:59:24 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 02 Jun 2023 22:59:54 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 02 Jun 2023 22:59:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 02 Jun 2023 22:59:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 23:00:28 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 02 Jun 2023 23:00:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Jun 2023 23:00:29 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 02 Jun 2023 23:00:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 02 Jun 2023 23:00:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 23:00:30 GMT
EXPOSE 3306 33060
# Fri, 02 Jun 2023 23:00:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ae143351a4fc570e80462825e827f3afbbabc4488aeae617542d42b521e5248`  
		Last Modified: Fri, 02 Jun 2023 22:41:37 GMT  
		Size: 43.8 MB (43787831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093b9ff06d4876e70f2620f141826cb4539ec8d199cca617013af6beea55bdc3`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf4f7b0363a59d4c3b6b8d9512406253633fbde87965376d96c2442a4d5d1ed`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8614746438f21c27808fe28de1009dc4791c5851e4ca822fc157f54970923c5`  
		Last Modified: Fri, 02 Jun 2023 23:00:44 GMT  
		Size: 4.5 MB (4456832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5aab2c5597c573d9d6efaf363a1e8e5672c55662832d2b559b4e263a763d1`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3e9a25efeb16879304ef4e09266c7562be10d36aebceda5acc9306165a433c`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1388739c015dac6d48f069dd3244dbe9016951625da6a8b94e5fb61b1fba9ff`  
		Last Modified: Fri, 02 Jun 2023 23:00:48 GMT  
		Size: 57.9 MB (57878613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a7da0e25e17bcf1d323a8477e936e2a1b2b569d07401d2dd4738828be7905b`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b0d0608a32def0b1d2c00a2ae8125fa493b15ccaa671ba53adf2364ca189c4`  
		Last Modified: Fri, 02 Jun 2023 23:00:49 GMT  
		Size: 63.1 MB (63060665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4191a53ea864946096ec2cba1542292cb1bf95072cae75675b26fae50a2bf64`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36880be7ebcb33b29760e2c596f17ac2f79e8bbc6b0f07a8b3ace99ed4a67d`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:ee1e7bf1a6c7f7fc26abbbed04b6e0ab6f202b48c50ef8f418324901420b207e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:8dd2269034dd8680a2d90403977c9604bbaeb0e30364d105340a50241245785c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179716143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7faa2f9a3fde46c5e8c2d1b5c8d0fb9372a5707162e3b2826fe59478a54cce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:06:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jun 2023 07:06:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:06:17 GMT
ENV GOSU_VERSION=1.16
# Tue, 13 Jun 2023 07:06:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jun 2023 07:06:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jun 2023 07:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:06:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 13 Jun 2023 07:06:32 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 13 Jun 2023 07:06:32 GMT
ENV MYSQL_VERSION=8.0.33-1debian11
# Tue, 13 Jun 2023 07:06:33 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Jun 2023 07:06:47 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 13 Jun 2023 07:06:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jun 2023 07:06:48 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 13 Jun 2023 07:06:48 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 13 Jun 2023 07:06:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 07:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:06:49 GMT
EXPOSE 3306 33060
# Tue, 13 Jun 2023 07:06:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe03a6bd2ae95b6630c019ae5bf8e7351c8f27095d7fa0fb9a0deb3a6a56d515`  
		Last Modified: Tue, 13 Jun 2023 07:07:58 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe98fd0054daa6f38d2c1aaeff6b257d29ba86de74067a273764fb9801b4df9`  
		Last Modified: Tue, 13 Jun 2023 07:07:59 GMT  
		Size: 4.4 MB (4414989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b46f788fa0e3949eb16f96da627627fef28391e6788017828fdc59d85e1e47`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 1.5 MB (1471490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a574d9be7097a3158569d7be3fe8f58245d2a1160a02322df42cc21ed4da6305`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32a1a43aaf90ecca1eaecc5cbdade060ae64eb3ad5c0164d3f7fdfa6df36c22`  
		Last Modified: Tue, 13 Jun 2023 07:07:59 GMT  
		Size: 12.7 MB (12662026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1168cde172f4894d8388f45337512f3c50e31b0052297b85690542a846df34f6`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db9de6fbb6e12066dfb465bb744c8874637465cb32df5af3b7bdc1853d1f07e`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7597d1f876243f8e8f404c3f283ef6cbbdba1f7a9e6dd0382d87b0c52a1c7286`  
		Last Modified: Tue, 13 Jun 2023 07:08:13 GMT  
		Size: 129.7 MB (129739199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90525318623af863af49636e05796881027a61b6c6f6f673755105a58f6e1ff`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569dbc33ff4adc1218e4182f4ef79c728b2ece52f04ab884388496922b9c38f5`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765dd48ed85e84d520ae837a9e4fa93353bff6066721a0b41e484f1baeaa4194`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:4bae98614cd6ad1aecbdd32ff1b37b93fb0ee22b069469e7bc9679bacef1abd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1717a37c2adc7772b569eb727bb198b6792f7d50c2adb4839ba637b5c9d88f42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165659693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71276df4a871c5c09ff8411247609cc9683d85290f9dc9b1871dd6e366a28f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sun, 04 Jun 2023 17:54:32 GMT
ADD file:39d09c6c7c3a0f64981f5cbcb12cc8f0128979c3d4b91d74c84fe62aca5ea87e in / 
# Sun, 04 Jun 2023 17:54:32 GMT
CMD ["/bin/bash"]
# Sun, 04 Jun 2023 18:53:08 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sun, 04 Jun 2023 18:53:08 GMT
ENV GOSU_VERSION=1.16
# Sun, 04 Jun 2023 18:53:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 04 Jun 2023 18:53:38 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_MAJOR=8.0
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sun, 04 Jun 2023 18:54:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sun, 04 Jun 2023 18:54:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sun, 04 Jun 2023 18:54:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:54:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sun, 04 Jun 2023 18:54:53 GMT
VOLUME [/var/lib/mysql]
# Sun, 04 Jun 2023 18:54:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sun, 04 Jun 2023 18:54:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sun, 04 Jun 2023 18:54:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 04 Jun 2023 18:54:53 GMT
EXPOSE 3306 33060
# Sun, 04 Jun 2023 18:54:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3e0c3751e6482e67b70ffad144b2cb9aec9be672df2642a322e875e51b748aeb`  
		Last Modified: Sun, 04 Jun 2023 17:55:32 GMT  
		Size: 44.9 MB (44872720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7914193c6f0e6bf32545a75c783e4f919ef1fd267a806876c5d2f72da6c4be54`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4b3f820487ae4bd2869d410c4e4dc497042a73306e0ba99071b261e33190c1`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 982.8 KB (982825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63683b304e3d24e14589c48906cad17ead6bdf22ecf67b6291c12f5bc1544ec3`  
		Last Modified: Sun, 04 Jun 2023 18:55:21 GMT  
		Size: 4.6 MB (4614163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad9069836bd68adbe6be6e2c3aab749575e961266cd5ca27831330c21bb80d7`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90cd4c0e5df7a54d89ca2140cf329f530b89fe8c79de8873c66cfada8f5de6`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892e565e2cf01a43d9d6d4b4053893b1b1ea7c36b5b77965eabe762292eb491b`  
		Last Modified: Sun, 04 Jun 2023 18:55:26 GMT  
		Size: 58.6 MB (58610758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73057d123da0d3d34811ea0383a736c549907f639c24ab1bf576813c3ad40ba8`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1a3c0ec34ee20aec3f319f1f72ab7e94a9171b755be01adc71c30b19406ecb`  
		Last Modified: Sun, 04 Jun 2023 18:55:28 GMT  
		Size: 56.6 MB (56569548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fe8dc4ffe938cf78e257d45b0831df9a5053470ebed1d6978a85d061cb6dad`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807488ae889657196a0f63400133a21d65d2ed24ecb1a05faed222acdbeac0d`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a1e67f2bd2f3e36f387146ce6e6de3eb6d318aaec480a64d5a3a1506abf85275
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170106612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3077e10c878f57a4beaa0255cb581855b32118f5c2a8eef0b2c21373644541f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Jun 2023 22:40:44 GMT
ADD file:ae7c6036695430900f5ff735197e9c0281881b97faaea00e40263ca539fe7fff in / 
# Fri, 02 Jun 2023 22:40:45 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 22:58:57 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 02 Jun 2023 22:58:57 GMT
ENV GOSU_VERSION=1.16
# Fri, 02 Jun 2023 22:59:01 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Jun 2023 22:59:24 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 02 Jun 2023 22:59:54 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 02 Jun 2023 22:59:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 02 Jun 2023 22:59:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 23:00:28 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 02 Jun 2023 23:00:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Jun 2023 23:00:29 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 02 Jun 2023 23:00:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 02 Jun 2023 23:00:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 23:00:30 GMT
EXPOSE 3306 33060
# Fri, 02 Jun 2023 23:00:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ae143351a4fc570e80462825e827f3afbbabc4488aeae617542d42b521e5248`  
		Last Modified: Fri, 02 Jun 2023 22:41:37 GMT  
		Size: 43.8 MB (43787831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093b9ff06d4876e70f2620f141826cb4539ec8d199cca617013af6beea55bdc3`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf4f7b0363a59d4c3b6b8d9512406253633fbde87965376d96c2442a4d5d1ed`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8614746438f21c27808fe28de1009dc4791c5851e4ca822fc157f54970923c5`  
		Last Modified: Fri, 02 Jun 2023 23:00:44 GMT  
		Size: 4.5 MB (4456832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5aab2c5597c573d9d6efaf363a1e8e5672c55662832d2b559b4e263a763d1`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3e9a25efeb16879304ef4e09266c7562be10d36aebceda5acc9306165a433c`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1388739c015dac6d48f069dd3244dbe9016951625da6a8b94e5fb61b1fba9ff`  
		Last Modified: Fri, 02 Jun 2023 23:00:48 GMT  
		Size: 57.9 MB (57878613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a7da0e25e17bcf1d323a8477e936e2a1b2b569d07401d2dd4738828be7905b`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b0d0608a32def0b1d2c00a2ae8125fa493b15ccaa671ba53adf2364ca189c4`  
		Last Modified: Fri, 02 Jun 2023 23:00:49 GMT  
		Size: 63.1 MB (63060665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4191a53ea864946096ec2cba1542292cb1bf95072cae75675b26fae50a2bf64`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36880be7ebcb33b29760e2c596f17ac2f79e8bbc6b0f07a8b3ace99ed4a67d`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.33`

```console
$ docker pull mysql@sha256:4bae98614cd6ad1aecbdd32ff1b37b93fb0ee22b069469e7bc9679bacef1abd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.33` - linux; amd64

```console
$ docker pull mysql@sha256:1717a37c2adc7772b569eb727bb198b6792f7d50c2adb4839ba637b5c9d88f42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165659693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71276df4a871c5c09ff8411247609cc9683d85290f9dc9b1871dd6e366a28f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sun, 04 Jun 2023 17:54:32 GMT
ADD file:39d09c6c7c3a0f64981f5cbcb12cc8f0128979c3d4b91d74c84fe62aca5ea87e in / 
# Sun, 04 Jun 2023 17:54:32 GMT
CMD ["/bin/bash"]
# Sun, 04 Jun 2023 18:53:08 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sun, 04 Jun 2023 18:53:08 GMT
ENV GOSU_VERSION=1.16
# Sun, 04 Jun 2023 18:53:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 04 Jun 2023 18:53:38 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_MAJOR=8.0
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sun, 04 Jun 2023 18:54:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sun, 04 Jun 2023 18:54:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sun, 04 Jun 2023 18:54:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:54:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sun, 04 Jun 2023 18:54:53 GMT
VOLUME [/var/lib/mysql]
# Sun, 04 Jun 2023 18:54:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sun, 04 Jun 2023 18:54:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sun, 04 Jun 2023 18:54:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 04 Jun 2023 18:54:53 GMT
EXPOSE 3306 33060
# Sun, 04 Jun 2023 18:54:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3e0c3751e6482e67b70ffad144b2cb9aec9be672df2642a322e875e51b748aeb`  
		Last Modified: Sun, 04 Jun 2023 17:55:32 GMT  
		Size: 44.9 MB (44872720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7914193c6f0e6bf32545a75c783e4f919ef1fd267a806876c5d2f72da6c4be54`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4b3f820487ae4bd2869d410c4e4dc497042a73306e0ba99071b261e33190c1`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 982.8 KB (982825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63683b304e3d24e14589c48906cad17ead6bdf22ecf67b6291c12f5bc1544ec3`  
		Last Modified: Sun, 04 Jun 2023 18:55:21 GMT  
		Size: 4.6 MB (4614163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad9069836bd68adbe6be6e2c3aab749575e961266cd5ca27831330c21bb80d7`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90cd4c0e5df7a54d89ca2140cf329f530b89fe8c79de8873c66cfada8f5de6`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892e565e2cf01a43d9d6d4b4053893b1b1ea7c36b5b77965eabe762292eb491b`  
		Last Modified: Sun, 04 Jun 2023 18:55:26 GMT  
		Size: 58.6 MB (58610758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73057d123da0d3d34811ea0383a736c549907f639c24ab1bf576813c3ad40ba8`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1a3c0ec34ee20aec3f319f1f72ab7e94a9171b755be01adc71c30b19406ecb`  
		Last Modified: Sun, 04 Jun 2023 18:55:28 GMT  
		Size: 56.6 MB (56569548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fe8dc4ffe938cf78e257d45b0831df9a5053470ebed1d6978a85d061cb6dad`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807488ae889657196a0f63400133a21d65d2ed24ecb1a05faed222acdbeac0d`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.33` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a1e67f2bd2f3e36f387146ce6e6de3eb6d318aaec480a64d5a3a1506abf85275
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170106612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3077e10c878f57a4beaa0255cb581855b32118f5c2a8eef0b2c21373644541f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Jun 2023 22:40:44 GMT
ADD file:ae7c6036695430900f5ff735197e9c0281881b97faaea00e40263ca539fe7fff in / 
# Fri, 02 Jun 2023 22:40:45 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 22:58:57 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 02 Jun 2023 22:58:57 GMT
ENV GOSU_VERSION=1.16
# Fri, 02 Jun 2023 22:59:01 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Jun 2023 22:59:24 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 02 Jun 2023 22:59:54 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 02 Jun 2023 22:59:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 02 Jun 2023 22:59:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 23:00:28 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 02 Jun 2023 23:00:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Jun 2023 23:00:29 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 02 Jun 2023 23:00:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 02 Jun 2023 23:00:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 23:00:30 GMT
EXPOSE 3306 33060
# Fri, 02 Jun 2023 23:00:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ae143351a4fc570e80462825e827f3afbbabc4488aeae617542d42b521e5248`  
		Last Modified: Fri, 02 Jun 2023 22:41:37 GMT  
		Size: 43.8 MB (43787831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093b9ff06d4876e70f2620f141826cb4539ec8d199cca617013af6beea55bdc3`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf4f7b0363a59d4c3b6b8d9512406253633fbde87965376d96c2442a4d5d1ed`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8614746438f21c27808fe28de1009dc4791c5851e4ca822fc157f54970923c5`  
		Last Modified: Fri, 02 Jun 2023 23:00:44 GMT  
		Size: 4.5 MB (4456832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5aab2c5597c573d9d6efaf363a1e8e5672c55662832d2b559b4e263a763d1`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3e9a25efeb16879304ef4e09266c7562be10d36aebceda5acc9306165a433c`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1388739c015dac6d48f069dd3244dbe9016951625da6a8b94e5fb61b1fba9ff`  
		Last Modified: Fri, 02 Jun 2023 23:00:48 GMT  
		Size: 57.9 MB (57878613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a7da0e25e17bcf1d323a8477e936e2a1b2b569d07401d2dd4738828be7905b`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b0d0608a32def0b1d2c00a2ae8125fa493b15ccaa671ba53adf2364ca189c4`  
		Last Modified: Fri, 02 Jun 2023 23:00:49 GMT  
		Size: 63.1 MB (63060665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4191a53ea864946096ec2cba1542292cb1bf95072cae75675b26fae50a2bf64`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36880be7ebcb33b29760e2c596f17ac2f79e8bbc6b0f07a8b3ace99ed4a67d`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.33-debian`

```console
$ docker pull mysql@sha256:ee1e7bf1a6c7f7fc26abbbed04b6e0ab6f202b48c50ef8f418324901420b207e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.33-debian` - linux; amd64

```console
$ docker pull mysql@sha256:8dd2269034dd8680a2d90403977c9604bbaeb0e30364d105340a50241245785c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179716143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7faa2f9a3fde46c5e8c2d1b5c8d0fb9372a5707162e3b2826fe59478a54cce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:06:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jun 2023 07:06:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:06:17 GMT
ENV GOSU_VERSION=1.16
# Tue, 13 Jun 2023 07:06:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jun 2023 07:06:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jun 2023 07:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:06:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 13 Jun 2023 07:06:32 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 13 Jun 2023 07:06:32 GMT
ENV MYSQL_VERSION=8.0.33-1debian11
# Tue, 13 Jun 2023 07:06:33 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Jun 2023 07:06:47 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 13 Jun 2023 07:06:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jun 2023 07:06:48 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 13 Jun 2023 07:06:48 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 13 Jun 2023 07:06:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 07:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:06:49 GMT
EXPOSE 3306 33060
# Tue, 13 Jun 2023 07:06:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe03a6bd2ae95b6630c019ae5bf8e7351c8f27095d7fa0fb9a0deb3a6a56d515`  
		Last Modified: Tue, 13 Jun 2023 07:07:58 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe98fd0054daa6f38d2c1aaeff6b257d29ba86de74067a273764fb9801b4df9`  
		Last Modified: Tue, 13 Jun 2023 07:07:59 GMT  
		Size: 4.4 MB (4414989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b46f788fa0e3949eb16f96da627627fef28391e6788017828fdc59d85e1e47`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 1.5 MB (1471490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a574d9be7097a3158569d7be3fe8f58245d2a1160a02322df42cc21ed4da6305`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32a1a43aaf90ecca1eaecc5cbdade060ae64eb3ad5c0164d3f7fdfa6df36c22`  
		Last Modified: Tue, 13 Jun 2023 07:07:59 GMT  
		Size: 12.7 MB (12662026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1168cde172f4894d8388f45337512f3c50e31b0052297b85690542a846df34f6`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db9de6fbb6e12066dfb465bb744c8874637465cb32df5af3b7bdc1853d1f07e`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7597d1f876243f8e8f404c3f283ef6cbbdba1f7a9e6dd0382d87b0c52a1c7286`  
		Last Modified: Tue, 13 Jun 2023 07:08:13 GMT  
		Size: 129.7 MB (129739199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90525318623af863af49636e05796881027a61b6c6f6f673755105a58f6e1ff`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569dbc33ff4adc1218e4182f4ef79c728b2ece52f04ab884388496922b9c38f5`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765dd48ed85e84d520ae837a9e4fa93353bff6066721a0b41e484f1baeaa4194`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.33-oracle`

```console
$ docker pull mysql@sha256:4bae98614cd6ad1aecbdd32ff1b37b93fb0ee22b069469e7bc9679bacef1abd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.33-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1717a37c2adc7772b569eb727bb198b6792f7d50c2adb4839ba637b5c9d88f42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165659693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71276df4a871c5c09ff8411247609cc9683d85290f9dc9b1871dd6e366a28f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sun, 04 Jun 2023 17:54:32 GMT
ADD file:39d09c6c7c3a0f64981f5cbcb12cc8f0128979c3d4b91d74c84fe62aca5ea87e in / 
# Sun, 04 Jun 2023 17:54:32 GMT
CMD ["/bin/bash"]
# Sun, 04 Jun 2023 18:53:08 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sun, 04 Jun 2023 18:53:08 GMT
ENV GOSU_VERSION=1.16
# Sun, 04 Jun 2023 18:53:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 04 Jun 2023 18:53:38 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_MAJOR=8.0
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sun, 04 Jun 2023 18:54:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sun, 04 Jun 2023 18:54:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sun, 04 Jun 2023 18:54:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:54:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sun, 04 Jun 2023 18:54:53 GMT
VOLUME [/var/lib/mysql]
# Sun, 04 Jun 2023 18:54:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sun, 04 Jun 2023 18:54:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sun, 04 Jun 2023 18:54:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 04 Jun 2023 18:54:53 GMT
EXPOSE 3306 33060
# Sun, 04 Jun 2023 18:54:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3e0c3751e6482e67b70ffad144b2cb9aec9be672df2642a322e875e51b748aeb`  
		Last Modified: Sun, 04 Jun 2023 17:55:32 GMT  
		Size: 44.9 MB (44872720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7914193c6f0e6bf32545a75c783e4f919ef1fd267a806876c5d2f72da6c4be54`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4b3f820487ae4bd2869d410c4e4dc497042a73306e0ba99071b261e33190c1`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 982.8 KB (982825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63683b304e3d24e14589c48906cad17ead6bdf22ecf67b6291c12f5bc1544ec3`  
		Last Modified: Sun, 04 Jun 2023 18:55:21 GMT  
		Size: 4.6 MB (4614163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad9069836bd68adbe6be6e2c3aab749575e961266cd5ca27831330c21bb80d7`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90cd4c0e5df7a54d89ca2140cf329f530b89fe8c79de8873c66cfada8f5de6`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892e565e2cf01a43d9d6d4b4053893b1b1ea7c36b5b77965eabe762292eb491b`  
		Last Modified: Sun, 04 Jun 2023 18:55:26 GMT  
		Size: 58.6 MB (58610758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73057d123da0d3d34811ea0383a736c549907f639c24ab1bf576813c3ad40ba8`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1a3c0ec34ee20aec3f319f1f72ab7e94a9171b755be01adc71c30b19406ecb`  
		Last Modified: Sun, 04 Jun 2023 18:55:28 GMT  
		Size: 56.6 MB (56569548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fe8dc4ffe938cf78e257d45b0831df9a5053470ebed1d6978a85d061cb6dad`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807488ae889657196a0f63400133a21d65d2ed24ecb1a05faed222acdbeac0d`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.33-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a1e67f2bd2f3e36f387146ce6e6de3eb6d318aaec480a64d5a3a1506abf85275
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170106612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3077e10c878f57a4beaa0255cb581855b32118f5c2a8eef0b2c21373644541f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Jun 2023 22:40:44 GMT
ADD file:ae7c6036695430900f5ff735197e9c0281881b97faaea00e40263ca539fe7fff in / 
# Fri, 02 Jun 2023 22:40:45 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 22:58:57 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 02 Jun 2023 22:58:57 GMT
ENV GOSU_VERSION=1.16
# Fri, 02 Jun 2023 22:59:01 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Jun 2023 22:59:24 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 02 Jun 2023 22:59:54 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 02 Jun 2023 22:59:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 02 Jun 2023 22:59:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 23:00:28 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 02 Jun 2023 23:00:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Jun 2023 23:00:29 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 02 Jun 2023 23:00:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 02 Jun 2023 23:00:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 23:00:30 GMT
EXPOSE 3306 33060
# Fri, 02 Jun 2023 23:00:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ae143351a4fc570e80462825e827f3afbbabc4488aeae617542d42b521e5248`  
		Last Modified: Fri, 02 Jun 2023 22:41:37 GMT  
		Size: 43.8 MB (43787831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093b9ff06d4876e70f2620f141826cb4539ec8d199cca617013af6beea55bdc3`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf4f7b0363a59d4c3b6b8d9512406253633fbde87965376d96c2442a4d5d1ed`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8614746438f21c27808fe28de1009dc4791c5851e4ca822fc157f54970923c5`  
		Last Modified: Fri, 02 Jun 2023 23:00:44 GMT  
		Size: 4.5 MB (4456832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5aab2c5597c573d9d6efaf363a1e8e5672c55662832d2b559b4e263a763d1`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3e9a25efeb16879304ef4e09266c7562be10d36aebceda5acc9306165a433c`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1388739c015dac6d48f069dd3244dbe9016951625da6a8b94e5fb61b1fba9ff`  
		Last Modified: Fri, 02 Jun 2023 23:00:48 GMT  
		Size: 57.9 MB (57878613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a7da0e25e17bcf1d323a8477e936e2a1b2b569d07401d2dd4738828be7905b`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b0d0608a32def0b1d2c00a2ae8125fa493b15ccaa671ba53adf2364ca189c4`  
		Last Modified: Fri, 02 Jun 2023 23:00:49 GMT  
		Size: 63.1 MB (63060665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4191a53ea864946096ec2cba1542292cb1bf95072cae75675b26fae50a2bf64`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36880be7ebcb33b29760e2c596f17ac2f79e8bbc6b0f07a8b3ace99ed4a67d`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:ee1e7bf1a6c7f7fc26abbbed04b6e0ab6f202b48c50ef8f418324901420b207e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:8dd2269034dd8680a2d90403977c9604bbaeb0e30364d105340a50241245785c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179716143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7faa2f9a3fde46c5e8c2d1b5c8d0fb9372a5707162e3b2826fe59478a54cce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:06:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jun 2023 07:06:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:06:17 GMT
ENV GOSU_VERSION=1.16
# Tue, 13 Jun 2023 07:06:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jun 2023 07:06:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jun 2023 07:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:06:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 13 Jun 2023 07:06:32 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 13 Jun 2023 07:06:32 GMT
ENV MYSQL_VERSION=8.0.33-1debian11
# Tue, 13 Jun 2023 07:06:33 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Jun 2023 07:06:47 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 13 Jun 2023 07:06:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jun 2023 07:06:48 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 13 Jun 2023 07:06:48 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 13 Jun 2023 07:06:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 07:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:06:49 GMT
EXPOSE 3306 33060
# Tue, 13 Jun 2023 07:06:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe03a6bd2ae95b6630c019ae5bf8e7351c8f27095d7fa0fb9a0deb3a6a56d515`  
		Last Modified: Tue, 13 Jun 2023 07:07:58 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe98fd0054daa6f38d2c1aaeff6b257d29ba86de74067a273764fb9801b4df9`  
		Last Modified: Tue, 13 Jun 2023 07:07:59 GMT  
		Size: 4.4 MB (4414989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b46f788fa0e3949eb16f96da627627fef28391e6788017828fdc59d85e1e47`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 1.5 MB (1471490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a574d9be7097a3158569d7be3fe8f58245d2a1160a02322df42cc21ed4da6305`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32a1a43aaf90ecca1eaecc5cbdade060ae64eb3ad5c0164d3f7fdfa6df36c22`  
		Last Modified: Tue, 13 Jun 2023 07:07:59 GMT  
		Size: 12.7 MB (12662026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1168cde172f4894d8388f45337512f3c50e31b0052297b85690542a846df34f6`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db9de6fbb6e12066dfb465bb744c8874637465cb32df5af3b7bdc1853d1f07e`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7597d1f876243f8e8f404c3f283ef6cbbdba1f7a9e6dd0382d87b0c52a1c7286`  
		Last Modified: Tue, 13 Jun 2023 07:08:13 GMT  
		Size: 129.7 MB (129739199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90525318623af863af49636e05796881027a61b6c6f6f673755105a58f6e1ff`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569dbc33ff4adc1218e4182f4ef79c728b2ece52f04ab884388496922b9c38f5`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765dd48ed85e84d520ae837a9e4fa93353bff6066721a0b41e484f1baeaa4194`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:4bae98614cd6ad1aecbdd32ff1b37b93fb0ee22b069469e7bc9679bacef1abd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:1717a37c2adc7772b569eb727bb198b6792f7d50c2adb4839ba637b5c9d88f42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165659693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71276df4a871c5c09ff8411247609cc9683d85290f9dc9b1871dd6e366a28f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sun, 04 Jun 2023 17:54:32 GMT
ADD file:39d09c6c7c3a0f64981f5cbcb12cc8f0128979c3d4b91d74c84fe62aca5ea87e in / 
# Sun, 04 Jun 2023 17:54:32 GMT
CMD ["/bin/bash"]
# Sun, 04 Jun 2023 18:53:08 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sun, 04 Jun 2023 18:53:08 GMT
ENV GOSU_VERSION=1.16
# Sun, 04 Jun 2023 18:53:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 04 Jun 2023 18:53:38 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_MAJOR=8.0
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sun, 04 Jun 2023 18:54:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sun, 04 Jun 2023 18:54:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sun, 04 Jun 2023 18:54:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:54:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sun, 04 Jun 2023 18:54:53 GMT
VOLUME [/var/lib/mysql]
# Sun, 04 Jun 2023 18:54:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sun, 04 Jun 2023 18:54:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sun, 04 Jun 2023 18:54:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 04 Jun 2023 18:54:53 GMT
EXPOSE 3306 33060
# Sun, 04 Jun 2023 18:54:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3e0c3751e6482e67b70ffad144b2cb9aec9be672df2642a322e875e51b748aeb`  
		Last Modified: Sun, 04 Jun 2023 17:55:32 GMT  
		Size: 44.9 MB (44872720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7914193c6f0e6bf32545a75c783e4f919ef1fd267a806876c5d2f72da6c4be54`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4b3f820487ae4bd2869d410c4e4dc497042a73306e0ba99071b261e33190c1`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 982.8 KB (982825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63683b304e3d24e14589c48906cad17ead6bdf22ecf67b6291c12f5bc1544ec3`  
		Last Modified: Sun, 04 Jun 2023 18:55:21 GMT  
		Size: 4.6 MB (4614163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad9069836bd68adbe6be6e2c3aab749575e961266cd5ca27831330c21bb80d7`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90cd4c0e5df7a54d89ca2140cf329f530b89fe8c79de8873c66cfada8f5de6`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892e565e2cf01a43d9d6d4b4053893b1b1ea7c36b5b77965eabe762292eb491b`  
		Last Modified: Sun, 04 Jun 2023 18:55:26 GMT  
		Size: 58.6 MB (58610758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73057d123da0d3d34811ea0383a736c549907f639c24ab1bf576813c3ad40ba8`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1a3c0ec34ee20aec3f319f1f72ab7e94a9171b755be01adc71c30b19406ecb`  
		Last Modified: Sun, 04 Jun 2023 18:55:28 GMT  
		Size: 56.6 MB (56569548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fe8dc4ffe938cf78e257d45b0831df9a5053470ebed1d6978a85d061cb6dad`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807488ae889657196a0f63400133a21d65d2ed24ecb1a05faed222acdbeac0d`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a1e67f2bd2f3e36f387146ce6e6de3eb6d318aaec480a64d5a3a1506abf85275
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170106612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3077e10c878f57a4beaa0255cb581855b32118f5c2a8eef0b2c21373644541f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Jun 2023 22:40:44 GMT
ADD file:ae7c6036695430900f5ff735197e9c0281881b97faaea00e40263ca539fe7fff in / 
# Fri, 02 Jun 2023 22:40:45 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 22:58:57 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 02 Jun 2023 22:58:57 GMT
ENV GOSU_VERSION=1.16
# Fri, 02 Jun 2023 22:59:01 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Jun 2023 22:59:24 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 02 Jun 2023 22:59:54 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 02 Jun 2023 22:59:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 02 Jun 2023 22:59:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 23:00:28 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 02 Jun 2023 23:00:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Jun 2023 23:00:29 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 02 Jun 2023 23:00:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 02 Jun 2023 23:00:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 23:00:30 GMT
EXPOSE 3306 33060
# Fri, 02 Jun 2023 23:00:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ae143351a4fc570e80462825e827f3afbbabc4488aeae617542d42b521e5248`  
		Last Modified: Fri, 02 Jun 2023 22:41:37 GMT  
		Size: 43.8 MB (43787831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093b9ff06d4876e70f2620f141826cb4539ec8d199cca617013af6beea55bdc3`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf4f7b0363a59d4c3b6b8d9512406253633fbde87965376d96c2442a4d5d1ed`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8614746438f21c27808fe28de1009dc4791c5851e4ca822fc157f54970923c5`  
		Last Modified: Fri, 02 Jun 2023 23:00:44 GMT  
		Size: 4.5 MB (4456832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5aab2c5597c573d9d6efaf363a1e8e5672c55662832d2b559b4e263a763d1`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3e9a25efeb16879304ef4e09266c7562be10d36aebceda5acc9306165a433c`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1388739c015dac6d48f069dd3244dbe9016951625da6a8b94e5fb61b1fba9ff`  
		Last Modified: Fri, 02 Jun 2023 23:00:48 GMT  
		Size: 57.9 MB (57878613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a7da0e25e17bcf1d323a8477e936e2a1b2b569d07401d2dd4738828be7905b`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b0d0608a32def0b1d2c00a2ae8125fa493b15ccaa671ba53adf2364ca189c4`  
		Last Modified: Fri, 02 Jun 2023 23:00:49 GMT  
		Size: 63.1 MB (63060665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4191a53ea864946096ec2cba1542292cb1bf95072cae75675b26fae50a2bf64`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36880be7ebcb33b29760e2c596f17ac2f79e8bbc6b0f07a8b3ace99ed4a67d`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:4bae98614cd6ad1aecbdd32ff1b37b93fb0ee22b069469e7bc9679bacef1abd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1717a37c2adc7772b569eb727bb198b6792f7d50c2adb4839ba637b5c9d88f42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165659693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71276df4a871c5c09ff8411247609cc9683d85290f9dc9b1871dd6e366a28f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sun, 04 Jun 2023 17:54:32 GMT
ADD file:39d09c6c7c3a0f64981f5cbcb12cc8f0128979c3d4b91d74c84fe62aca5ea87e in / 
# Sun, 04 Jun 2023 17:54:32 GMT
CMD ["/bin/bash"]
# Sun, 04 Jun 2023 18:53:08 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sun, 04 Jun 2023 18:53:08 GMT
ENV GOSU_VERSION=1.16
# Sun, 04 Jun 2023 18:53:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 04 Jun 2023 18:53:38 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_MAJOR=8.0
# Sun, 04 Jun 2023 18:53:40 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:53:40 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sun, 04 Jun 2023 18:54:13 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sun, 04 Jun 2023 18:54:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sun, 04 Jun 2023 18:54:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sun, 04 Jun 2023 18:54:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sun, 04 Jun 2023 18:54:53 GMT
VOLUME [/var/lib/mysql]
# Sun, 04 Jun 2023 18:54:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sun, 04 Jun 2023 18:54:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sun, 04 Jun 2023 18:54:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 04 Jun 2023 18:54:53 GMT
EXPOSE 3306 33060
# Sun, 04 Jun 2023 18:54:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3e0c3751e6482e67b70ffad144b2cb9aec9be672df2642a322e875e51b748aeb`  
		Last Modified: Sun, 04 Jun 2023 17:55:32 GMT  
		Size: 44.9 MB (44872720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7914193c6f0e6bf32545a75c783e4f919ef1fd267a806876c5d2f72da6c4be54`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4b3f820487ae4bd2869d410c4e4dc497042a73306e0ba99071b261e33190c1`  
		Last Modified: Sun, 04 Jun 2023 18:55:22 GMT  
		Size: 982.8 KB (982825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63683b304e3d24e14589c48906cad17ead6bdf22ecf67b6291c12f5bc1544ec3`  
		Last Modified: Sun, 04 Jun 2023 18:55:21 GMT  
		Size: 4.6 MB (4614163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad9069836bd68adbe6be6e2c3aab749575e961266cd5ca27831330c21bb80d7`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90cd4c0e5df7a54d89ca2140cf329f530b89fe8c79de8873c66cfada8f5de6`  
		Last Modified: Sun, 04 Jun 2023 18:55:20 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892e565e2cf01a43d9d6d4b4053893b1b1ea7c36b5b77965eabe762292eb491b`  
		Last Modified: Sun, 04 Jun 2023 18:55:26 GMT  
		Size: 58.6 MB (58610758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73057d123da0d3d34811ea0383a736c549907f639c24ab1bf576813c3ad40ba8`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1a3c0ec34ee20aec3f319f1f72ab7e94a9171b755be01adc71c30b19406ecb`  
		Last Modified: Sun, 04 Jun 2023 18:55:28 GMT  
		Size: 56.6 MB (56569548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fe8dc4ffe938cf78e257d45b0831df9a5053470ebed1d6978a85d061cb6dad`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807488ae889657196a0f63400133a21d65d2ed24ecb1a05faed222acdbeac0d`  
		Last Modified: Sun, 04 Jun 2023 18:55:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a1e67f2bd2f3e36f387146ce6e6de3eb6d318aaec480a64d5a3a1506abf85275
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170106612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3077e10c878f57a4beaa0255cb581855b32118f5c2a8eef0b2c21373644541f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Jun 2023 22:40:44 GMT
ADD file:ae7c6036695430900f5ff735197e9c0281881b97faaea00e40263ca539fe7fff in / 
# Fri, 02 Jun 2023 22:40:45 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 22:58:57 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 02 Jun 2023 22:58:57 GMT
ENV GOSU_VERSION=1.16
# Fri, 02 Jun 2023 22:59:01 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Jun 2023 22:59:24 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 02 Jun 2023 22:59:26 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 22:59:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 02 Jun 2023 22:59:54 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 02 Jun 2023 22:59:56 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 02 Jun 2023 22:59:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 02 Jun 2023 23:00:28 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 02 Jun 2023 23:00:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Jun 2023 23:00:29 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 02 Jun 2023 23:00:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 02 Jun 2023 23:00:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 23:00:30 GMT
EXPOSE 3306 33060
# Fri, 02 Jun 2023 23:00:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2ae143351a4fc570e80462825e827f3afbbabc4488aeae617542d42b521e5248`  
		Last Modified: Fri, 02 Jun 2023 22:41:37 GMT  
		Size: 43.8 MB (43787831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093b9ff06d4876e70f2620f141826cb4539ec8d199cca617013af6beea55bdc3`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf4f7b0363a59d4c3b6b8d9512406253633fbde87965376d96c2442a4d5d1ed`  
		Last Modified: Fri, 02 Jun 2023 23:00:45 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8614746438f21c27808fe28de1009dc4791c5851e4ca822fc157f54970923c5`  
		Last Modified: Fri, 02 Jun 2023 23:00:44 GMT  
		Size: 4.5 MB (4456832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5aab2c5597c573d9d6efaf363a1e8e5672c55662832d2b559b4e263a763d1`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3e9a25efeb16879304ef4e09266c7562be10d36aebceda5acc9306165a433c`  
		Last Modified: Fri, 02 Jun 2023 23:00:43 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1388739c015dac6d48f069dd3244dbe9016951625da6a8b94e5fb61b1fba9ff`  
		Last Modified: Fri, 02 Jun 2023 23:00:48 GMT  
		Size: 57.9 MB (57878613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a7da0e25e17bcf1d323a8477e936e2a1b2b569d07401d2dd4738828be7905b`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b0d0608a32def0b1d2c00a2ae8125fa493b15ccaa671ba53adf2364ca189c4`  
		Last Modified: Fri, 02 Jun 2023 23:00:49 GMT  
		Size: 63.1 MB (63060665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4191a53ea864946096ec2cba1542292cb1bf95072cae75675b26fae50a2bf64`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d36880be7ebcb33b29760e2c596f17ac2f79e8bbc6b0f07a8b3ace99ed4a67d`  
		Last Modified: Fri, 02 Jun 2023 23:00:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
