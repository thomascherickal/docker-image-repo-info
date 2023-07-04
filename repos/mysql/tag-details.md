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
$ docker pull mysql@sha256:dd29f448c221a5ccd8d7545394772af6fe02925935e45a1c1e803ca1c08274f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:29ea1f451c3aad88df5a24288f76442286dc7fa6874d96a022e93a8a7efda880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165650520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b53e2624b431e562ed9076a9a506c5e78387f2cb4dad5968fd51ade839baa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 16 Jun 2023 00:20:42 GMT
ADD file:9f649031a04a4d0b24cc167d52bbd5ae3415fd808304c971291e35e75109822a in / 
# Fri, 16 Jun 2023 00:20:43 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:37:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 16 Jun 2023 00:37:33 GMT
ENV GOSU_VERSION=1.16
# Fri, 16 Jun 2023 00:37:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 00:38:03 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 16 Jun 2023 00:38:37 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 16 Jun 2023 00:38:38 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 16 Jun 2023 00:38:38 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:39:15 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 16 Jun 2023 00:39:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 16 Jun 2023 00:39:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 16 Jun 2023 00:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 16 Jun 2023 00:39:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 00:39:16 GMT
EXPOSE 3306 33060
# Fri, 16 Jun 2023 00:39:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:46ef68baacb785b3cf2f2826bfce791acb5264bed0fdf301623ac0c3c57f4daf`  
		Last Modified: Fri, 16 Jun 2023 00:22:14 GMT  
		Size: 44.9 MB (44871780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c1114b2e9c0ba99041080c16f9cd2cc0b58f3ba47400cbeded060ae9aa2a58`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05e3f388023fb59f887c07497c9d09720f06e7c9c0641c8650c91219d992ef`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cc3fcd99122af19a3586bbd08f963df55c278e637c28789868871e57ac52be`  
		Last Modified: Fri, 16 Jun 2023 00:39:46 GMT  
		Size: 4.6 MB (4612914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bbc8bdf52a1396cf678cea6022e4ddd772594aa67be88ee5d2526dca4f8119`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d88f83726a9409e62c9e5bdbe16cfe138ef4815a0e60012438c6df0e3170102`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c7d5d33f72689fd134bf4550db3753da17ad9ac56aa5bd15f7b9a1bb7453c`  
		Last Modified: Fri, 16 Jun 2023 00:39:52 GMT  
		Size: 58.6 MB (58602433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3175a2a660e9718faf64d43427ec34dd44af39a81c68c2a231bf10f6ae1c9`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaedeb27fa9b58368158724d925fe3ceda7fc4db137e4c56a6fb9f25a24e5d2`  
		Last Modified: Fri, 16 Jun 2023 00:39:53 GMT  
		Size: 56.6 MB (56570890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf91e7784414e9912ef38afc2c6771177cd73be84a212ba7fe23799f66e9699f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1770db1c329de5a86e8685058094ee739297578f72fbfb376991078c288c59f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1d42cf001a7bd8cb99fcc41ff98730b69094317cd3f78f9e9990c289e193da7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169420967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772571a08c67835aed7436d84973e885cc439b6cdd4dd1cc661a907d8acd3591`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 00:52:20 GMT
ADD file:1313260ee8b32fa94bcf06c44034cd7e4f9baf44c7df9e74facfe21323b37292 in / 
# Tue, 04 Jul 2023 00:52:21 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 01:28:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 01:28:04 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 01:28:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 01:28:31 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 01:29:02 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 01:29:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 01:29:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:29:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 01:29:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 01:29:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 01:29:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 01:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 01:29:41 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 01:29:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:29e800056b7e3d5007df41c0ad55416bb45d5863affcf39316c5755e71b20a30`  
		Last Modified: Tue, 04 Jul 2023 00:53:16 GMT  
		Size: 43.6 MB (43595268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69da292eb326146b0c10267953b72d6fcd767e284c36c30d51473fbcb67ca5a2`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850ef02dd581452d67b8bb9f54cd949b21fb95ff57bde8fadec5902bd385695`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 913.0 KB (913006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a76caa9e2025c7ecf56e460c12252a1216f8ac7773a0c7b289628b6c53760d`  
		Last Modified: Tue, 04 Jul 2023 01:30:07 GMT  
		Size: 4.3 MB (4298277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881324b108321b7769c7d33bb4b0d2ae626a06ae82441448e5d3c1c5e0eebf77`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5d1a8fa489bd8a99aeade310f01d71c431979332edfd44d3f2f02c7fa531fb`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efbe9eacf59876277173d2d29ad4fbe9be9678e82ea7308ef0f816b862a0653`  
		Last Modified: Tue, 04 Jul 2023 01:30:09 GMT  
		Size: 57.7 MB (57696479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80db22f26c0faf0e95ac6454baa4179c1c6481a688d8473246a212c1cfe9ee24`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5595b935c31c94590c65a3bd92f06b5f4e56874b04b4d8c351cd03327c4c7dc`  
		Last Modified: Tue, 04 Jul 2023 01:30:12 GMT  
		Size: 62.9 MB (62908250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c391d4efe15967c07ecfcbb07109613e9d801d994a094624dc6881fec27f5eb7`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 5.4 KB (5396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5527cf2eb5f0f72a2582baa44f61182d16ea054b51bff962ef6760480e17ba9`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
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
$ docker pull mysql@sha256:dd29f448c221a5ccd8d7545394772af6fe02925935e45a1c1e803ca1c08274f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:29ea1f451c3aad88df5a24288f76442286dc7fa6874d96a022e93a8a7efda880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165650520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b53e2624b431e562ed9076a9a506c5e78387f2cb4dad5968fd51ade839baa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 16 Jun 2023 00:20:42 GMT
ADD file:9f649031a04a4d0b24cc167d52bbd5ae3415fd808304c971291e35e75109822a in / 
# Fri, 16 Jun 2023 00:20:43 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:37:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 16 Jun 2023 00:37:33 GMT
ENV GOSU_VERSION=1.16
# Fri, 16 Jun 2023 00:37:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 00:38:03 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 16 Jun 2023 00:38:37 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 16 Jun 2023 00:38:38 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 16 Jun 2023 00:38:38 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:39:15 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 16 Jun 2023 00:39:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 16 Jun 2023 00:39:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 16 Jun 2023 00:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 16 Jun 2023 00:39:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 00:39:16 GMT
EXPOSE 3306 33060
# Fri, 16 Jun 2023 00:39:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:46ef68baacb785b3cf2f2826bfce791acb5264bed0fdf301623ac0c3c57f4daf`  
		Last Modified: Fri, 16 Jun 2023 00:22:14 GMT  
		Size: 44.9 MB (44871780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c1114b2e9c0ba99041080c16f9cd2cc0b58f3ba47400cbeded060ae9aa2a58`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05e3f388023fb59f887c07497c9d09720f06e7c9c0641c8650c91219d992ef`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cc3fcd99122af19a3586bbd08f963df55c278e637c28789868871e57ac52be`  
		Last Modified: Fri, 16 Jun 2023 00:39:46 GMT  
		Size: 4.6 MB (4612914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bbc8bdf52a1396cf678cea6022e4ddd772594aa67be88ee5d2526dca4f8119`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d88f83726a9409e62c9e5bdbe16cfe138ef4815a0e60012438c6df0e3170102`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c7d5d33f72689fd134bf4550db3753da17ad9ac56aa5bd15f7b9a1bb7453c`  
		Last Modified: Fri, 16 Jun 2023 00:39:52 GMT  
		Size: 58.6 MB (58602433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3175a2a660e9718faf64d43427ec34dd44af39a81c68c2a231bf10f6ae1c9`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaedeb27fa9b58368158724d925fe3ceda7fc4db137e4c56a6fb9f25a24e5d2`  
		Last Modified: Fri, 16 Jun 2023 00:39:53 GMT  
		Size: 56.6 MB (56570890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf91e7784414e9912ef38afc2c6771177cd73be84a212ba7fe23799f66e9699f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1770db1c329de5a86e8685058094ee739297578f72fbfb376991078c288c59f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1d42cf001a7bd8cb99fcc41ff98730b69094317cd3f78f9e9990c289e193da7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169420967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772571a08c67835aed7436d84973e885cc439b6cdd4dd1cc661a907d8acd3591`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 00:52:20 GMT
ADD file:1313260ee8b32fa94bcf06c44034cd7e4f9baf44c7df9e74facfe21323b37292 in / 
# Tue, 04 Jul 2023 00:52:21 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 01:28:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 01:28:04 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 01:28:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 01:28:31 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 01:29:02 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 01:29:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 01:29:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:29:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 01:29:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 01:29:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 01:29:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 01:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 01:29:41 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 01:29:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:29e800056b7e3d5007df41c0ad55416bb45d5863affcf39316c5755e71b20a30`  
		Last Modified: Tue, 04 Jul 2023 00:53:16 GMT  
		Size: 43.6 MB (43595268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69da292eb326146b0c10267953b72d6fcd767e284c36c30d51473fbcb67ca5a2`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850ef02dd581452d67b8bb9f54cd949b21fb95ff57bde8fadec5902bd385695`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 913.0 KB (913006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a76caa9e2025c7ecf56e460c12252a1216f8ac7773a0c7b289628b6c53760d`  
		Last Modified: Tue, 04 Jul 2023 01:30:07 GMT  
		Size: 4.3 MB (4298277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881324b108321b7769c7d33bb4b0d2ae626a06ae82441448e5d3c1c5e0eebf77`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5d1a8fa489bd8a99aeade310f01d71c431979332edfd44d3f2f02c7fa531fb`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efbe9eacf59876277173d2d29ad4fbe9be9678e82ea7308ef0f816b862a0653`  
		Last Modified: Tue, 04 Jul 2023 01:30:09 GMT  
		Size: 57.7 MB (57696479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80db22f26c0faf0e95ac6454baa4179c1c6481a688d8473246a212c1cfe9ee24`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5595b935c31c94590c65a3bd92f06b5f4e56874b04b4d8c351cd03327c4c7dc`  
		Last Modified: Tue, 04 Jul 2023 01:30:12 GMT  
		Size: 62.9 MB (62908250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c391d4efe15967c07ecfcbb07109613e9d801d994a094624dc6881fec27f5eb7`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 5.4 KB (5396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5527cf2eb5f0f72a2582baa44f61182d16ea054b51bff962ef6760480e17ba9`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:dd29f448c221a5ccd8d7545394772af6fe02925935e45a1c1e803ca1c08274f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:29ea1f451c3aad88df5a24288f76442286dc7fa6874d96a022e93a8a7efda880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165650520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b53e2624b431e562ed9076a9a506c5e78387f2cb4dad5968fd51ade839baa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 16 Jun 2023 00:20:42 GMT
ADD file:9f649031a04a4d0b24cc167d52bbd5ae3415fd808304c971291e35e75109822a in / 
# Fri, 16 Jun 2023 00:20:43 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:37:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 16 Jun 2023 00:37:33 GMT
ENV GOSU_VERSION=1.16
# Fri, 16 Jun 2023 00:37:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 00:38:03 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 16 Jun 2023 00:38:37 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 16 Jun 2023 00:38:38 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 16 Jun 2023 00:38:38 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:39:15 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 16 Jun 2023 00:39:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 16 Jun 2023 00:39:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 16 Jun 2023 00:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 16 Jun 2023 00:39:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 00:39:16 GMT
EXPOSE 3306 33060
# Fri, 16 Jun 2023 00:39:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:46ef68baacb785b3cf2f2826bfce791acb5264bed0fdf301623ac0c3c57f4daf`  
		Last Modified: Fri, 16 Jun 2023 00:22:14 GMT  
		Size: 44.9 MB (44871780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c1114b2e9c0ba99041080c16f9cd2cc0b58f3ba47400cbeded060ae9aa2a58`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05e3f388023fb59f887c07497c9d09720f06e7c9c0641c8650c91219d992ef`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cc3fcd99122af19a3586bbd08f963df55c278e637c28789868871e57ac52be`  
		Last Modified: Fri, 16 Jun 2023 00:39:46 GMT  
		Size: 4.6 MB (4612914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bbc8bdf52a1396cf678cea6022e4ddd772594aa67be88ee5d2526dca4f8119`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d88f83726a9409e62c9e5bdbe16cfe138ef4815a0e60012438c6df0e3170102`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c7d5d33f72689fd134bf4550db3753da17ad9ac56aa5bd15f7b9a1bb7453c`  
		Last Modified: Fri, 16 Jun 2023 00:39:52 GMT  
		Size: 58.6 MB (58602433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3175a2a660e9718faf64d43427ec34dd44af39a81c68c2a231bf10f6ae1c9`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaedeb27fa9b58368158724d925fe3ceda7fc4db137e4c56a6fb9f25a24e5d2`  
		Last Modified: Fri, 16 Jun 2023 00:39:53 GMT  
		Size: 56.6 MB (56570890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf91e7784414e9912ef38afc2c6771177cd73be84a212ba7fe23799f66e9699f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1770db1c329de5a86e8685058094ee739297578f72fbfb376991078c288c59f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1d42cf001a7bd8cb99fcc41ff98730b69094317cd3f78f9e9990c289e193da7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169420967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772571a08c67835aed7436d84973e885cc439b6cdd4dd1cc661a907d8acd3591`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 00:52:20 GMT
ADD file:1313260ee8b32fa94bcf06c44034cd7e4f9baf44c7df9e74facfe21323b37292 in / 
# Tue, 04 Jul 2023 00:52:21 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 01:28:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 01:28:04 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 01:28:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 01:28:31 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 01:29:02 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 01:29:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 01:29:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:29:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 01:29:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 01:29:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 01:29:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 01:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 01:29:41 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 01:29:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:29e800056b7e3d5007df41c0ad55416bb45d5863affcf39316c5755e71b20a30`  
		Last Modified: Tue, 04 Jul 2023 00:53:16 GMT  
		Size: 43.6 MB (43595268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69da292eb326146b0c10267953b72d6fcd767e284c36c30d51473fbcb67ca5a2`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850ef02dd581452d67b8bb9f54cd949b21fb95ff57bde8fadec5902bd385695`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 913.0 KB (913006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a76caa9e2025c7ecf56e460c12252a1216f8ac7773a0c7b289628b6c53760d`  
		Last Modified: Tue, 04 Jul 2023 01:30:07 GMT  
		Size: 4.3 MB (4298277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881324b108321b7769c7d33bb4b0d2ae626a06ae82441448e5d3c1c5e0eebf77`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5d1a8fa489bd8a99aeade310f01d71c431979332edfd44d3f2f02c7fa531fb`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efbe9eacf59876277173d2d29ad4fbe9be9678e82ea7308ef0f816b862a0653`  
		Last Modified: Tue, 04 Jul 2023 01:30:09 GMT  
		Size: 57.7 MB (57696479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80db22f26c0faf0e95ac6454baa4179c1c6481a688d8473246a212c1cfe9ee24`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5595b935c31c94590c65a3bd92f06b5f4e56874b04b4d8c351cd03327c4c7dc`  
		Last Modified: Tue, 04 Jul 2023 01:30:12 GMT  
		Size: 62.9 MB (62908250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c391d4efe15967c07ecfcbb07109613e9d801d994a094624dc6881fec27f5eb7`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 5.4 KB (5396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5527cf2eb5f0f72a2582baa44f61182d16ea054b51bff962ef6760480e17ba9`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
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
$ docker pull mysql@sha256:dd29f448c221a5ccd8d7545394772af6fe02925935e45a1c1e803ca1c08274f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:29ea1f451c3aad88df5a24288f76442286dc7fa6874d96a022e93a8a7efda880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165650520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b53e2624b431e562ed9076a9a506c5e78387f2cb4dad5968fd51ade839baa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 16 Jun 2023 00:20:42 GMT
ADD file:9f649031a04a4d0b24cc167d52bbd5ae3415fd808304c971291e35e75109822a in / 
# Fri, 16 Jun 2023 00:20:43 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:37:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 16 Jun 2023 00:37:33 GMT
ENV GOSU_VERSION=1.16
# Fri, 16 Jun 2023 00:37:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 00:38:03 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 16 Jun 2023 00:38:37 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 16 Jun 2023 00:38:38 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 16 Jun 2023 00:38:38 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:39:15 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 16 Jun 2023 00:39:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 16 Jun 2023 00:39:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 16 Jun 2023 00:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 16 Jun 2023 00:39:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 00:39:16 GMT
EXPOSE 3306 33060
# Fri, 16 Jun 2023 00:39:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:46ef68baacb785b3cf2f2826bfce791acb5264bed0fdf301623ac0c3c57f4daf`  
		Last Modified: Fri, 16 Jun 2023 00:22:14 GMT  
		Size: 44.9 MB (44871780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c1114b2e9c0ba99041080c16f9cd2cc0b58f3ba47400cbeded060ae9aa2a58`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05e3f388023fb59f887c07497c9d09720f06e7c9c0641c8650c91219d992ef`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cc3fcd99122af19a3586bbd08f963df55c278e637c28789868871e57ac52be`  
		Last Modified: Fri, 16 Jun 2023 00:39:46 GMT  
		Size: 4.6 MB (4612914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bbc8bdf52a1396cf678cea6022e4ddd772594aa67be88ee5d2526dca4f8119`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d88f83726a9409e62c9e5bdbe16cfe138ef4815a0e60012438c6df0e3170102`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c7d5d33f72689fd134bf4550db3753da17ad9ac56aa5bd15f7b9a1bb7453c`  
		Last Modified: Fri, 16 Jun 2023 00:39:52 GMT  
		Size: 58.6 MB (58602433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3175a2a660e9718faf64d43427ec34dd44af39a81c68c2a231bf10f6ae1c9`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaedeb27fa9b58368158724d925fe3ceda7fc4db137e4c56a6fb9f25a24e5d2`  
		Last Modified: Fri, 16 Jun 2023 00:39:53 GMT  
		Size: 56.6 MB (56570890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf91e7784414e9912ef38afc2c6771177cd73be84a212ba7fe23799f66e9699f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1770db1c329de5a86e8685058094ee739297578f72fbfb376991078c288c59f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1d42cf001a7bd8cb99fcc41ff98730b69094317cd3f78f9e9990c289e193da7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169420967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772571a08c67835aed7436d84973e885cc439b6cdd4dd1cc661a907d8acd3591`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 00:52:20 GMT
ADD file:1313260ee8b32fa94bcf06c44034cd7e4f9baf44c7df9e74facfe21323b37292 in / 
# Tue, 04 Jul 2023 00:52:21 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 01:28:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 01:28:04 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 01:28:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 01:28:31 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 01:29:02 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 01:29:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 01:29:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:29:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 01:29:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 01:29:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 01:29:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 01:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 01:29:41 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 01:29:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:29e800056b7e3d5007df41c0ad55416bb45d5863affcf39316c5755e71b20a30`  
		Last Modified: Tue, 04 Jul 2023 00:53:16 GMT  
		Size: 43.6 MB (43595268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69da292eb326146b0c10267953b72d6fcd767e284c36c30d51473fbcb67ca5a2`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850ef02dd581452d67b8bb9f54cd949b21fb95ff57bde8fadec5902bd385695`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 913.0 KB (913006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a76caa9e2025c7ecf56e460c12252a1216f8ac7773a0c7b289628b6c53760d`  
		Last Modified: Tue, 04 Jul 2023 01:30:07 GMT  
		Size: 4.3 MB (4298277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881324b108321b7769c7d33bb4b0d2ae626a06ae82441448e5d3c1c5e0eebf77`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5d1a8fa489bd8a99aeade310f01d71c431979332edfd44d3f2f02c7fa531fb`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efbe9eacf59876277173d2d29ad4fbe9be9678e82ea7308ef0f816b862a0653`  
		Last Modified: Tue, 04 Jul 2023 01:30:09 GMT  
		Size: 57.7 MB (57696479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80db22f26c0faf0e95ac6454baa4179c1c6481a688d8473246a212c1cfe9ee24`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5595b935c31c94590c65a3bd92f06b5f4e56874b04b4d8c351cd03327c4c7dc`  
		Last Modified: Tue, 04 Jul 2023 01:30:12 GMT  
		Size: 62.9 MB (62908250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c391d4efe15967c07ecfcbb07109613e9d801d994a094624dc6881fec27f5eb7`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 5.4 KB (5396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5527cf2eb5f0f72a2582baa44f61182d16ea054b51bff962ef6760480e17ba9`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.33`

```console
$ docker pull mysql@sha256:dd29f448c221a5ccd8d7545394772af6fe02925935e45a1c1e803ca1c08274f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.33` - linux; amd64

```console
$ docker pull mysql@sha256:29ea1f451c3aad88df5a24288f76442286dc7fa6874d96a022e93a8a7efda880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165650520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b53e2624b431e562ed9076a9a506c5e78387f2cb4dad5968fd51ade839baa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 16 Jun 2023 00:20:42 GMT
ADD file:9f649031a04a4d0b24cc167d52bbd5ae3415fd808304c971291e35e75109822a in / 
# Fri, 16 Jun 2023 00:20:43 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:37:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 16 Jun 2023 00:37:33 GMT
ENV GOSU_VERSION=1.16
# Fri, 16 Jun 2023 00:37:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 00:38:03 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 16 Jun 2023 00:38:37 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 16 Jun 2023 00:38:38 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 16 Jun 2023 00:38:38 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:39:15 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 16 Jun 2023 00:39:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 16 Jun 2023 00:39:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 16 Jun 2023 00:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 16 Jun 2023 00:39:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 00:39:16 GMT
EXPOSE 3306 33060
# Fri, 16 Jun 2023 00:39:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:46ef68baacb785b3cf2f2826bfce791acb5264bed0fdf301623ac0c3c57f4daf`  
		Last Modified: Fri, 16 Jun 2023 00:22:14 GMT  
		Size: 44.9 MB (44871780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c1114b2e9c0ba99041080c16f9cd2cc0b58f3ba47400cbeded060ae9aa2a58`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05e3f388023fb59f887c07497c9d09720f06e7c9c0641c8650c91219d992ef`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cc3fcd99122af19a3586bbd08f963df55c278e637c28789868871e57ac52be`  
		Last Modified: Fri, 16 Jun 2023 00:39:46 GMT  
		Size: 4.6 MB (4612914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bbc8bdf52a1396cf678cea6022e4ddd772594aa67be88ee5d2526dca4f8119`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d88f83726a9409e62c9e5bdbe16cfe138ef4815a0e60012438c6df0e3170102`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c7d5d33f72689fd134bf4550db3753da17ad9ac56aa5bd15f7b9a1bb7453c`  
		Last Modified: Fri, 16 Jun 2023 00:39:52 GMT  
		Size: 58.6 MB (58602433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3175a2a660e9718faf64d43427ec34dd44af39a81c68c2a231bf10f6ae1c9`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaedeb27fa9b58368158724d925fe3ceda7fc4db137e4c56a6fb9f25a24e5d2`  
		Last Modified: Fri, 16 Jun 2023 00:39:53 GMT  
		Size: 56.6 MB (56570890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf91e7784414e9912ef38afc2c6771177cd73be84a212ba7fe23799f66e9699f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1770db1c329de5a86e8685058094ee739297578f72fbfb376991078c288c59f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.33` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1d42cf001a7bd8cb99fcc41ff98730b69094317cd3f78f9e9990c289e193da7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169420967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772571a08c67835aed7436d84973e885cc439b6cdd4dd1cc661a907d8acd3591`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 00:52:20 GMT
ADD file:1313260ee8b32fa94bcf06c44034cd7e4f9baf44c7df9e74facfe21323b37292 in / 
# Tue, 04 Jul 2023 00:52:21 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 01:28:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 01:28:04 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 01:28:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 01:28:31 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 01:29:02 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 01:29:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 01:29:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:29:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 01:29:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 01:29:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 01:29:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 01:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 01:29:41 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 01:29:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:29e800056b7e3d5007df41c0ad55416bb45d5863affcf39316c5755e71b20a30`  
		Last Modified: Tue, 04 Jul 2023 00:53:16 GMT  
		Size: 43.6 MB (43595268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69da292eb326146b0c10267953b72d6fcd767e284c36c30d51473fbcb67ca5a2`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850ef02dd581452d67b8bb9f54cd949b21fb95ff57bde8fadec5902bd385695`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 913.0 KB (913006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a76caa9e2025c7ecf56e460c12252a1216f8ac7773a0c7b289628b6c53760d`  
		Last Modified: Tue, 04 Jul 2023 01:30:07 GMT  
		Size: 4.3 MB (4298277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881324b108321b7769c7d33bb4b0d2ae626a06ae82441448e5d3c1c5e0eebf77`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5d1a8fa489bd8a99aeade310f01d71c431979332edfd44d3f2f02c7fa531fb`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efbe9eacf59876277173d2d29ad4fbe9be9678e82ea7308ef0f816b862a0653`  
		Last Modified: Tue, 04 Jul 2023 01:30:09 GMT  
		Size: 57.7 MB (57696479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80db22f26c0faf0e95ac6454baa4179c1c6481a688d8473246a212c1cfe9ee24`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5595b935c31c94590c65a3bd92f06b5f4e56874b04b4d8c351cd03327c4c7dc`  
		Last Modified: Tue, 04 Jul 2023 01:30:12 GMT  
		Size: 62.9 MB (62908250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c391d4efe15967c07ecfcbb07109613e9d801d994a094624dc6881fec27f5eb7`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 5.4 KB (5396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5527cf2eb5f0f72a2582baa44f61182d16ea054b51bff962ef6760480e17ba9`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
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
$ docker pull mysql@sha256:dd29f448c221a5ccd8d7545394772af6fe02925935e45a1c1e803ca1c08274f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.33-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:29ea1f451c3aad88df5a24288f76442286dc7fa6874d96a022e93a8a7efda880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165650520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b53e2624b431e562ed9076a9a506c5e78387f2cb4dad5968fd51ade839baa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 16 Jun 2023 00:20:42 GMT
ADD file:9f649031a04a4d0b24cc167d52bbd5ae3415fd808304c971291e35e75109822a in / 
# Fri, 16 Jun 2023 00:20:43 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:37:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 16 Jun 2023 00:37:33 GMT
ENV GOSU_VERSION=1.16
# Fri, 16 Jun 2023 00:37:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 00:38:03 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 16 Jun 2023 00:38:37 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 16 Jun 2023 00:38:38 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 16 Jun 2023 00:38:38 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:39:15 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 16 Jun 2023 00:39:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 16 Jun 2023 00:39:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 16 Jun 2023 00:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 16 Jun 2023 00:39:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 00:39:16 GMT
EXPOSE 3306 33060
# Fri, 16 Jun 2023 00:39:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:46ef68baacb785b3cf2f2826bfce791acb5264bed0fdf301623ac0c3c57f4daf`  
		Last Modified: Fri, 16 Jun 2023 00:22:14 GMT  
		Size: 44.9 MB (44871780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c1114b2e9c0ba99041080c16f9cd2cc0b58f3ba47400cbeded060ae9aa2a58`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05e3f388023fb59f887c07497c9d09720f06e7c9c0641c8650c91219d992ef`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cc3fcd99122af19a3586bbd08f963df55c278e637c28789868871e57ac52be`  
		Last Modified: Fri, 16 Jun 2023 00:39:46 GMT  
		Size: 4.6 MB (4612914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bbc8bdf52a1396cf678cea6022e4ddd772594aa67be88ee5d2526dca4f8119`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d88f83726a9409e62c9e5bdbe16cfe138ef4815a0e60012438c6df0e3170102`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c7d5d33f72689fd134bf4550db3753da17ad9ac56aa5bd15f7b9a1bb7453c`  
		Last Modified: Fri, 16 Jun 2023 00:39:52 GMT  
		Size: 58.6 MB (58602433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3175a2a660e9718faf64d43427ec34dd44af39a81c68c2a231bf10f6ae1c9`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaedeb27fa9b58368158724d925fe3ceda7fc4db137e4c56a6fb9f25a24e5d2`  
		Last Modified: Fri, 16 Jun 2023 00:39:53 GMT  
		Size: 56.6 MB (56570890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf91e7784414e9912ef38afc2c6771177cd73be84a212ba7fe23799f66e9699f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1770db1c329de5a86e8685058094ee739297578f72fbfb376991078c288c59f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.33-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1d42cf001a7bd8cb99fcc41ff98730b69094317cd3f78f9e9990c289e193da7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169420967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772571a08c67835aed7436d84973e885cc439b6cdd4dd1cc661a907d8acd3591`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 00:52:20 GMT
ADD file:1313260ee8b32fa94bcf06c44034cd7e4f9baf44c7df9e74facfe21323b37292 in / 
# Tue, 04 Jul 2023 00:52:21 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 01:28:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 01:28:04 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 01:28:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 01:28:31 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 01:29:02 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 01:29:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 01:29:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:29:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 01:29:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 01:29:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 01:29:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 01:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 01:29:41 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 01:29:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:29e800056b7e3d5007df41c0ad55416bb45d5863affcf39316c5755e71b20a30`  
		Last Modified: Tue, 04 Jul 2023 00:53:16 GMT  
		Size: 43.6 MB (43595268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69da292eb326146b0c10267953b72d6fcd767e284c36c30d51473fbcb67ca5a2`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850ef02dd581452d67b8bb9f54cd949b21fb95ff57bde8fadec5902bd385695`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 913.0 KB (913006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a76caa9e2025c7ecf56e460c12252a1216f8ac7773a0c7b289628b6c53760d`  
		Last Modified: Tue, 04 Jul 2023 01:30:07 GMT  
		Size: 4.3 MB (4298277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881324b108321b7769c7d33bb4b0d2ae626a06ae82441448e5d3c1c5e0eebf77`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5d1a8fa489bd8a99aeade310f01d71c431979332edfd44d3f2f02c7fa531fb`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efbe9eacf59876277173d2d29ad4fbe9be9678e82ea7308ef0f816b862a0653`  
		Last Modified: Tue, 04 Jul 2023 01:30:09 GMT  
		Size: 57.7 MB (57696479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80db22f26c0faf0e95ac6454baa4179c1c6481a688d8473246a212c1cfe9ee24`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5595b935c31c94590c65a3bd92f06b5f4e56874b04b4d8c351cd03327c4c7dc`  
		Last Modified: Tue, 04 Jul 2023 01:30:12 GMT  
		Size: 62.9 MB (62908250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c391d4efe15967c07ecfcbb07109613e9d801d994a094624dc6881fec27f5eb7`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 5.4 KB (5396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5527cf2eb5f0f72a2582baa44f61182d16ea054b51bff962ef6760480e17ba9`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
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
$ docker pull mysql@sha256:dd29f448c221a5ccd8d7545394772af6fe02925935e45a1c1e803ca1c08274f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:29ea1f451c3aad88df5a24288f76442286dc7fa6874d96a022e93a8a7efda880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165650520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b53e2624b431e562ed9076a9a506c5e78387f2cb4dad5968fd51ade839baa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 16 Jun 2023 00:20:42 GMT
ADD file:9f649031a04a4d0b24cc167d52bbd5ae3415fd808304c971291e35e75109822a in / 
# Fri, 16 Jun 2023 00:20:43 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:37:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 16 Jun 2023 00:37:33 GMT
ENV GOSU_VERSION=1.16
# Fri, 16 Jun 2023 00:37:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 00:38:03 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 16 Jun 2023 00:38:37 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 16 Jun 2023 00:38:38 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 16 Jun 2023 00:38:38 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:39:15 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 16 Jun 2023 00:39:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 16 Jun 2023 00:39:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 16 Jun 2023 00:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 16 Jun 2023 00:39:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 00:39:16 GMT
EXPOSE 3306 33060
# Fri, 16 Jun 2023 00:39:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:46ef68baacb785b3cf2f2826bfce791acb5264bed0fdf301623ac0c3c57f4daf`  
		Last Modified: Fri, 16 Jun 2023 00:22:14 GMT  
		Size: 44.9 MB (44871780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c1114b2e9c0ba99041080c16f9cd2cc0b58f3ba47400cbeded060ae9aa2a58`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05e3f388023fb59f887c07497c9d09720f06e7c9c0641c8650c91219d992ef`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cc3fcd99122af19a3586bbd08f963df55c278e637c28789868871e57ac52be`  
		Last Modified: Fri, 16 Jun 2023 00:39:46 GMT  
		Size: 4.6 MB (4612914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bbc8bdf52a1396cf678cea6022e4ddd772594aa67be88ee5d2526dca4f8119`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d88f83726a9409e62c9e5bdbe16cfe138ef4815a0e60012438c6df0e3170102`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c7d5d33f72689fd134bf4550db3753da17ad9ac56aa5bd15f7b9a1bb7453c`  
		Last Modified: Fri, 16 Jun 2023 00:39:52 GMT  
		Size: 58.6 MB (58602433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3175a2a660e9718faf64d43427ec34dd44af39a81c68c2a231bf10f6ae1c9`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaedeb27fa9b58368158724d925fe3ceda7fc4db137e4c56a6fb9f25a24e5d2`  
		Last Modified: Fri, 16 Jun 2023 00:39:53 GMT  
		Size: 56.6 MB (56570890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf91e7784414e9912ef38afc2c6771177cd73be84a212ba7fe23799f66e9699f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1770db1c329de5a86e8685058094ee739297578f72fbfb376991078c288c59f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1d42cf001a7bd8cb99fcc41ff98730b69094317cd3f78f9e9990c289e193da7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169420967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772571a08c67835aed7436d84973e885cc439b6cdd4dd1cc661a907d8acd3591`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 00:52:20 GMT
ADD file:1313260ee8b32fa94bcf06c44034cd7e4f9baf44c7df9e74facfe21323b37292 in / 
# Tue, 04 Jul 2023 00:52:21 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 01:28:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 01:28:04 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 01:28:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 01:28:31 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 01:29:02 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 01:29:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 01:29:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:29:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 01:29:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 01:29:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 01:29:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 01:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 01:29:41 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 01:29:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:29e800056b7e3d5007df41c0ad55416bb45d5863affcf39316c5755e71b20a30`  
		Last Modified: Tue, 04 Jul 2023 00:53:16 GMT  
		Size: 43.6 MB (43595268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69da292eb326146b0c10267953b72d6fcd767e284c36c30d51473fbcb67ca5a2`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850ef02dd581452d67b8bb9f54cd949b21fb95ff57bde8fadec5902bd385695`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 913.0 KB (913006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a76caa9e2025c7ecf56e460c12252a1216f8ac7773a0c7b289628b6c53760d`  
		Last Modified: Tue, 04 Jul 2023 01:30:07 GMT  
		Size: 4.3 MB (4298277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881324b108321b7769c7d33bb4b0d2ae626a06ae82441448e5d3c1c5e0eebf77`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5d1a8fa489bd8a99aeade310f01d71c431979332edfd44d3f2f02c7fa531fb`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efbe9eacf59876277173d2d29ad4fbe9be9678e82ea7308ef0f816b862a0653`  
		Last Modified: Tue, 04 Jul 2023 01:30:09 GMT  
		Size: 57.7 MB (57696479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80db22f26c0faf0e95ac6454baa4179c1c6481a688d8473246a212c1cfe9ee24`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5595b935c31c94590c65a3bd92f06b5f4e56874b04b4d8c351cd03327c4c7dc`  
		Last Modified: Tue, 04 Jul 2023 01:30:12 GMT  
		Size: 62.9 MB (62908250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c391d4efe15967c07ecfcbb07109613e9d801d994a094624dc6881fec27f5eb7`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 5.4 KB (5396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5527cf2eb5f0f72a2582baa44f61182d16ea054b51bff962ef6760480e17ba9`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:dd29f448c221a5ccd8d7545394772af6fe02925935e45a1c1e803ca1c08274f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:29ea1f451c3aad88df5a24288f76442286dc7fa6874d96a022e93a8a7efda880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165650520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b53e2624b431e562ed9076a9a506c5e78387f2cb4dad5968fd51ade839baa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 16 Jun 2023 00:20:42 GMT
ADD file:9f649031a04a4d0b24cc167d52bbd5ae3415fd808304c971291e35e75109822a in / 
# Fri, 16 Jun 2023 00:20:43 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:37:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 16 Jun 2023 00:37:33 GMT
ENV GOSU_VERSION=1.16
# Fri, 16 Jun 2023 00:37:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 00:38:03 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 16 Jun 2023 00:38:37 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 16 Jun 2023 00:38:38 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 16 Jun 2023 00:38:38 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:39:15 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 16 Jun 2023 00:39:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 16 Jun 2023 00:39:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 16 Jun 2023 00:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 16 Jun 2023 00:39:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 00:39:16 GMT
EXPOSE 3306 33060
# Fri, 16 Jun 2023 00:39:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:46ef68baacb785b3cf2f2826bfce791acb5264bed0fdf301623ac0c3c57f4daf`  
		Last Modified: Fri, 16 Jun 2023 00:22:14 GMT  
		Size: 44.9 MB (44871780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c1114b2e9c0ba99041080c16f9cd2cc0b58f3ba47400cbeded060ae9aa2a58`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05e3f388023fb59f887c07497c9d09720f06e7c9c0641c8650c91219d992ef`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cc3fcd99122af19a3586bbd08f963df55c278e637c28789868871e57ac52be`  
		Last Modified: Fri, 16 Jun 2023 00:39:46 GMT  
		Size: 4.6 MB (4612914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bbc8bdf52a1396cf678cea6022e4ddd772594aa67be88ee5d2526dca4f8119`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d88f83726a9409e62c9e5bdbe16cfe138ef4815a0e60012438c6df0e3170102`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c7d5d33f72689fd134bf4550db3753da17ad9ac56aa5bd15f7b9a1bb7453c`  
		Last Modified: Fri, 16 Jun 2023 00:39:52 GMT  
		Size: 58.6 MB (58602433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3175a2a660e9718faf64d43427ec34dd44af39a81c68c2a231bf10f6ae1c9`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaedeb27fa9b58368158724d925fe3ceda7fc4db137e4c56a6fb9f25a24e5d2`  
		Last Modified: Fri, 16 Jun 2023 00:39:53 GMT  
		Size: 56.6 MB (56570890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf91e7784414e9912ef38afc2c6771177cd73be84a212ba7fe23799f66e9699f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1770db1c329de5a86e8685058094ee739297578f72fbfb376991078c288c59f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1d42cf001a7bd8cb99fcc41ff98730b69094317cd3f78f9e9990c289e193da7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169420967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772571a08c67835aed7436d84973e885cc439b6cdd4dd1cc661a907d8acd3591`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 00:52:20 GMT
ADD file:1313260ee8b32fa94bcf06c44034cd7e4f9baf44c7df9e74facfe21323b37292 in / 
# Tue, 04 Jul 2023 00:52:21 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 01:28:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 01:28:04 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 01:28:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 01:28:31 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 01:29:02 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 01:29:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 01:29:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:29:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 01:29:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 01:29:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 01:29:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 01:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 01:29:41 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 01:29:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:29e800056b7e3d5007df41c0ad55416bb45d5863affcf39316c5755e71b20a30`  
		Last Modified: Tue, 04 Jul 2023 00:53:16 GMT  
		Size: 43.6 MB (43595268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69da292eb326146b0c10267953b72d6fcd767e284c36c30d51473fbcb67ca5a2`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850ef02dd581452d67b8bb9f54cd949b21fb95ff57bde8fadec5902bd385695`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 913.0 KB (913006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a76caa9e2025c7ecf56e460c12252a1216f8ac7773a0c7b289628b6c53760d`  
		Last Modified: Tue, 04 Jul 2023 01:30:07 GMT  
		Size: 4.3 MB (4298277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881324b108321b7769c7d33bb4b0d2ae626a06ae82441448e5d3c1c5e0eebf77`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5d1a8fa489bd8a99aeade310f01d71c431979332edfd44d3f2f02c7fa531fb`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efbe9eacf59876277173d2d29ad4fbe9be9678e82ea7308ef0f816b862a0653`  
		Last Modified: Tue, 04 Jul 2023 01:30:09 GMT  
		Size: 57.7 MB (57696479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80db22f26c0faf0e95ac6454baa4179c1c6481a688d8473246a212c1cfe9ee24`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5595b935c31c94590c65a3bd92f06b5f4e56874b04b4d8c351cd03327c4c7dc`  
		Last Modified: Tue, 04 Jul 2023 01:30:12 GMT  
		Size: 62.9 MB (62908250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c391d4efe15967c07ecfcbb07109613e9d801d994a094624dc6881fec27f5eb7`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 5.4 KB (5396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5527cf2eb5f0f72a2582baa44f61182d16ea054b51bff962ef6760480e17ba9`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
