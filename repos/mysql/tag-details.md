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
$ docker pull mysql@sha256:bd873931ef20f30a5a9bf71498ce4e02c88cf48b2e8b782c337076d814deebde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:03b6dcedf5a2754da00e119e2cc6094ed3c884ad36b67bb25fe67be4b4f9bdb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169271448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be84dd575ee2ecdb186dc43a9cd951890a764d2cefbd31a72cdf4410c43a2d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:53:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 14 Jun 2023 09:53:50 GMT
ENV GOSU_VERSION=1.16
# Wed, 14 Jun 2023 09:53:53 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Jun 2023 09:54:11 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 14 Jun 2023 09:54:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Wed, 14 Jun 2023 09:54:13 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 14 Jun 2023 09:54:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el7
# Wed, 14 Jun 2023 09:55:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 14 Jun 2023 09:55:16 GMT
VOLUME [/var/lib/mysql]
# Wed, 14 Jun 2023 09:55:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 14 Jun 2023 09:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 09:55:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 09:55:17 GMT
EXPOSE 3306 33060
# Wed, 14 Jun 2023 09:55:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca4383b183f283dc0ac1a0351f5cb31f75dbd244bee8dc0988af4a50f2c59df`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 872.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e282e7651b1612ff17f6246e0847dad6996add940329721a4756a1879f15a23`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 983.7 KB (983711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa0e0ca7078cd2e1abcaa6847bc545576fd23586b4ae3ccc90b31637f27b1f`  
		Last Modified: Wed, 14 Jun 2023 09:55:48 GMT  
		Size: 4.6 MB (4601387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb790cf638212f7a95cd187ed8515ff749c06d616bab23ee7ff4f87969533c7`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7ffc37d8e9c1691a3e04e9fcdf2409484ca22e3b8a1b81e30c0b0ad85551df`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4393c12228b9628c8d3a8c421e92080b206ee9445951e9119fce64d61a7fd143`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 25.5 MB (25534088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389d2c130d520b0e7953b08faa0ad308866e0cb139cd341ddc16501aac8cc3a7`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5df3caef94cc41376f0f14fd6db2c5e224ad013a805aa8df2b5a7a90eed01e5`  
		Last Modified: Wed, 14 Jun 2023 09:55:58 GMT  
		Size: 87.7 MB (87657804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6aa409290d0f55131bc8d7d406e767576e88c510c69b28ac02aaf7167e07c4`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa350980ea9f8455483b598af47fcb9e6d96f5d4b2d50f4d3fdcee486c7f562`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:c0a0e68b9bc8d6cebdbdef8a6e769df5502a361f9190be694bd84e4035fecfb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:9f266e88e9418d3e290303eeff93b2b0b1091e48979dda1407168716e8e00aae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.8 MB (162760797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5d7c63fe3391e41709423d7663a381baea7ee5ca33a923a0a4768009cc45a44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:47 GMT
ADD file:ca4076bfffab8d09636384070ca253570590554cff76a132afaae5cd89b363b5 in / 
# Tue, 04 Jul 2023 01:20:48 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:40:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:40:49 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:40:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:40:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:41:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:41:05 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:41:05 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 04 Jul 2023 16:41:05 GMT
ENV MYSQL_VERSION=5.7.42-1debian10
# Tue, 04 Jul 2023 16:41:06 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Jul 2023 16:41:24 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 04 Jul 2023 16:41:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:41:24 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:41:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:41:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:41:25 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:41:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:90ac1ecaf92c8ae0cb37d29d8cc01b5802612c12edb933c369ad4c586ea94c6c`  
		Last Modified: Tue, 04 Jul 2023 01:26:21 GMT  
		Size: 27.1 MB (27138502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5332fa444fcbc9427056611d173b59e9fb27193696d2caff0ce93902012bf2c`  
		Last Modified: Tue, 04 Jul 2023 16:42:55 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df99bbd075464fe4c45ccfb06b4f3261dcb494b081d2bf090ed8bdb72c6f273`  
		Last Modified: Tue, 04 Jul 2023 16:42:54 GMT  
		Size: 4.2 MB (4182356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1074e6f5cec3a9ad3219a0bf1b7c4d342e68b9311b347a3c0bbdb9b519f104f6`  
		Last Modified: Tue, 04 Jul 2023 16:42:53 GMT  
		Size: 1.4 MB (1441848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bbcb49a75325f17e87e7366fd5499c77bd750fd0a563ecf4fa330598b567ad`  
		Last Modified: Tue, 04 Jul 2023 16:42:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b88e8cde452e8be99b1b7b0e95df9f144877dd3f6a5a751d8d84b5bf98172d`  
		Last Modified: Tue, 04 Jul 2023 16:42:56 GMT  
		Size: 14.1 MB (14089552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd01f08045baa85450d1a60acdb8043f3822f8f08fbc23a6427b43e0d31907b1`  
		Last Modified: Tue, 04 Jul 2023 16:42:51 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6ca6adc2aaa205cfce0083344463b5b459968a0894526ecac3305a1eac1830`  
		Last Modified: Tue, 04 Jul 2023 16:42:51 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57f7cb4781685a978155f98f294792b9c1eaa227c7a22edf025b79e3a5ba5c2`  
		Last Modified: Tue, 04 Jul 2023 16:43:05 GMT  
		Size: 115.9 MB (115898351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d80f44b4d6a403257ac7dfb82cf09de4952b0ce1723f75732a045ba5c92556`  
		Last Modified: Tue, 04 Jul 2023 16:42:51 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2a073f32ef118e7b46e8ff821eb2b0b0a56eb101918cda05b274f0ad3caf49`  
		Last Modified: Tue, 04 Jul 2023 16:42:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:bd873931ef20f30a5a9bf71498ce4e02c88cf48b2e8b782c337076d814deebde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:03b6dcedf5a2754da00e119e2cc6094ed3c884ad36b67bb25fe67be4b4f9bdb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169271448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be84dd575ee2ecdb186dc43a9cd951890a764d2cefbd31a72cdf4410c43a2d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:53:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 14 Jun 2023 09:53:50 GMT
ENV GOSU_VERSION=1.16
# Wed, 14 Jun 2023 09:53:53 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Jun 2023 09:54:11 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 14 Jun 2023 09:54:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Wed, 14 Jun 2023 09:54:13 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 14 Jun 2023 09:54:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el7
# Wed, 14 Jun 2023 09:55:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 14 Jun 2023 09:55:16 GMT
VOLUME [/var/lib/mysql]
# Wed, 14 Jun 2023 09:55:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 14 Jun 2023 09:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 09:55:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 09:55:17 GMT
EXPOSE 3306 33060
# Wed, 14 Jun 2023 09:55:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca4383b183f283dc0ac1a0351f5cb31f75dbd244bee8dc0988af4a50f2c59df`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 872.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e282e7651b1612ff17f6246e0847dad6996add940329721a4756a1879f15a23`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 983.7 KB (983711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa0e0ca7078cd2e1abcaa6847bc545576fd23586b4ae3ccc90b31637f27b1f`  
		Last Modified: Wed, 14 Jun 2023 09:55:48 GMT  
		Size: 4.6 MB (4601387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb790cf638212f7a95cd187ed8515ff749c06d616bab23ee7ff4f87969533c7`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7ffc37d8e9c1691a3e04e9fcdf2409484ca22e3b8a1b81e30c0b0ad85551df`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4393c12228b9628c8d3a8c421e92080b206ee9445951e9119fce64d61a7fd143`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 25.5 MB (25534088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389d2c130d520b0e7953b08faa0ad308866e0cb139cd341ddc16501aac8cc3a7`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5df3caef94cc41376f0f14fd6db2c5e224ad013a805aa8df2b5a7a90eed01e5`  
		Last Modified: Wed, 14 Jun 2023 09:55:58 GMT  
		Size: 87.7 MB (87657804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6aa409290d0f55131bc8d7d406e767576e88c510c69b28ac02aaf7167e07c4`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa350980ea9f8455483b598af47fcb9e6d96f5d4b2d50f4d3fdcee486c7f562`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:bd873931ef20f30a5a9bf71498ce4e02c88cf48b2e8b782c337076d814deebde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:03b6dcedf5a2754da00e119e2cc6094ed3c884ad36b67bb25fe67be4b4f9bdb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169271448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be84dd575ee2ecdb186dc43a9cd951890a764d2cefbd31a72cdf4410c43a2d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:53:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 14 Jun 2023 09:53:50 GMT
ENV GOSU_VERSION=1.16
# Wed, 14 Jun 2023 09:53:53 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Jun 2023 09:54:11 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 14 Jun 2023 09:54:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Wed, 14 Jun 2023 09:54:13 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 14 Jun 2023 09:54:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el7
# Wed, 14 Jun 2023 09:55:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 14 Jun 2023 09:55:16 GMT
VOLUME [/var/lib/mysql]
# Wed, 14 Jun 2023 09:55:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 14 Jun 2023 09:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 09:55:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 09:55:17 GMT
EXPOSE 3306 33060
# Wed, 14 Jun 2023 09:55:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca4383b183f283dc0ac1a0351f5cb31f75dbd244bee8dc0988af4a50f2c59df`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 872.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e282e7651b1612ff17f6246e0847dad6996add940329721a4756a1879f15a23`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 983.7 KB (983711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa0e0ca7078cd2e1abcaa6847bc545576fd23586b4ae3ccc90b31637f27b1f`  
		Last Modified: Wed, 14 Jun 2023 09:55:48 GMT  
		Size: 4.6 MB (4601387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb790cf638212f7a95cd187ed8515ff749c06d616bab23ee7ff4f87969533c7`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7ffc37d8e9c1691a3e04e9fcdf2409484ca22e3b8a1b81e30c0b0ad85551df`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4393c12228b9628c8d3a8c421e92080b206ee9445951e9119fce64d61a7fd143`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 25.5 MB (25534088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389d2c130d520b0e7953b08faa0ad308866e0cb139cd341ddc16501aac8cc3a7`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5df3caef94cc41376f0f14fd6db2c5e224ad013a805aa8df2b5a7a90eed01e5`  
		Last Modified: Wed, 14 Jun 2023 09:55:58 GMT  
		Size: 87.7 MB (87657804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6aa409290d0f55131bc8d7d406e767576e88c510c69b28ac02aaf7167e07c4`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa350980ea9f8455483b598af47fcb9e6d96f5d4b2d50f4d3fdcee486c7f562`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:c0a0e68b9bc8d6cebdbdef8a6e769df5502a361f9190be694bd84e4035fecfb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:9f266e88e9418d3e290303eeff93b2b0b1091e48979dda1407168716e8e00aae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.8 MB (162760797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5d7c63fe3391e41709423d7663a381baea7ee5ca33a923a0a4768009cc45a44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:47 GMT
ADD file:ca4076bfffab8d09636384070ca253570590554cff76a132afaae5cd89b363b5 in / 
# Tue, 04 Jul 2023 01:20:48 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:40:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:40:49 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:40:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:40:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:41:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:41:05 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:41:05 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 04 Jul 2023 16:41:05 GMT
ENV MYSQL_VERSION=5.7.42-1debian10
# Tue, 04 Jul 2023 16:41:06 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Jul 2023 16:41:24 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 04 Jul 2023 16:41:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:41:24 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:41:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:41:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:41:25 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:41:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:90ac1ecaf92c8ae0cb37d29d8cc01b5802612c12edb933c369ad4c586ea94c6c`  
		Last Modified: Tue, 04 Jul 2023 01:26:21 GMT  
		Size: 27.1 MB (27138502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5332fa444fcbc9427056611d173b59e9fb27193696d2caff0ce93902012bf2c`  
		Last Modified: Tue, 04 Jul 2023 16:42:55 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df99bbd075464fe4c45ccfb06b4f3261dcb494b081d2bf090ed8bdb72c6f273`  
		Last Modified: Tue, 04 Jul 2023 16:42:54 GMT  
		Size: 4.2 MB (4182356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1074e6f5cec3a9ad3219a0bf1b7c4d342e68b9311b347a3c0bbdb9b519f104f6`  
		Last Modified: Tue, 04 Jul 2023 16:42:53 GMT  
		Size: 1.4 MB (1441848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bbcb49a75325f17e87e7366fd5499c77bd750fd0a563ecf4fa330598b567ad`  
		Last Modified: Tue, 04 Jul 2023 16:42:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b88e8cde452e8be99b1b7b0e95df9f144877dd3f6a5a751d8d84b5bf98172d`  
		Last Modified: Tue, 04 Jul 2023 16:42:56 GMT  
		Size: 14.1 MB (14089552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd01f08045baa85450d1a60acdb8043f3822f8f08fbc23a6427b43e0d31907b1`  
		Last Modified: Tue, 04 Jul 2023 16:42:51 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6ca6adc2aaa205cfce0083344463b5b459968a0894526ecac3305a1eac1830`  
		Last Modified: Tue, 04 Jul 2023 16:42:51 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57f7cb4781685a978155f98f294792b9c1eaa227c7a22edf025b79e3a5ba5c2`  
		Last Modified: Tue, 04 Jul 2023 16:43:05 GMT  
		Size: 115.9 MB (115898351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d80f44b4d6a403257ac7dfb82cf09de4952b0ce1723f75732a045ba5c92556`  
		Last Modified: Tue, 04 Jul 2023 16:42:51 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2a073f32ef118e7b46e8ff821eb2b0b0a56eb101918cda05b274f0ad3caf49`  
		Last Modified: Tue, 04 Jul 2023 16:42:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:bd873931ef20f30a5a9bf71498ce4e02c88cf48b2e8b782c337076d814deebde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:03b6dcedf5a2754da00e119e2cc6094ed3c884ad36b67bb25fe67be4b4f9bdb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169271448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be84dd575ee2ecdb186dc43a9cd951890a764d2cefbd31a72cdf4410c43a2d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:53:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 14 Jun 2023 09:53:50 GMT
ENV GOSU_VERSION=1.16
# Wed, 14 Jun 2023 09:53:53 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Jun 2023 09:54:11 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 14 Jun 2023 09:54:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Wed, 14 Jun 2023 09:54:13 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 14 Jun 2023 09:54:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el7
# Wed, 14 Jun 2023 09:55:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 14 Jun 2023 09:55:16 GMT
VOLUME [/var/lib/mysql]
# Wed, 14 Jun 2023 09:55:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 14 Jun 2023 09:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 09:55:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 09:55:17 GMT
EXPOSE 3306 33060
# Wed, 14 Jun 2023 09:55:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca4383b183f283dc0ac1a0351f5cb31f75dbd244bee8dc0988af4a50f2c59df`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 872.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e282e7651b1612ff17f6246e0847dad6996add940329721a4756a1879f15a23`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 983.7 KB (983711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa0e0ca7078cd2e1abcaa6847bc545576fd23586b4ae3ccc90b31637f27b1f`  
		Last Modified: Wed, 14 Jun 2023 09:55:48 GMT  
		Size: 4.6 MB (4601387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb790cf638212f7a95cd187ed8515ff749c06d616bab23ee7ff4f87969533c7`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7ffc37d8e9c1691a3e04e9fcdf2409484ca22e3b8a1b81e30c0b0ad85551df`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4393c12228b9628c8d3a8c421e92080b206ee9445951e9119fce64d61a7fd143`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 25.5 MB (25534088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389d2c130d520b0e7953b08faa0ad308866e0cb139cd341ddc16501aac8cc3a7`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5df3caef94cc41376f0f14fd6db2c5e224ad013a805aa8df2b5a7a90eed01e5`  
		Last Modified: Wed, 14 Jun 2023 09:55:58 GMT  
		Size: 87.7 MB (87657804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6aa409290d0f55131bc8d7d406e767576e88c510c69b28ac02aaf7167e07c4`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa350980ea9f8455483b598af47fcb9e6d96f5d4b2d50f4d3fdcee486c7f562`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.42`

```console
$ docker pull mysql@sha256:bd873931ef20f30a5a9bf71498ce4e02c88cf48b2e8b782c337076d814deebde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.42` - linux; amd64

```console
$ docker pull mysql@sha256:03b6dcedf5a2754da00e119e2cc6094ed3c884ad36b67bb25fe67be4b4f9bdb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169271448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be84dd575ee2ecdb186dc43a9cd951890a764d2cefbd31a72cdf4410c43a2d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:53:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 14 Jun 2023 09:53:50 GMT
ENV GOSU_VERSION=1.16
# Wed, 14 Jun 2023 09:53:53 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Jun 2023 09:54:11 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 14 Jun 2023 09:54:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Wed, 14 Jun 2023 09:54:13 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 14 Jun 2023 09:54:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el7
# Wed, 14 Jun 2023 09:55:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 14 Jun 2023 09:55:16 GMT
VOLUME [/var/lib/mysql]
# Wed, 14 Jun 2023 09:55:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 14 Jun 2023 09:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 09:55:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 09:55:17 GMT
EXPOSE 3306 33060
# Wed, 14 Jun 2023 09:55:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca4383b183f283dc0ac1a0351f5cb31f75dbd244bee8dc0988af4a50f2c59df`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 872.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e282e7651b1612ff17f6246e0847dad6996add940329721a4756a1879f15a23`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 983.7 KB (983711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa0e0ca7078cd2e1abcaa6847bc545576fd23586b4ae3ccc90b31637f27b1f`  
		Last Modified: Wed, 14 Jun 2023 09:55:48 GMT  
		Size: 4.6 MB (4601387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb790cf638212f7a95cd187ed8515ff749c06d616bab23ee7ff4f87969533c7`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7ffc37d8e9c1691a3e04e9fcdf2409484ca22e3b8a1b81e30c0b0ad85551df`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4393c12228b9628c8d3a8c421e92080b206ee9445951e9119fce64d61a7fd143`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 25.5 MB (25534088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389d2c130d520b0e7953b08faa0ad308866e0cb139cd341ddc16501aac8cc3a7`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5df3caef94cc41376f0f14fd6db2c5e224ad013a805aa8df2b5a7a90eed01e5`  
		Last Modified: Wed, 14 Jun 2023 09:55:58 GMT  
		Size: 87.7 MB (87657804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6aa409290d0f55131bc8d7d406e767576e88c510c69b28ac02aaf7167e07c4`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa350980ea9f8455483b598af47fcb9e6d96f5d4b2d50f4d3fdcee486c7f562`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.42-debian`

```console
$ docker pull mysql@sha256:c0a0e68b9bc8d6cebdbdef8a6e769df5502a361f9190be694bd84e4035fecfb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.42-debian` - linux; amd64

```console
$ docker pull mysql@sha256:9f266e88e9418d3e290303eeff93b2b0b1091e48979dda1407168716e8e00aae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.8 MB (162760797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5d7c63fe3391e41709423d7663a381baea7ee5ca33a923a0a4768009cc45a44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:47 GMT
ADD file:ca4076bfffab8d09636384070ca253570590554cff76a132afaae5cd89b363b5 in / 
# Tue, 04 Jul 2023 01:20:48 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:40:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:40:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:40:49 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:40:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:40:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:41:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:41:05 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:41:05 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 04 Jul 2023 16:41:05 GMT
ENV MYSQL_VERSION=5.7.42-1debian10
# Tue, 04 Jul 2023 16:41:06 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Jul 2023 16:41:24 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 04 Jul 2023 16:41:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:41:24 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:41:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:41:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:41:25 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:41:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:90ac1ecaf92c8ae0cb37d29d8cc01b5802612c12edb933c369ad4c586ea94c6c`  
		Last Modified: Tue, 04 Jul 2023 01:26:21 GMT  
		Size: 27.1 MB (27138502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5332fa444fcbc9427056611d173b59e9fb27193696d2caff0ce93902012bf2c`  
		Last Modified: Tue, 04 Jul 2023 16:42:55 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df99bbd075464fe4c45ccfb06b4f3261dcb494b081d2bf090ed8bdb72c6f273`  
		Last Modified: Tue, 04 Jul 2023 16:42:54 GMT  
		Size: 4.2 MB (4182356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1074e6f5cec3a9ad3219a0bf1b7c4d342e68b9311b347a3c0bbdb9b519f104f6`  
		Last Modified: Tue, 04 Jul 2023 16:42:53 GMT  
		Size: 1.4 MB (1441848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bbcb49a75325f17e87e7366fd5499c77bd750fd0a563ecf4fa330598b567ad`  
		Last Modified: Tue, 04 Jul 2023 16:42:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b88e8cde452e8be99b1b7b0e95df9f144877dd3f6a5a751d8d84b5bf98172d`  
		Last Modified: Tue, 04 Jul 2023 16:42:56 GMT  
		Size: 14.1 MB (14089552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd01f08045baa85450d1a60acdb8043f3822f8f08fbc23a6427b43e0d31907b1`  
		Last Modified: Tue, 04 Jul 2023 16:42:51 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6ca6adc2aaa205cfce0083344463b5b459968a0894526ecac3305a1eac1830`  
		Last Modified: Tue, 04 Jul 2023 16:42:51 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57f7cb4781685a978155f98f294792b9c1eaa227c7a22edf025b79e3a5ba5c2`  
		Last Modified: Tue, 04 Jul 2023 16:43:05 GMT  
		Size: 115.9 MB (115898351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d80f44b4d6a403257ac7dfb82cf09de4952b0ce1723f75732a045ba5c92556`  
		Last Modified: Tue, 04 Jul 2023 16:42:51 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2a073f32ef118e7b46e8ff821eb2b0b0a56eb101918cda05b274f0ad3caf49`  
		Last Modified: Tue, 04 Jul 2023 16:42:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.42-oracle`

```console
$ docker pull mysql@sha256:bd873931ef20f30a5a9bf71498ce4e02c88cf48b2e8b782c337076d814deebde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.42-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:03b6dcedf5a2754da00e119e2cc6094ed3c884ad36b67bb25fe67be4b4f9bdb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169271448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be84dd575ee2ecdb186dc43a9cd951890a764d2cefbd31a72cdf4410c43a2d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:53:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 14 Jun 2023 09:53:50 GMT
ENV GOSU_VERSION=1.16
# Wed, 14 Jun 2023 09:53:53 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Jun 2023 09:54:11 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 14 Jun 2023 09:54:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Wed, 14 Jun 2023 09:54:13 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 14 Jun 2023 09:54:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el7
# Wed, 14 Jun 2023 09:55:15 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 14 Jun 2023 09:55:16 GMT
VOLUME [/var/lib/mysql]
# Wed, 14 Jun 2023 09:55:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 14 Jun 2023 09:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 14 Jun 2023 09:55:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 09:55:17 GMT
EXPOSE 3306 33060
# Wed, 14 Jun 2023 09:55:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca4383b183f283dc0ac1a0351f5cb31f75dbd244bee8dc0988af4a50f2c59df`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 872.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e282e7651b1612ff17f6246e0847dad6996add940329721a4756a1879f15a23`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 983.7 KB (983711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa0e0ca7078cd2e1abcaa6847bc545576fd23586b4ae3ccc90b31637f27b1f`  
		Last Modified: Wed, 14 Jun 2023 09:55:48 GMT  
		Size: 4.6 MB (4601387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb790cf638212f7a95cd187ed8515ff749c06d616bab23ee7ff4f87969533c7`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7ffc37d8e9c1691a3e04e9fcdf2409484ca22e3b8a1b81e30c0b0ad85551df`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4393c12228b9628c8d3a8c421e92080b206ee9445951e9119fce64d61a7fd143`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 25.5 MB (25534088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389d2c130d520b0e7953b08faa0ad308866e0cb139cd341ddc16501aac8cc3a7`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5df3caef94cc41376f0f14fd6db2c5e224ad013a805aa8df2b5a7a90eed01e5`  
		Last Modified: Wed, 14 Jun 2023 09:55:58 GMT  
		Size: 87.7 MB (87657804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6aa409290d0f55131bc8d7d406e767576e88c510c69b28ac02aaf7167e07c4`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa350980ea9f8455483b598af47fcb9e6d96f5d4b2d50f4d3fdcee486c7f562`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:c84934bc75e80e93f98acac72fdffe3bcd719e2c67443ccd92b25d03b60db2dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:47e045b6313ef483654ac47c31e6fdbfc6ecf6b399a65c03859bee2cfbb1621f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165628492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041315a161837f8bb87361e13390abda7159b98aeedee5e6152a0bb7a9b45f27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:16 GMT
ADD file:7a7c6d19e1a4f691c6bd96ea6b7568f6cc041fce11298e57d51913b978e9e7e3 in / 
# Tue, 04 Jul 2023 02:04:17 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:38:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 16:38:07 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:38:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:38:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 16:39:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:39:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 16:39:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:39:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:39:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:39:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:39:54 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:39:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2c03c89dcad02e83fe01768b82c438fcf60b831104614ca96ed5d8df01db295`  
		Last Modified: Tue, 04 Jul 2023 02:05:27 GMT  
		Size: 44.9 MB (44876686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68eb43837bf88f9e06c8bd54cca2548b7cf92495536d40998a334e0ac299a6e6`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796892ddf5acde022b0881d1683b58c8ea2eca8046b7c63f79a011100ace6581`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bca45eb31e17400b610ab11f38d7fda3319f149326b2c5f712c33a56b9c957f`  
		Last Modified: Tue, 04 Jul 2023 16:41:48 GMT  
		Size: 4.6 MB (4599947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb53bc0dcca4d129ba3e1a91a856537be70a9c5c6032aa5cf9763bf36198fdc`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c6bdc7a40aed4ca602a4bb4ce9781007d5cdb32d661c760d37aeb77273b38`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f27b5c7697033c604eed80da6ab110d7e81ea4e73717c148d7dedd5342f0275`  
		Last Modified: Tue, 04 Jul 2023 16:41:53 GMT  
		Size: 58.6 MB (58595633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438533a248105048d7f275a49f6885462110fd9a37bbe411d12e07a1bf13c7e8`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bdf19985e0de68dd9f165eaea8ff61c961cbee89ebf349fbdc2dc429d0793a`  
		Last Modified: Tue, 04 Jul 2023 16:41:55 GMT  
		Size: 56.6 MB (56563726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667fa148337b6da471bc16887a43ab664e64472abe6f890c50209169de3987c9`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa702110e47beeb15b1dc74593040b23f270479dd8361f0491223c2b65d139`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:62edf9f348c5dcf178e6b600b22318bad18fde151d4766126e5e7b68e16547c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169426885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e6f938c13843277ec4fe0b165319ad8fad9d5638dfc42245e56638314cbae8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 22 Jul 2023 01:21:07 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 22 Jul 2023 01:21:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 22 Jul 2023 01:21:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:21:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 22 Jul 2023 01:21:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 22 Jul 2023 01:21:49 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 22 Jul 2023 01:21:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 22 Jul 2023 01:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Jul 2023 01:21:50 GMT
EXPOSE 3306 33060
# Sat, 22 Jul 2023 01:21:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5db4d9b98684ded0da9ecd2569a4882619860e87910d7982064b73a73035c`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22418c1834882fc37b934c33040fa267cce75b3437ac6e6c1030ca392d8cddd`  
		Last Modified: Sat, 22 Jul 2023 01:22:15 GMT  
		Size: 57.7 MB (57696245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5876e40ed21700302c8cd3ac3ff37a1e71cf871485a5e5ef7241a5dd6239e5`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7221ad5e06ec7f9649161e73793ec55eb8008ffba87b4509e6bf687ea30798eb`  
		Last Modified: Sat, 22 Jul 2023 01:22:17 GMT  
		Size: 62.9 MB (62889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778fd411739775dd92f0708d1251fec5705a9cb9f503fd143c817c3f43feaf7a`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6298de70dec567edc9b0dc265b794a8ad26b9fd1e77038f50c6d34e2af4a4`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:7cade3f2720efda2be0e6184d8e050d1c3b9e84297e18d9a4566173afe41a031
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:1db9b0e99314bae1b8285f369fff1291b8f911bfcbc0e93e3cf8e9aa2c884599
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179716041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5557a1823e3010b0b659f0f388f7fddd2df56326896370cf7a16767089753ae9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:40:01 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:40:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:40:06 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:40:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:40:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:40:21 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:40:21 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 16:40:21 GMT
ENV MYSQL_VERSION=8.0.33-1debian11
# Tue, 04 Jul 2023 16:40:22 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Jul 2023 16:40:37 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 04 Jul 2023 16:40:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:40:38 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 04 Jul 2023 16:40:38 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:40:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:40:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:40:38 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:40:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b694d81657a2feaabf9dd99971bd263fcf6e6365a9088a19fa255cbbbd3bb5`  
		Last Modified: Tue, 04 Jul 2023 16:42:21 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16d5c24c0e588a5ced581dcb0b12a2608480f00d8c9ac214a45b463632263a6`  
		Last Modified: Tue, 04 Jul 2023 16:42:22 GMT  
		Size: 4.4 MB (4415050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c78718e67739ad983a38d623f4bc0f8c5c712b57384f4a852b04c48f87d30c1`  
		Last Modified: Tue, 04 Jul 2023 16:42:20 GMT  
		Size: 1.5 MB (1471510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf8c2abf7d7e75cca7b9d6dd26a939bc3568604779a0e31bf9d077f244d1282`  
		Last Modified: Tue, 04 Jul 2023 16:42:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96b9824aacf27d6bf0a547ca61f950cf76367b65e8857a3a35db10d11ac064d`  
		Last Modified: Tue, 04 Jul 2023 16:42:22 GMT  
		Size: 12.7 MB (12661822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab06d32a3885f91fb15d03b06b1810f1dca279106872eda0260a50f3d204e27b`  
		Last Modified: Tue, 04 Jul 2023 16:42:19 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c8338bebc08fd94875a670c7a3fde461c905aee593ffa00fbe699f98e2fefb`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001a9c226c59f3cfbef49ab0e01347aa3201d202440bfaa469ec84ca4393cf3b`  
		Last Modified: Tue, 04 Jul 2023 16:42:35 GMT  
		Size: 129.7 MB (129739240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bd03e6832e22792ec6507355ca65899a59fb442587ab1b9a2b8ad310298017`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20867e10013d172dbf130c2d282973c83dd13b3bba86a8fab429dff990e9b096`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d2995730ac54cb82ea8294ee1a56fedee0b3d817fa969ed1c998f40f9dd386`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:c84934bc75e80e93f98acac72fdffe3bcd719e2c67443ccd92b25d03b60db2dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:47e045b6313ef483654ac47c31e6fdbfc6ecf6b399a65c03859bee2cfbb1621f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165628492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041315a161837f8bb87361e13390abda7159b98aeedee5e6152a0bb7a9b45f27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:16 GMT
ADD file:7a7c6d19e1a4f691c6bd96ea6b7568f6cc041fce11298e57d51913b978e9e7e3 in / 
# Tue, 04 Jul 2023 02:04:17 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:38:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 16:38:07 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:38:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:38:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 16:39:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:39:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 16:39:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:39:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:39:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:39:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:39:54 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:39:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2c03c89dcad02e83fe01768b82c438fcf60b831104614ca96ed5d8df01db295`  
		Last Modified: Tue, 04 Jul 2023 02:05:27 GMT  
		Size: 44.9 MB (44876686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68eb43837bf88f9e06c8bd54cca2548b7cf92495536d40998a334e0ac299a6e6`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796892ddf5acde022b0881d1683b58c8ea2eca8046b7c63f79a011100ace6581`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bca45eb31e17400b610ab11f38d7fda3319f149326b2c5f712c33a56b9c957f`  
		Last Modified: Tue, 04 Jul 2023 16:41:48 GMT  
		Size: 4.6 MB (4599947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb53bc0dcca4d129ba3e1a91a856537be70a9c5c6032aa5cf9763bf36198fdc`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c6bdc7a40aed4ca602a4bb4ce9781007d5cdb32d661c760d37aeb77273b38`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f27b5c7697033c604eed80da6ab110d7e81ea4e73717c148d7dedd5342f0275`  
		Last Modified: Tue, 04 Jul 2023 16:41:53 GMT  
		Size: 58.6 MB (58595633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438533a248105048d7f275a49f6885462110fd9a37bbe411d12e07a1bf13c7e8`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bdf19985e0de68dd9f165eaea8ff61c961cbee89ebf349fbdc2dc429d0793a`  
		Last Modified: Tue, 04 Jul 2023 16:41:55 GMT  
		Size: 56.6 MB (56563726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667fa148337b6da471bc16887a43ab664e64472abe6f890c50209169de3987c9`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa702110e47beeb15b1dc74593040b23f270479dd8361f0491223c2b65d139`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:62edf9f348c5dcf178e6b600b22318bad18fde151d4766126e5e7b68e16547c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169426885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e6f938c13843277ec4fe0b165319ad8fad9d5638dfc42245e56638314cbae8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 22 Jul 2023 01:21:07 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 22 Jul 2023 01:21:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 22 Jul 2023 01:21:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:21:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 22 Jul 2023 01:21:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 22 Jul 2023 01:21:49 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 22 Jul 2023 01:21:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 22 Jul 2023 01:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Jul 2023 01:21:50 GMT
EXPOSE 3306 33060
# Sat, 22 Jul 2023 01:21:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5db4d9b98684ded0da9ecd2569a4882619860e87910d7982064b73a73035c`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22418c1834882fc37b934c33040fa267cce75b3437ac6e6c1030ca392d8cddd`  
		Last Modified: Sat, 22 Jul 2023 01:22:15 GMT  
		Size: 57.7 MB (57696245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5876e40ed21700302c8cd3ac3ff37a1e71cf871485a5e5ef7241a5dd6239e5`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7221ad5e06ec7f9649161e73793ec55eb8008ffba87b4509e6bf687ea30798eb`  
		Last Modified: Sat, 22 Jul 2023 01:22:17 GMT  
		Size: 62.9 MB (62889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778fd411739775dd92f0708d1251fec5705a9cb9f503fd143c817c3f43feaf7a`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6298de70dec567edc9b0dc265b794a8ad26b9fd1e77038f50c6d34e2af4a4`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:c84934bc75e80e93f98acac72fdffe3bcd719e2c67443ccd92b25d03b60db2dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:47e045b6313ef483654ac47c31e6fdbfc6ecf6b399a65c03859bee2cfbb1621f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165628492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041315a161837f8bb87361e13390abda7159b98aeedee5e6152a0bb7a9b45f27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:16 GMT
ADD file:7a7c6d19e1a4f691c6bd96ea6b7568f6cc041fce11298e57d51913b978e9e7e3 in / 
# Tue, 04 Jul 2023 02:04:17 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:38:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 16:38:07 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:38:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:38:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 16:39:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:39:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 16:39:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:39:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:39:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:39:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:39:54 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:39:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2c03c89dcad02e83fe01768b82c438fcf60b831104614ca96ed5d8df01db295`  
		Last Modified: Tue, 04 Jul 2023 02:05:27 GMT  
		Size: 44.9 MB (44876686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68eb43837bf88f9e06c8bd54cca2548b7cf92495536d40998a334e0ac299a6e6`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796892ddf5acde022b0881d1683b58c8ea2eca8046b7c63f79a011100ace6581`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bca45eb31e17400b610ab11f38d7fda3319f149326b2c5f712c33a56b9c957f`  
		Last Modified: Tue, 04 Jul 2023 16:41:48 GMT  
		Size: 4.6 MB (4599947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb53bc0dcca4d129ba3e1a91a856537be70a9c5c6032aa5cf9763bf36198fdc`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c6bdc7a40aed4ca602a4bb4ce9781007d5cdb32d661c760d37aeb77273b38`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f27b5c7697033c604eed80da6ab110d7e81ea4e73717c148d7dedd5342f0275`  
		Last Modified: Tue, 04 Jul 2023 16:41:53 GMT  
		Size: 58.6 MB (58595633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438533a248105048d7f275a49f6885462110fd9a37bbe411d12e07a1bf13c7e8`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bdf19985e0de68dd9f165eaea8ff61c961cbee89ebf349fbdc2dc429d0793a`  
		Last Modified: Tue, 04 Jul 2023 16:41:55 GMT  
		Size: 56.6 MB (56563726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667fa148337b6da471bc16887a43ab664e64472abe6f890c50209169de3987c9`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa702110e47beeb15b1dc74593040b23f270479dd8361f0491223c2b65d139`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:62edf9f348c5dcf178e6b600b22318bad18fde151d4766126e5e7b68e16547c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169426885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e6f938c13843277ec4fe0b165319ad8fad9d5638dfc42245e56638314cbae8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 22 Jul 2023 01:21:07 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 22 Jul 2023 01:21:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 22 Jul 2023 01:21:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:21:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 22 Jul 2023 01:21:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 22 Jul 2023 01:21:49 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 22 Jul 2023 01:21:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 22 Jul 2023 01:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Jul 2023 01:21:50 GMT
EXPOSE 3306 33060
# Sat, 22 Jul 2023 01:21:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5db4d9b98684ded0da9ecd2569a4882619860e87910d7982064b73a73035c`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22418c1834882fc37b934c33040fa267cce75b3437ac6e6c1030ca392d8cddd`  
		Last Modified: Sat, 22 Jul 2023 01:22:15 GMT  
		Size: 57.7 MB (57696245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5876e40ed21700302c8cd3ac3ff37a1e71cf871485a5e5ef7241a5dd6239e5`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7221ad5e06ec7f9649161e73793ec55eb8008ffba87b4509e6bf687ea30798eb`  
		Last Modified: Sat, 22 Jul 2023 01:22:17 GMT  
		Size: 62.9 MB (62889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778fd411739775dd92f0708d1251fec5705a9cb9f503fd143c817c3f43feaf7a`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6298de70dec567edc9b0dc265b794a8ad26b9fd1e77038f50c6d34e2af4a4`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:7cade3f2720efda2be0e6184d8e050d1c3b9e84297e18d9a4566173afe41a031
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:1db9b0e99314bae1b8285f369fff1291b8f911bfcbc0e93e3cf8e9aa2c884599
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179716041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5557a1823e3010b0b659f0f388f7fddd2df56326896370cf7a16767089753ae9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:40:01 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:40:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:40:06 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:40:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:40:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:40:21 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:40:21 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 16:40:21 GMT
ENV MYSQL_VERSION=8.0.33-1debian11
# Tue, 04 Jul 2023 16:40:22 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Jul 2023 16:40:37 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 04 Jul 2023 16:40:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:40:38 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 04 Jul 2023 16:40:38 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:40:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:40:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:40:38 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:40:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b694d81657a2feaabf9dd99971bd263fcf6e6365a9088a19fa255cbbbd3bb5`  
		Last Modified: Tue, 04 Jul 2023 16:42:21 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16d5c24c0e588a5ced581dcb0b12a2608480f00d8c9ac214a45b463632263a6`  
		Last Modified: Tue, 04 Jul 2023 16:42:22 GMT  
		Size: 4.4 MB (4415050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c78718e67739ad983a38d623f4bc0f8c5c712b57384f4a852b04c48f87d30c1`  
		Last Modified: Tue, 04 Jul 2023 16:42:20 GMT  
		Size: 1.5 MB (1471510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf8c2abf7d7e75cca7b9d6dd26a939bc3568604779a0e31bf9d077f244d1282`  
		Last Modified: Tue, 04 Jul 2023 16:42:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96b9824aacf27d6bf0a547ca61f950cf76367b65e8857a3a35db10d11ac064d`  
		Last Modified: Tue, 04 Jul 2023 16:42:22 GMT  
		Size: 12.7 MB (12661822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab06d32a3885f91fb15d03b06b1810f1dca279106872eda0260a50f3d204e27b`  
		Last Modified: Tue, 04 Jul 2023 16:42:19 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c8338bebc08fd94875a670c7a3fde461c905aee593ffa00fbe699f98e2fefb`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001a9c226c59f3cfbef49ab0e01347aa3201d202440bfaa469ec84ca4393cf3b`  
		Last Modified: Tue, 04 Jul 2023 16:42:35 GMT  
		Size: 129.7 MB (129739240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bd03e6832e22792ec6507355ca65899a59fb442587ab1b9a2b8ad310298017`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20867e10013d172dbf130c2d282973c83dd13b3bba86a8fab429dff990e9b096`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d2995730ac54cb82ea8294ee1a56fedee0b3d817fa969ed1c998f40f9dd386`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:c84934bc75e80e93f98acac72fdffe3bcd719e2c67443ccd92b25d03b60db2dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:47e045b6313ef483654ac47c31e6fdbfc6ecf6b399a65c03859bee2cfbb1621f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165628492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041315a161837f8bb87361e13390abda7159b98aeedee5e6152a0bb7a9b45f27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:16 GMT
ADD file:7a7c6d19e1a4f691c6bd96ea6b7568f6cc041fce11298e57d51913b978e9e7e3 in / 
# Tue, 04 Jul 2023 02:04:17 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:38:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 16:38:07 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:38:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:38:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 16:39:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:39:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 16:39:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:39:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:39:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:39:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:39:54 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:39:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2c03c89dcad02e83fe01768b82c438fcf60b831104614ca96ed5d8df01db295`  
		Last Modified: Tue, 04 Jul 2023 02:05:27 GMT  
		Size: 44.9 MB (44876686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68eb43837bf88f9e06c8bd54cca2548b7cf92495536d40998a334e0ac299a6e6`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796892ddf5acde022b0881d1683b58c8ea2eca8046b7c63f79a011100ace6581`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bca45eb31e17400b610ab11f38d7fda3319f149326b2c5f712c33a56b9c957f`  
		Last Modified: Tue, 04 Jul 2023 16:41:48 GMT  
		Size: 4.6 MB (4599947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb53bc0dcca4d129ba3e1a91a856537be70a9c5c6032aa5cf9763bf36198fdc`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c6bdc7a40aed4ca602a4bb4ce9781007d5cdb32d661c760d37aeb77273b38`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f27b5c7697033c604eed80da6ab110d7e81ea4e73717c148d7dedd5342f0275`  
		Last Modified: Tue, 04 Jul 2023 16:41:53 GMT  
		Size: 58.6 MB (58595633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438533a248105048d7f275a49f6885462110fd9a37bbe411d12e07a1bf13c7e8`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bdf19985e0de68dd9f165eaea8ff61c961cbee89ebf349fbdc2dc429d0793a`  
		Last Modified: Tue, 04 Jul 2023 16:41:55 GMT  
		Size: 56.6 MB (56563726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667fa148337b6da471bc16887a43ab664e64472abe6f890c50209169de3987c9`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa702110e47beeb15b1dc74593040b23f270479dd8361f0491223c2b65d139`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:62edf9f348c5dcf178e6b600b22318bad18fde151d4766126e5e7b68e16547c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169426885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e6f938c13843277ec4fe0b165319ad8fad9d5638dfc42245e56638314cbae8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 22 Jul 2023 01:21:07 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 22 Jul 2023 01:21:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 22 Jul 2023 01:21:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:21:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 22 Jul 2023 01:21:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 22 Jul 2023 01:21:49 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 22 Jul 2023 01:21:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 22 Jul 2023 01:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Jul 2023 01:21:50 GMT
EXPOSE 3306 33060
# Sat, 22 Jul 2023 01:21:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5db4d9b98684ded0da9ecd2569a4882619860e87910d7982064b73a73035c`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22418c1834882fc37b934c33040fa267cce75b3437ac6e6c1030ca392d8cddd`  
		Last Modified: Sat, 22 Jul 2023 01:22:15 GMT  
		Size: 57.7 MB (57696245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5876e40ed21700302c8cd3ac3ff37a1e71cf871485a5e5ef7241a5dd6239e5`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7221ad5e06ec7f9649161e73793ec55eb8008ffba87b4509e6bf687ea30798eb`  
		Last Modified: Sat, 22 Jul 2023 01:22:17 GMT  
		Size: 62.9 MB (62889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778fd411739775dd92f0708d1251fec5705a9cb9f503fd143c817c3f43feaf7a`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6298de70dec567edc9b0dc265b794a8ad26b9fd1e77038f50c6d34e2af4a4`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.33`

```console
$ docker pull mysql@sha256:c84934bc75e80e93f98acac72fdffe3bcd719e2c67443ccd92b25d03b60db2dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.33` - linux; amd64

```console
$ docker pull mysql@sha256:47e045b6313ef483654ac47c31e6fdbfc6ecf6b399a65c03859bee2cfbb1621f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165628492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041315a161837f8bb87361e13390abda7159b98aeedee5e6152a0bb7a9b45f27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:16 GMT
ADD file:7a7c6d19e1a4f691c6bd96ea6b7568f6cc041fce11298e57d51913b978e9e7e3 in / 
# Tue, 04 Jul 2023 02:04:17 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:38:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 16:38:07 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:38:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:38:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 16:39:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:39:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 16:39:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:39:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:39:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:39:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:39:54 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:39:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2c03c89dcad02e83fe01768b82c438fcf60b831104614ca96ed5d8df01db295`  
		Last Modified: Tue, 04 Jul 2023 02:05:27 GMT  
		Size: 44.9 MB (44876686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68eb43837bf88f9e06c8bd54cca2548b7cf92495536d40998a334e0ac299a6e6`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796892ddf5acde022b0881d1683b58c8ea2eca8046b7c63f79a011100ace6581`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bca45eb31e17400b610ab11f38d7fda3319f149326b2c5f712c33a56b9c957f`  
		Last Modified: Tue, 04 Jul 2023 16:41:48 GMT  
		Size: 4.6 MB (4599947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb53bc0dcca4d129ba3e1a91a856537be70a9c5c6032aa5cf9763bf36198fdc`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c6bdc7a40aed4ca602a4bb4ce9781007d5cdb32d661c760d37aeb77273b38`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f27b5c7697033c604eed80da6ab110d7e81ea4e73717c148d7dedd5342f0275`  
		Last Modified: Tue, 04 Jul 2023 16:41:53 GMT  
		Size: 58.6 MB (58595633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438533a248105048d7f275a49f6885462110fd9a37bbe411d12e07a1bf13c7e8`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bdf19985e0de68dd9f165eaea8ff61c961cbee89ebf349fbdc2dc429d0793a`  
		Last Modified: Tue, 04 Jul 2023 16:41:55 GMT  
		Size: 56.6 MB (56563726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667fa148337b6da471bc16887a43ab664e64472abe6f890c50209169de3987c9`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa702110e47beeb15b1dc74593040b23f270479dd8361f0491223c2b65d139`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.33` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:62edf9f348c5dcf178e6b600b22318bad18fde151d4766126e5e7b68e16547c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169426885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e6f938c13843277ec4fe0b165319ad8fad9d5638dfc42245e56638314cbae8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 22 Jul 2023 01:21:07 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 22 Jul 2023 01:21:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 22 Jul 2023 01:21:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:21:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 22 Jul 2023 01:21:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 22 Jul 2023 01:21:49 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 22 Jul 2023 01:21:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 22 Jul 2023 01:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Jul 2023 01:21:50 GMT
EXPOSE 3306 33060
# Sat, 22 Jul 2023 01:21:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5db4d9b98684ded0da9ecd2569a4882619860e87910d7982064b73a73035c`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22418c1834882fc37b934c33040fa267cce75b3437ac6e6c1030ca392d8cddd`  
		Last Modified: Sat, 22 Jul 2023 01:22:15 GMT  
		Size: 57.7 MB (57696245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5876e40ed21700302c8cd3ac3ff37a1e71cf871485a5e5ef7241a5dd6239e5`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7221ad5e06ec7f9649161e73793ec55eb8008ffba87b4509e6bf687ea30798eb`  
		Last Modified: Sat, 22 Jul 2023 01:22:17 GMT  
		Size: 62.9 MB (62889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778fd411739775dd92f0708d1251fec5705a9cb9f503fd143c817c3f43feaf7a`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6298de70dec567edc9b0dc265b794a8ad26b9fd1e77038f50c6d34e2af4a4`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.33-debian`

```console
$ docker pull mysql@sha256:7cade3f2720efda2be0e6184d8e050d1c3b9e84297e18d9a4566173afe41a031
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.33-debian` - linux; amd64

```console
$ docker pull mysql@sha256:1db9b0e99314bae1b8285f369fff1291b8f911bfcbc0e93e3cf8e9aa2c884599
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179716041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5557a1823e3010b0b659f0f388f7fddd2df56326896370cf7a16767089753ae9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:40:01 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:40:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:40:06 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:40:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:40:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:40:21 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:40:21 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 16:40:21 GMT
ENV MYSQL_VERSION=8.0.33-1debian11
# Tue, 04 Jul 2023 16:40:22 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Jul 2023 16:40:37 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 04 Jul 2023 16:40:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:40:38 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 04 Jul 2023 16:40:38 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:40:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:40:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:40:38 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:40:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b694d81657a2feaabf9dd99971bd263fcf6e6365a9088a19fa255cbbbd3bb5`  
		Last Modified: Tue, 04 Jul 2023 16:42:21 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16d5c24c0e588a5ced581dcb0b12a2608480f00d8c9ac214a45b463632263a6`  
		Last Modified: Tue, 04 Jul 2023 16:42:22 GMT  
		Size: 4.4 MB (4415050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c78718e67739ad983a38d623f4bc0f8c5c712b57384f4a852b04c48f87d30c1`  
		Last Modified: Tue, 04 Jul 2023 16:42:20 GMT  
		Size: 1.5 MB (1471510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf8c2abf7d7e75cca7b9d6dd26a939bc3568604779a0e31bf9d077f244d1282`  
		Last Modified: Tue, 04 Jul 2023 16:42:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96b9824aacf27d6bf0a547ca61f950cf76367b65e8857a3a35db10d11ac064d`  
		Last Modified: Tue, 04 Jul 2023 16:42:22 GMT  
		Size: 12.7 MB (12661822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab06d32a3885f91fb15d03b06b1810f1dca279106872eda0260a50f3d204e27b`  
		Last Modified: Tue, 04 Jul 2023 16:42:19 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c8338bebc08fd94875a670c7a3fde461c905aee593ffa00fbe699f98e2fefb`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001a9c226c59f3cfbef49ab0e01347aa3201d202440bfaa469ec84ca4393cf3b`  
		Last Modified: Tue, 04 Jul 2023 16:42:35 GMT  
		Size: 129.7 MB (129739240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bd03e6832e22792ec6507355ca65899a59fb442587ab1b9a2b8ad310298017`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20867e10013d172dbf130c2d282973c83dd13b3bba86a8fab429dff990e9b096`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d2995730ac54cb82ea8294ee1a56fedee0b3d817fa969ed1c998f40f9dd386`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.33-oracle`

```console
$ docker pull mysql@sha256:c84934bc75e80e93f98acac72fdffe3bcd719e2c67443ccd92b25d03b60db2dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.33-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:47e045b6313ef483654ac47c31e6fdbfc6ecf6b399a65c03859bee2cfbb1621f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165628492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041315a161837f8bb87361e13390abda7159b98aeedee5e6152a0bb7a9b45f27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:16 GMT
ADD file:7a7c6d19e1a4f691c6bd96ea6b7568f6cc041fce11298e57d51913b978e9e7e3 in / 
# Tue, 04 Jul 2023 02:04:17 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:38:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 16:38:07 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:38:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:38:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 16:39:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:39:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 16:39:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:39:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:39:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:39:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:39:54 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:39:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2c03c89dcad02e83fe01768b82c438fcf60b831104614ca96ed5d8df01db295`  
		Last Modified: Tue, 04 Jul 2023 02:05:27 GMT  
		Size: 44.9 MB (44876686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68eb43837bf88f9e06c8bd54cca2548b7cf92495536d40998a334e0ac299a6e6`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796892ddf5acde022b0881d1683b58c8ea2eca8046b7c63f79a011100ace6581`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bca45eb31e17400b610ab11f38d7fda3319f149326b2c5f712c33a56b9c957f`  
		Last Modified: Tue, 04 Jul 2023 16:41:48 GMT  
		Size: 4.6 MB (4599947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb53bc0dcca4d129ba3e1a91a856537be70a9c5c6032aa5cf9763bf36198fdc`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c6bdc7a40aed4ca602a4bb4ce9781007d5cdb32d661c760d37aeb77273b38`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f27b5c7697033c604eed80da6ab110d7e81ea4e73717c148d7dedd5342f0275`  
		Last Modified: Tue, 04 Jul 2023 16:41:53 GMT  
		Size: 58.6 MB (58595633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438533a248105048d7f275a49f6885462110fd9a37bbe411d12e07a1bf13c7e8`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bdf19985e0de68dd9f165eaea8ff61c961cbee89ebf349fbdc2dc429d0793a`  
		Last Modified: Tue, 04 Jul 2023 16:41:55 GMT  
		Size: 56.6 MB (56563726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667fa148337b6da471bc16887a43ab664e64472abe6f890c50209169de3987c9`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa702110e47beeb15b1dc74593040b23f270479dd8361f0491223c2b65d139`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.33-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:62edf9f348c5dcf178e6b600b22318bad18fde151d4766126e5e7b68e16547c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169426885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e6f938c13843277ec4fe0b165319ad8fad9d5638dfc42245e56638314cbae8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 22 Jul 2023 01:21:07 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 22 Jul 2023 01:21:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 22 Jul 2023 01:21:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:21:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 22 Jul 2023 01:21:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 22 Jul 2023 01:21:49 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 22 Jul 2023 01:21:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 22 Jul 2023 01:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Jul 2023 01:21:50 GMT
EXPOSE 3306 33060
# Sat, 22 Jul 2023 01:21:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5db4d9b98684ded0da9ecd2569a4882619860e87910d7982064b73a73035c`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22418c1834882fc37b934c33040fa267cce75b3437ac6e6c1030ca392d8cddd`  
		Last Modified: Sat, 22 Jul 2023 01:22:15 GMT  
		Size: 57.7 MB (57696245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5876e40ed21700302c8cd3ac3ff37a1e71cf871485a5e5ef7241a5dd6239e5`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7221ad5e06ec7f9649161e73793ec55eb8008ffba87b4509e6bf687ea30798eb`  
		Last Modified: Sat, 22 Jul 2023 01:22:17 GMT  
		Size: 62.9 MB (62889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778fd411739775dd92f0708d1251fec5705a9cb9f503fd143c817c3f43feaf7a`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6298de70dec567edc9b0dc265b794a8ad26b9fd1e77038f50c6d34e2af4a4`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:7cade3f2720efda2be0e6184d8e050d1c3b9e84297e18d9a4566173afe41a031
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:1db9b0e99314bae1b8285f369fff1291b8f911bfcbc0e93e3cf8e9aa2c884599
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179716041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5557a1823e3010b0b659f0f388f7fddd2df56326896370cf7a16767089753ae9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:40:01 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Jul 2023 16:40:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:40:06 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:40:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:40:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 16:40:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:40:21 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:40:21 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 16:40:21 GMT
ENV MYSQL_VERSION=8.0.33-1debian11
# Tue, 04 Jul 2023 16:40:22 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Jul 2023 16:40:37 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 04 Jul 2023 16:40:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:40:38 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 04 Jul 2023 16:40:38 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:40:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:40:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:40:38 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:40:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b694d81657a2feaabf9dd99971bd263fcf6e6365a9088a19fa255cbbbd3bb5`  
		Last Modified: Tue, 04 Jul 2023 16:42:21 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16d5c24c0e588a5ced581dcb0b12a2608480f00d8c9ac214a45b463632263a6`  
		Last Modified: Tue, 04 Jul 2023 16:42:22 GMT  
		Size: 4.4 MB (4415050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c78718e67739ad983a38d623f4bc0f8c5c712b57384f4a852b04c48f87d30c1`  
		Last Modified: Tue, 04 Jul 2023 16:42:20 GMT  
		Size: 1.5 MB (1471510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf8c2abf7d7e75cca7b9d6dd26a939bc3568604779a0e31bf9d077f244d1282`  
		Last Modified: Tue, 04 Jul 2023 16:42:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96b9824aacf27d6bf0a547ca61f950cf76367b65e8857a3a35db10d11ac064d`  
		Last Modified: Tue, 04 Jul 2023 16:42:22 GMT  
		Size: 12.7 MB (12661822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab06d32a3885f91fb15d03b06b1810f1dca279106872eda0260a50f3d204e27b`  
		Last Modified: Tue, 04 Jul 2023 16:42:19 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c8338bebc08fd94875a670c7a3fde461c905aee593ffa00fbe699f98e2fefb`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001a9c226c59f3cfbef49ab0e01347aa3201d202440bfaa469ec84ca4393cf3b`  
		Last Modified: Tue, 04 Jul 2023 16:42:35 GMT  
		Size: 129.7 MB (129739240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bd03e6832e22792ec6507355ca65899a59fb442587ab1b9a2b8ad310298017`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20867e10013d172dbf130c2d282973c83dd13b3bba86a8fab429dff990e9b096`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d2995730ac54cb82ea8294ee1a56fedee0b3d817fa969ed1c998f40f9dd386`  
		Last Modified: Tue, 04 Jul 2023 16:42:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:c84934bc75e80e93f98acac72fdffe3bcd719e2c67443ccd92b25d03b60db2dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:47e045b6313ef483654ac47c31e6fdbfc6ecf6b399a65c03859bee2cfbb1621f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165628492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041315a161837f8bb87361e13390abda7159b98aeedee5e6152a0bb7a9b45f27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:16 GMT
ADD file:7a7c6d19e1a4f691c6bd96ea6b7568f6cc041fce11298e57d51913b978e9e7e3 in / 
# Tue, 04 Jul 2023 02:04:17 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:38:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 16:38:07 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:38:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:38:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 16:39:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:39:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 16:39:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:39:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:39:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:39:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:39:54 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:39:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2c03c89dcad02e83fe01768b82c438fcf60b831104614ca96ed5d8df01db295`  
		Last Modified: Tue, 04 Jul 2023 02:05:27 GMT  
		Size: 44.9 MB (44876686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68eb43837bf88f9e06c8bd54cca2548b7cf92495536d40998a334e0ac299a6e6`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796892ddf5acde022b0881d1683b58c8ea2eca8046b7c63f79a011100ace6581`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bca45eb31e17400b610ab11f38d7fda3319f149326b2c5f712c33a56b9c957f`  
		Last Modified: Tue, 04 Jul 2023 16:41:48 GMT  
		Size: 4.6 MB (4599947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb53bc0dcca4d129ba3e1a91a856537be70a9c5c6032aa5cf9763bf36198fdc`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c6bdc7a40aed4ca602a4bb4ce9781007d5cdb32d661c760d37aeb77273b38`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f27b5c7697033c604eed80da6ab110d7e81ea4e73717c148d7dedd5342f0275`  
		Last Modified: Tue, 04 Jul 2023 16:41:53 GMT  
		Size: 58.6 MB (58595633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438533a248105048d7f275a49f6885462110fd9a37bbe411d12e07a1bf13c7e8`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bdf19985e0de68dd9f165eaea8ff61c961cbee89ebf349fbdc2dc429d0793a`  
		Last Modified: Tue, 04 Jul 2023 16:41:55 GMT  
		Size: 56.6 MB (56563726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667fa148337b6da471bc16887a43ab664e64472abe6f890c50209169de3987c9`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa702110e47beeb15b1dc74593040b23f270479dd8361f0491223c2b65d139`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:62edf9f348c5dcf178e6b600b22318bad18fde151d4766126e5e7b68e16547c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169426885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e6f938c13843277ec4fe0b165319ad8fad9d5638dfc42245e56638314cbae8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 22 Jul 2023 01:21:07 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 22 Jul 2023 01:21:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 22 Jul 2023 01:21:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:21:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 22 Jul 2023 01:21:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 22 Jul 2023 01:21:49 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 22 Jul 2023 01:21:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 22 Jul 2023 01:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Jul 2023 01:21:50 GMT
EXPOSE 3306 33060
# Sat, 22 Jul 2023 01:21:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5db4d9b98684ded0da9ecd2569a4882619860e87910d7982064b73a73035c`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22418c1834882fc37b934c33040fa267cce75b3437ac6e6c1030ca392d8cddd`  
		Last Modified: Sat, 22 Jul 2023 01:22:15 GMT  
		Size: 57.7 MB (57696245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5876e40ed21700302c8cd3ac3ff37a1e71cf871485a5e5ef7241a5dd6239e5`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7221ad5e06ec7f9649161e73793ec55eb8008ffba87b4509e6bf687ea30798eb`  
		Last Modified: Sat, 22 Jul 2023 01:22:17 GMT  
		Size: 62.9 MB (62889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778fd411739775dd92f0708d1251fec5705a9cb9f503fd143c817c3f43feaf7a`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6298de70dec567edc9b0dc265b794a8ad26b9fd1e77038f50c6d34e2af4a4`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:c84934bc75e80e93f98acac72fdffe3bcd719e2c67443ccd92b25d03b60db2dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:47e045b6313ef483654ac47c31e6fdbfc6ecf6b399a65c03859bee2cfbb1621f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165628492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041315a161837f8bb87361e13390abda7159b98aeedee5e6152a0bb7a9b45f27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:16 GMT
ADD file:7a7c6d19e1a4f691c6bd96ea6b7568f6cc041fce11298e57d51913b978e9e7e3 in / 
# Tue, 04 Jul 2023 02:04:17 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:38:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 16:38:07 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 16:38:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 16:38:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 16:38:39 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:38:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 16:39:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 16:39:15 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 16:39:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 16:39:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 16:39:53 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:39:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 16:39:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:39:54 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 16:39:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2c03c89dcad02e83fe01768b82c438fcf60b831104614ca96ed5d8df01db295`  
		Last Modified: Tue, 04 Jul 2023 02:05:27 GMT  
		Size: 44.9 MB (44876686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68eb43837bf88f9e06c8bd54cca2548b7cf92495536d40998a334e0ac299a6e6`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796892ddf5acde022b0881d1683b58c8ea2eca8046b7c63f79a011100ace6581`  
		Last Modified: Tue, 04 Jul 2023 16:41:49 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bca45eb31e17400b610ab11f38d7fda3319f149326b2c5f712c33a56b9c957f`  
		Last Modified: Tue, 04 Jul 2023 16:41:48 GMT  
		Size: 4.6 MB (4599947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb53bc0dcca4d129ba3e1a91a856537be70a9c5c6032aa5cf9763bf36198fdc`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c6bdc7a40aed4ca602a4bb4ce9781007d5cdb32d661c760d37aeb77273b38`  
		Last Modified: Tue, 04 Jul 2023 16:41:47 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f27b5c7697033c604eed80da6ab110d7e81ea4e73717c148d7dedd5342f0275`  
		Last Modified: Tue, 04 Jul 2023 16:41:53 GMT  
		Size: 58.6 MB (58595633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438533a248105048d7f275a49f6885462110fd9a37bbe411d12e07a1bf13c7e8`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bdf19985e0de68dd9f165eaea8ff61c961cbee89ebf349fbdc2dc429d0793a`  
		Last Modified: Tue, 04 Jul 2023 16:41:55 GMT  
		Size: 56.6 MB (56563726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667fa148337b6da471bc16887a43ab664e64472abe6f890c50209169de3987c9`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 5.4 KB (5395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baa702110e47beeb15b1dc74593040b23f270479dd8361f0491223c2b65d139`  
		Last Modified: Tue, 04 Jul 2023 16:41:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:62edf9f348c5dcf178e6b600b22318bad18fde151d4766126e5e7b68e16547c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169426885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e6f938c13843277ec4fe0b165319ad8fad9d5638dfc42245e56638314cbae8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 22 Jul 2023 01:21:07 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 22 Jul 2023 01:21:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 22 Jul 2023 01:21:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Sat, 22 Jul 2023 01:21:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 22 Jul 2023 01:21:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 22 Jul 2023 01:21:49 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 22 Jul 2023 01:21:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 22 Jul 2023 01:21:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Jul 2023 01:21:50 GMT
EXPOSE 3306 33060
# Sat, 22 Jul 2023 01:21:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b5db4d9b98684ded0da9ecd2569a4882619860e87910d7982064b73a73035c`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22418c1834882fc37b934c33040fa267cce75b3437ac6e6c1030ca392d8cddd`  
		Last Modified: Sat, 22 Jul 2023 01:22:15 GMT  
		Size: 57.7 MB (57696245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5876e40ed21700302c8cd3ac3ff37a1e71cf871485a5e5ef7241a5dd6239e5`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7221ad5e06ec7f9649161e73793ec55eb8008ffba87b4509e6bf687ea30798eb`  
		Last Modified: Sat, 22 Jul 2023 01:22:17 GMT  
		Size: 62.9 MB (62889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778fd411739775dd92f0708d1251fec5705a9cb9f503fd143c817c3f43feaf7a`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6298de70dec567edc9b0dc265b794a8ad26b9fd1e77038f50c6d34e2af4a4`  
		Last Modified: Sat, 22 Jul 2023 01:22:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
