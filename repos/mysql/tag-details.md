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
$ docker pull mysql@sha256:6306f106a056e24b3a2582a59a4c84cd199907f826eff27df36406f227cd9a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:bd0fb5a175fc225ce9c2c4357c0f532bda1413e0b8555a157770f92daa5a89e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144279475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d410f4167eea912908b2f9bcc24eff870cb3c131dfb755088b79a4188bfeb40f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:56 GMT
ADD file:3853624d773c4bf6fc1464ca06bd07366109fab78072fcab59075073a5da6525 in / 
# Wed, 07 Dec 2022 01:51:56 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:23:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:23:50 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:23:52 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:24:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 07 Dec 2022 02:24:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Wed, 07 Dec 2022 02:24:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:24:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:24:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:24:30 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Wed, 07 Dec 2022 02:24:53 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:24:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:24:54 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:24:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:24:55 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:24:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26998a7c52d2b84e7927f97651d1d703a805c8e4d3f658a03138721f5a5dd44`  
		Last Modified: Wed, 07 Dec 2022 01:53:46 GMT  
		Size: 49.8 MB (49818482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d8a3567e30df99576e0a4dbca773af581230fee203891610e6ccbdaa823d2`  
		Last Modified: Wed, 07 Dec 2022 02:26:00 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfee1f0f349e08af59ed77c7d56ede70f0c5739daa2477ef54a4ee457f5e3e47`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ff8dfb9b12b027c35d779fe4f06a9b3d0d26efed52153324cfa2f409423b0d`  
		Last Modified: Wed, 07 Dec 2022 02:25:59 GMT  
		Size: 4.5 MB (4539026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56cbebc916d35659623816867a456610961f77db6d9753e738c5564651dfa0`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e747e5e37d77f3d8331753fc4c4eb0b0e5af8648ee5b2eec8fa274ebdddb475`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711a06e512dab8bc033e74a32300e408fc4d5ab67e6db0f84942d3ddadb7376d`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 25.5 MB (25532079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288d68e4e9e0f5e70378db2d166bf205b73ca677bdf72384be72fa529264ed1`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49271f2d6d157b6b14c6d6c165b3b29b8d29aef70edd653702832a48bcecf382`  
		Last Modified: Wed, 07 Dec 2022 02:26:08 GMT  
		Size: 63.4 MB (63449972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782f6cac69ce870188610aef114b2852e9f69f2b849a4df90c0209bf8dc1717`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701dea355691c2e0ccc548aa219fc1dd83ba44ff81843802aef25e77e813454d`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:ef71a56987ad9afad56dd4632d6c62cd27a116df6b93f8a9fc15381bb436ecc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:d6ec8e4fe681e6298a50bd59b3d8d9e9035981687f063bf0d2cbd6a8964a8625
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162597038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbd9c7db3046f9bd22e7252f5845774d6adcf9bf42ad8add99032fb9e88bcbf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 06 Dec 2022 04:44:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:44:13 GMT
ENV GOSU_VERSION=1.14
# Tue, 06 Dec 2022 04:44:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 06 Dec 2022 04:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 06 Dec 2022 04:44:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:44:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 06 Dec 2022 04:44:32 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 06 Dec 2022 04:44:32 GMT
ENV MYSQL_VERSION=5.7.40-1debian10
# Tue, 06 Dec 2022 04:44:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 06 Dec 2022 04:44:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 06 Dec 2022 04:44:52 GMT
VOLUME [/var/lib/mysql]
# Tue, 06 Dec 2022 04:44:52 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:44:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 04:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 04:44:53 GMT
EXPOSE 3306 33060
# Tue, 06 Dec 2022 04:44:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6eab20599fab240a56b06125a77b4921dd39662d3b9f9008da7306531772a1d0`  
		Last Modified: Tue, 06 Dec 2022 01:25:52 GMT  
		Size: 27.1 MB (27140356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea57fc39a1a89ab01844cc46674942409f4380e146cb8a22f4c5ad1b87e3872`  
		Last Modified: Tue, 06 Dec 2022 04:46:07 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733c3c1b8137266b1d8e75626012e324bb2946bb31d4e8248193684dc34b4b15`  
		Last Modified: Tue, 06 Dec 2022 04:46:06 GMT  
		Size: 4.2 MB (4182295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44692a06b98ce6816652f9ac3b767907642e16ecc89c6cb448403574a897aa4e`  
		Last Modified: Tue, 06 Dec 2022 04:46:06 GMT  
		Size: 1.4 MB (1388898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd4e1b5fe5fe5299c31dc8c1474c09dbe6a88acbbc8d229dcc58db4716fa0a`  
		Last Modified: Tue, 06 Dec 2022 04:46:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06983bf406f84225009fa856d42bdb362cf5617e3f179ffab8d70863f2079b04`  
		Last Modified: Tue, 06 Dec 2022 04:46:08 GMT  
		Size: 14.1 MB (14089391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4430e1554a0149ef0af8f99089ef22550a9dd065e9340a7c340935404d81cf44`  
		Last Modified: Tue, 06 Dec 2022 04:46:04 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adca83c99087831f13c752755049fb8373bea190c51e6b8e260d90929178c1f`  
		Last Modified: Tue, 06 Dec 2022 04:46:04 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dac9d65754add19e83fd832e21c7cb3e27b497fc541aa4e76bbc738e40fd53`  
		Last Modified: Tue, 06 Dec 2022 04:46:19 GMT  
		Size: 115.8 MB (115785905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bea97f97e578ce8e3025ee027de2cb9536b1f5e113a5e486775249b1c13146`  
		Last Modified: Tue, 06 Dec 2022 04:46:04 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6217a0f4a47d9dd1cfb3e55a54d7065f6166cb40be4516072b9db798c7d4bc`  
		Last Modified: Tue, 06 Dec 2022 04:46:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:6306f106a056e24b3a2582a59a4c84cd199907f826eff27df36406f227cd9a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:bd0fb5a175fc225ce9c2c4357c0f532bda1413e0b8555a157770f92daa5a89e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144279475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d410f4167eea912908b2f9bcc24eff870cb3c131dfb755088b79a4188bfeb40f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:56 GMT
ADD file:3853624d773c4bf6fc1464ca06bd07366109fab78072fcab59075073a5da6525 in / 
# Wed, 07 Dec 2022 01:51:56 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:23:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:23:50 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:23:52 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:24:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 07 Dec 2022 02:24:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Wed, 07 Dec 2022 02:24:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:24:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:24:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:24:30 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Wed, 07 Dec 2022 02:24:53 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:24:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:24:54 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:24:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:24:55 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:24:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26998a7c52d2b84e7927f97651d1d703a805c8e4d3f658a03138721f5a5dd44`  
		Last Modified: Wed, 07 Dec 2022 01:53:46 GMT  
		Size: 49.8 MB (49818482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d8a3567e30df99576e0a4dbca773af581230fee203891610e6ccbdaa823d2`  
		Last Modified: Wed, 07 Dec 2022 02:26:00 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfee1f0f349e08af59ed77c7d56ede70f0c5739daa2477ef54a4ee457f5e3e47`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ff8dfb9b12b027c35d779fe4f06a9b3d0d26efed52153324cfa2f409423b0d`  
		Last Modified: Wed, 07 Dec 2022 02:25:59 GMT  
		Size: 4.5 MB (4539026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56cbebc916d35659623816867a456610961f77db6d9753e738c5564651dfa0`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e747e5e37d77f3d8331753fc4c4eb0b0e5af8648ee5b2eec8fa274ebdddb475`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711a06e512dab8bc033e74a32300e408fc4d5ab67e6db0f84942d3ddadb7376d`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 25.5 MB (25532079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288d68e4e9e0f5e70378db2d166bf205b73ca677bdf72384be72fa529264ed1`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49271f2d6d157b6b14c6d6c165b3b29b8d29aef70edd653702832a48bcecf382`  
		Last Modified: Wed, 07 Dec 2022 02:26:08 GMT  
		Size: 63.4 MB (63449972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782f6cac69ce870188610aef114b2852e9f69f2b849a4df90c0209bf8dc1717`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701dea355691c2e0ccc548aa219fc1dd83ba44ff81843802aef25e77e813454d`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:6306f106a056e24b3a2582a59a4c84cd199907f826eff27df36406f227cd9a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:bd0fb5a175fc225ce9c2c4357c0f532bda1413e0b8555a157770f92daa5a89e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144279475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d410f4167eea912908b2f9bcc24eff870cb3c131dfb755088b79a4188bfeb40f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:56 GMT
ADD file:3853624d773c4bf6fc1464ca06bd07366109fab78072fcab59075073a5da6525 in / 
# Wed, 07 Dec 2022 01:51:56 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:23:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:23:50 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:23:52 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:24:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 07 Dec 2022 02:24:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Wed, 07 Dec 2022 02:24:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:24:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:24:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:24:30 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Wed, 07 Dec 2022 02:24:53 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:24:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:24:54 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:24:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:24:55 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:24:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26998a7c52d2b84e7927f97651d1d703a805c8e4d3f658a03138721f5a5dd44`  
		Last Modified: Wed, 07 Dec 2022 01:53:46 GMT  
		Size: 49.8 MB (49818482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d8a3567e30df99576e0a4dbca773af581230fee203891610e6ccbdaa823d2`  
		Last Modified: Wed, 07 Dec 2022 02:26:00 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfee1f0f349e08af59ed77c7d56ede70f0c5739daa2477ef54a4ee457f5e3e47`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ff8dfb9b12b027c35d779fe4f06a9b3d0d26efed52153324cfa2f409423b0d`  
		Last Modified: Wed, 07 Dec 2022 02:25:59 GMT  
		Size: 4.5 MB (4539026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56cbebc916d35659623816867a456610961f77db6d9753e738c5564651dfa0`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e747e5e37d77f3d8331753fc4c4eb0b0e5af8648ee5b2eec8fa274ebdddb475`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711a06e512dab8bc033e74a32300e408fc4d5ab67e6db0f84942d3ddadb7376d`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 25.5 MB (25532079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288d68e4e9e0f5e70378db2d166bf205b73ca677bdf72384be72fa529264ed1`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49271f2d6d157b6b14c6d6c165b3b29b8d29aef70edd653702832a48bcecf382`  
		Last Modified: Wed, 07 Dec 2022 02:26:08 GMT  
		Size: 63.4 MB (63449972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782f6cac69ce870188610aef114b2852e9f69f2b849a4df90c0209bf8dc1717`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701dea355691c2e0ccc548aa219fc1dd83ba44ff81843802aef25e77e813454d`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:ef71a56987ad9afad56dd4632d6c62cd27a116df6b93f8a9fc15381bb436ecc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:d6ec8e4fe681e6298a50bd59b3d8d9e9035981687f063bf0d2cbd6a8964a8625
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162597038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbd9c7db3046f9bd22e7252f5845774d6adcf9bf42ad8add99032fb9e88bcbf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 06 Dec 2022 04:44:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:44:13 GMT
ENV GOSU_VERSION=1.14
# Tue, 06 Dec 2022 04:44:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 06 Dec 2022 04:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 06 Dec 2022 04:44:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:44:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 06 Dec 2022 04:44:32 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 06 Dec 2022 04:44:32 GMT
ENV MYSQL_VERSION=5.7.40-1debian10
# Tue, 06 Dec 2022 04:44:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 06 Dec 2022 04:44:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 06 Dec 2022 04:44:52 GMT
VOLUME [/var/lib/mysql]
# Tue, 06 Dec 2022 04:44:52 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:44:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 04:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 04:44:53 GMT
EXPOSE 3306 33060
# Tue, 06 Dec 2022 04:44:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6eab20599fab240a56b06125a77b4921dd39662d3b9f9008da7306531772a1d0`  
		Last Modified: Tue, 06 Dec 2022 01:25:52 GMT  
		Size: 27.1 MB (27140356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea57fc39a1a89ab01844cc46674942409f4380e146cb8a22f4c5ad1b87e3872`  
		Last Modified: Tue, 06 Dec 2022 04:46:07 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733c3c1b8137266b1d8e75626012e324bb2946bb31d4e8248193684dc34b4b15`  
		Last Modified: Tue, 06 Dec 2022 04:46:06 GMT  
		Size: 4.2 MB (4182295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44692a06b98ce6816652f9ac3b767907642e16ecc89c6cb448403574a897aa4e`  
		Last Modified: Tue, 06 Dec 2022 04:46:06 GMT  
		Size: 1.4 MB (1388898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd4e1b5fe5fe5299c31dc8c1474c09dbe6a88acbbc8d229dcc58db4716fa0a`  
		Last Modified: Tue, 06 Dec 2022 04:46:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06983bf406f84225009fa856d42bdb362cf5617e3f179ffab8d70863f2079b04`  
		Last Modified: Tue, 06 Dec 2022 04:46:08 GMT  
		Size: 14.1 MB (14089391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4430e1554a0149ef0af8f99089ef22550a9dd065e9340a7c340935404d81cf44`  
		Last Modified: Tue, 06 Dec 2022 04:46:04 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adca83c99087831f13c752755049fb8373bea190c51e6b8e260d90929178c1f`  
		Last Modified: Tue, 06 Dec 2022 04:46:04 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dac9d65754add19e83fd832e21c7cb3e27b497fc541aa4e76bbc738e40fd53`  
		Last Modified: Tue, 06 Dec 2022 04:46:19 GMT  
		Size: 115.8 MB (115785905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bea97f97e578ce8e3025ee027de2cb9536b1f5e113a5e486775249b1c13146`  
		Last Modified: Tue, 06 Dec 2022 04:46:04 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6217a0f4a47d9dd1cfb3e55a54d7065f6166cb40be4516072b9db798c7d4bc`  
		Last Modified: Tue, 06 Dec 2022 04:46:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:6306f106a056e24b3a2582a59a4c84cd199907f826eff27df36406f227cd9a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:bd0fb5a175fc225ce9c2c4357c0f532bda1413e0b8555a157770f92daa5a89e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144279475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d410f4167eea912908b2f9bcc24eff870cb3c131dfb755088b79a4188bfeb40f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:56 GMT
ADD file:3853624d773c4bf6fc1464ca06bd07366109fab78072fcab59075073a5da6525 in / 
# Wed, 07 Dec 2022 01:51:56 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:23:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:23:50 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:23:52 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:24:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 07 Dec 2022 02:24:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Wed, 07 Dec 2022 02:24:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:24:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:24:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:24:30 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Wed, 07 Dec 2022 02:24:53 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:24:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:24:54 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:24:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:24:55 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:24:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26998a7c52d2b84e7927f97651d1d703a805c8e4d3f658a03138721f5a5dd44`  
		Last Modified: Wed, 07 Dec 2022 01:53:46 GMT  
		Size: 49.8 MB (49818482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d8a3567e30df99576e0a4dbca773af581230fee203891610e6ccbdaa823d2`  
		Last Modified: Wed, 07 Dec 2022 02:26:00 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfee1f0f349e08af59ed77c7d56ede70f0c5739daa2477ef54a4ee457f5e3e47`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ff8dfb9b12b027c35d779fe4f06a9b3d0d26efed52153324cfa2f409423b0d`  
		Last Modified: Wed, 07 Dec 2022 02:25:59 GMT  
		Size: 4.5 MB (4539026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56cbebc916d35659623816867a456610961f77db6d9753e738c5564651dfa0`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e747e5e37d77f3d8331753fc4c4eb0b0e5af8648ee5b2eec8fa274ebdddb475`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711a06e512dab8bc033e74a32300e408fc4d5ab67e6db0f84942d3ddadb7376d`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 25.5 MB (25532079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288d68e4e9e0f5e70378db2d166bf205b73ca677bdf72384be72fa529264ed1`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49271f2d6d157b6b14c6d6c165b3b29b8d29aef70edd653702832a48bcecf382`  
		Last Modified: Wed, 07 Dec 2022 02:26:08 GMT  
		Size: 63.4 MB (63449972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782f6cac69ce870188610aef114b2852e9f69f2b849a4df90c0209bf8dc1717`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701dea355691c2e0ccc548aa219fc1dd83ba44ff81843802aef25e77e813454d`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40`

```console
$ docker pull mysql@sha256:6306f106a056e24b3a2582a59a4c84cd199907f826eff27df36406f227cd9a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40` - linux; amd64

```console
$ docker pull mysql@sha256:bd0fb5a175fc225ce9c2c4357c0f532bda1413e0b8555a157770f92daa5a89e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144279475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d410f4167eea912908b2f9bcc24eff870cb3c131dfb755088b79a4188bfeb40f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:56 GMT
ADD file:3853624d773c4bf6fc1464ca06bd07366109fab78072fcab59075073a5da6525 in / 
# Wed, 07 Dec 2022 01:51:56 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:23:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:23:50 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:23:52 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:24:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 07 Dec 2022 02:24:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Wed, 07 Dec 2022 02:24:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:24:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:24:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:24:30 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Wed, 07 Dec 2022 02:24:53 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:24:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:24:54 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:24:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:24:55 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:24:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26998a7c52d2b84e7927f97651d1d703a805c8e4d3f658a03138721f5a5dd44`  
		Last Modified: Wed, 07 Dec 2022 01:53:46 GMT  
		Size: 49.8 MB (49818482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d8a3567e30df99576e0a4dbca773af581230fee203891610e6ccbdaa823d2`  
		Last Modified: Wed, 07 Dec 2022 02:26:00 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfee1f0f349e08af59ed77c7d56ede70f0c5739daa2477ef54a4ee457f5e3e47`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ff8dfb9b12b027c35d779fe4f06a9b3d0d26efed52153324cfa2f409423b0d`  
		Last Modified: Wed, 07 Dec 2022 02:25:59 GMT  
		Size: 4.5 MB (4539026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56cbebc916d35659623816867a456610961f77db6d9753e738c5564651dfa0`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e747e5e37d77f3d8331753fc4c4eb0b0e5af8648ee5b2eec8fa274ebdddb475`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711a06e512dab8bc033e74a32300e408fc4d5ab67e6db0f84942d3ddadb7376d`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 25.5 MB (25532079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288d68e4e9e0f5e70378db2d166bf205b73ca677bdf72384be72fa529264ed1`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49271f2d6d157b6b14c6d6c165b3b29b8d29aef70edd653702832a48bcecf382`  
		Last Modified: Wed, 07 Dec 2022 02:26:08 GMT  
		Size: 63.4 MB (63449972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782f6cac69ce870188610aef114b2852e9f69f2b849a4df90c0209bf8dc1717`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701dea355691c2e0ccc548aa219fc1dd83ba44ff81843802aef25e77e813454d`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40-debian`

```console
$ docker pull mysql@sha256:ef71a56987ad9afad56dd4632d6c62cd27a116df6b93f8a9fc15381bb436ecc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40-debian` - linux; amd64

```console
$ docker pull mysql@sha256:d6ec8e4fe681e6298a50bd59b3d8d9e9035981687f063bf0d2cbd6a8964a8625
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162597038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fbd9c7db3046f9bd22e7252f5845774d6adcf9bf42ad8add99032fb9e88bcbf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 06 Dec 2022 04:44:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:44:13 GMT
ENV GOSU_VERSION=1.14
# Tue, 06 Dec 2022 04:44:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 06 Dec 2022 04:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 06 Dec 2022 04:44:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:44:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 06 Dec 2022 04:44:32 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 06 Dec 2022 04:44:32 GMT
ENV MYSQL_VERSION=5.7.40-1debian10
# Tue, 06 Dec 2022 04:44:32 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 06 Dec 2022 04:44:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 06 Dec 2022 04:44:52 GMT
VOLUME [/var/lib/mysql]
# Tue, 06 Dec 2022 04:44:52 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:44:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 04:44:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 04:44:53 GMT
EXPOSE 3306 33060
# Tue, 06 Dec 2022 04:44:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6eab20599fab240a56b06125a77b4921dd39662d3b9f9008da7306531772a1d0`  
		Last Modified: Tue, 06 Dec 2022 01:25:52 GMT  
		Size: 27.1 MB (27140356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea57fc39a1a89ab01844cc46674942409f4380e146cb8a22f4c5ad1b87e3872`  
		Last Modified: Tue, 06 Dec 2022 04:46:07 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733c3c1b8137266b1d8e75626012e324bb2946bb31d4e8248193684dc34b4b15`  
		Last Modified: Tue, 06 Dec 2022 04:46:06 GMT  
		Size: 4.2 MB (4182295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44692a06b98ce6816652f9ac3b767907642e16ecc89c6cb448403574a897aa4e`  
		Last Modified: Tue, 06 Dec 2022 04:46:06 GMT  
		Size: 1.4 MB (1388898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd4e1b5fe5fe5299c31dc8c1474c09dbe6a88acbbc8d229dcc58db4716fa0a`  
		Last Modified: Tue, 06 Dec 2022 04:46:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06983bf406f84225009fa856d42bdb362cf5617e3f179ffab8d70863f2079b04`  
		Last Modified: Tue, 06 Dec 2022 04:46:08 GMT  
		Size: 14.1 MB (14089391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4430e1554a0149ef0af8f99089ef22550a9dd065e9340a7c340935404d81cf44`  
		Last Modified: Tue, 06 Dec 2022 04:46:04 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adca83c99087831f13c752755049fb8373bea190c51e6b8e260d90929178c1f`  
		Last Modified: Tue, 06 Dec 2022 04:46:04 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dac9d65754add19e83fd832e21c7cb3e27b497fc541aa4e76bbc738e40fd53`  
		Last Modified: Tue, 06 Dec 2022 04:46:19 GMT  
		Size: 115.8 MB (115785905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bea97f97e578ce8e3025ee027de2cb9536b1f5e113a5e486775249b1c13146`  
		Last Modified: Tue, 06 Dec 2022 04:46:04 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6217a0f4a47d9dd1cfb3e55a54d7065f6166cb40be4516072b9db798c7d4bc`  
		Last Modified: Tue, 06 Dec 2022 04:46:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40-oracle`

```console
$ docker pull mysql@sha256:6306f106a056e24b3a2582a59a4c84cd199907f826eff27df36406f227cd9a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:bd0fb5a175fc225ce9c2c4357c0f532bda1413e0b8555a157770f92daa5a89e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144279475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d410f4167eea912908b2f9bcc24eff870cb3c131dfb755088b79a4188bfeb40f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:56 GMT
ADD file:3853624d773c4bf6fc1464ca06bd07366109fab78072fcab59075073a5da6525 in / 
# Wed, 07 Dec 2022 01:51:56 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:23:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:23:50 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:23:52 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:24:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 07 Dec 2022 02:24:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Wed, 07 Dec 2022 02:24:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:24:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:24:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:24:30 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Wed, 07 Dec 2022 02:24:53 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:24:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:24:54 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:24:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:24:55 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:24:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26998a7c52d2b84e7927f97651d1d703a805c8e4d3f658a03138721f5a5dd44`  
		Last Modified: Wed, 07 Dec 2022 01:53:46 GMT  
		Size: 49.8 MB (49818482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d8a3567e30df99576e0a4dbca773af581230fee203891610e6ccbdaa823d2`  
		Last Modified: Wed, 07 Dec 2022 02:26:00 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfee1f0f349e08af59ed77c7d56ede70f0c5739daa2477ef54a4ee457f5e3e47`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ff8dfb9b12b027c35d779fe4f06a9b3d0d26efed52153324cfa2f409423b0d`  
		Last Modified: Wed, 07 Dec 2022 02:25:59 GMT  
		Size: 4.5 MB (4539026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56cbebc916d35659623816867a456610961f77db6d9753e738c5564651dfa0`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e747e5e37d77f3d8331753fc4c4eb0b0e5af8648ee5b2eec8fa274ebdddb475`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711a06e512dab8bc033e74a32300e408fc4d5ab67e6db0f84942d3ddadb7376d`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 25.5 MB (25532079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288d68e4e9e0f5e70378db2d166bf205b73ca677bdf72384be72fa529264ed1`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49271f2d6d157b6b14c6d6c165b3b29b8d29aef70edd653702832a48bcecf382`  
		Last Modified: Wed, 07 Dec 2022 02:26:08 GMT  
		Size: 63.4 MB (63449972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782f6cac69ce870188610aef114b2852e9f69f2b849a4df90c0209bf8dc1717`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701dea355691c2e0ccc548aa219fc1dd83ba44ff81843802aef25e77e813454d`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:d4f67ded44fb6b55965f589d265009cb3069ddd332d77446bcd5d52db78d5394
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:1628361373b1fb29bdfedabddb5e5af829daea710c3df004f4ce84579adf1954
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177567069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c0ef1d0be535fbfd666a69b560596c725caf7f29e26bb5bf0d980370bc2a983`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:43:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 06 Dec 2022 04:43:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:43:22 GMT
ENV GOSU_VERSION=1.14
# Tue, 06 Dec 2022 04:43:31 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 06 Dec 2022 04:43:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 06 Dec 2022 04:43:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:43:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 06 Dec 2022 04:43:38 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 06 Dec 2022 04:43:38 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Tue, 06 Dec 2022 04:43:39 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 06 Dec 2022 04:43:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 06 Dec 2022 04:43:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 06 Dec 2022 04:43:56 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 06 Dec 2022 04:43:56 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:43:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 04:43:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 04:43:57 GMT
EXPOSE 3306 33060
# Tue, 06 Dec 2022 04:43:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f557800178ef7bec7396d4ab1625f0cd1bc22601706c41716ad41fd6ed7997`  
		Last Modified: Tue, 06 Dec 2022 04:45:31 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7c763cf1f3faeb13290eab77b6c732fb470241c3f08ae15aa2afb2ce4b9f08`  
		Last Modified: Tue, 06 Dec 2022 04:45:32 GMT  
		Size: 4.4 MB (4415501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6573edc9d11c3b9ba9b7e36d71a9f4f3476e2fcab4df04c46141d423010c0a9`  
		Last Modified: Tue, 06 Dec 2022 04:45:30 GMT  
		Size: 1.4 MB (1419524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fa379afc883c76128c375a3775cccc6ff43b65024f8030c50f81497f9744a2`  
		Last Modified: Tue, 06 Dec 2022 04:45:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7dc5e954004a23948497385b01f41ca9ebc8a87d1c8e7dfed71908b0b02e8e`  
		Last Modified: Tue, 06 Dec 2022 04:45:32 GMT  
		Size: 12.7 MB (12662783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175608a80561089726550674683fb7e3ffb2a973aa073b8d5112c016c99d16f4`  
		Last Modified: Tue, 06 Dec 2022 04:45:29 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c1c50fc1c65d0022b93a5f2b349b2252b35fd4ea2216837ca09882e90911f3`  
		Last Modified: Tue, 06 Dec 2022 04:45:27 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7994408f08442812e6ec85316ce37ddb00ace1cbc75c2bb67e1389506742eac`  
		Last Modified: Tue, 06 Dec 2022 04:45:47 GMT  
		Size: 127.6 MB (127645374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9037ec04597974c12673f8ad3ef29e29b9d18efbc199dba45c867c1785a111b`  
		Last Modified: Tue, 06 Dec 2022 04:45:27 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f623bf92911bcd1dcefebf323e6557fbaec875298ca5e7a1996eed6b1730c37c`  
		Last Modified: Tue, 06 Dec 2022 04:45:28 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f752a92ec102003df70542567485b80303c188d8320ed466c49ae0250be4ea`  
		Last Modified: Tue, 06 Dec 2022 04:45:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:d4f67ded44fb6b55965f589d265009cb3069ddd332d77446bcd5d52db78d5394
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:1628361373b1fb29bdfedabddb5e5af829daea710c3df004f4ce84579adf1954
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177567069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c0ef1d0be535fbfd666a69b560596c725caf7f29e26bb5bf0d980370bc2a983`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:43:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 06 Dec 2022 04:43:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:43:22 GMT
ENV GOSU_VERSION=1.14
# Tue, 06 Dec 2022 04:43:31 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 06 Dec 2022 04:43:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 06 Dec 2022 04:43:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:43:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 06 Dec 2022 04:43:38 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 06 Dec 2022 04:43:38 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Tue, 06 Dec 2022 04:43:39 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 06 Dec 2022 04:43:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 06 Dec 2022 04:43:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 06 Dec 2022 04:43:56 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 06 Dec 2022 04:43:56 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:43:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 04:43:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 04:43:57 GMT
EXPOSE 3306 33060
# Tue, 06 Dec 2022 04:43:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f557800178ef7bec7396d4ab1625f0cd1bc22601706c41716ad41fd6ed7997`  
		Last Modified: Tue, 06 Dec 2022 04:45:31 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7c763cf1f3faeb13290eab77b6c732fb470241c3f08ae15aa2afb2ce4b9f08`  
		Last Modified: Tue, 06 Dec 2022 04:45:32 GMT  
		Size: 4.4 MB (4415501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6573edc9d11c3b9ba9b7e36d71a9f4f3476e2fcab4df04c46141d423010c0a9`  
		Last Modified: Tue, 06 Dec 2022 04:45:30 GMT  
		Size: 1.4 MB (1419524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fa379afc883c76128c375a3775cccc6ff43b65024f8030c50f81497f9744a2`  
		Last Modified: Tue, 06 Dec 2022 04:45:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7dc5e954004a23948497385b01f41ca9ebc8a87d1c8e7dfed71908b0b02e8e`  
		Last Modified: Tue, 06 Dec 2022 04:45:32 GMT  
		Size: 12.7 MB (12662783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175608a80561089726550674683fb7e3ffb2a973aa073b8d5112c016c99d16f4`  
		Last Modified: Tue, 06 Dec 2022 04:45:29 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c1c50fc1c65d0022b93a5f2b349b2252b35fd4ea2216837ca09882e90911f3`  
		Last Modified: Tue, 06 Dec 2022 04:45:27 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7994408f08442812e6ec85316ce37ddb00ace1cbc75c2bb67e1389506742eac`  
		Last Modified: Tue, 06 Dec 2022 04:45:47 GMT  
		Size: 127.6 MB (127645374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9037ec04597974c12673f8ad3ef29e29b9d18efbc199dba45c867c1785a111b`  
		Last Modified: Tue, 06 Dec 2022 04:45:27 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f623bf92911bcd1dcefebf323e6557fbaec875298ca5e7a1996eed6b1730c37c`  
		Last Modified: Tue, 06 Dec 2022 04:45:28 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f752a92ec102003df70542567485b80303c188d8320ed466c49ae0250be4ea`  
		Last Modified: Tue, 06 Dec 2022 04:45:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.31` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.31` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31-debian`

```console
$ docker pull mysql@sha256:d4f67ded44fb6b55965f589d265009cb3069ddd332d77446bcd5d52db78d5394
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.31-debian` - linux; amd64

```console
$ docker pull mysql@sha256:1628361373b1fb29bdfedabddb5e5af829daea710c3df004f4ce84579adf1954
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177567069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c0ef1d0be535fbfd666a69b560596c725caf7f29e26bb5bf0d980370bc2a983`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:43:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 06 Dec 2022 04:43:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:43:22 GMT
ENV GOSU_VERSION=1.14
# Tue, 06 Dec 2022 04:43:31 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 06 Dec 2022 04:43:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 06 Dec 2022 04:43:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:43:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 06 Dec 2022 04:43:38 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 06 Dec 2022 04:43:38 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Tue, 06 Dec 2022 04:43:39 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 06 Dec 2022 04:43:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 06 Dec 2022 04:43:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 06 Dec 2022 04:43:56 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 06 Dec 2022 04:43:56 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:43:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 04:43:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 04:43:57 GMT
EXPOSE 3306 33060
# Tue, 06 Dec 2022 04:43:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f557800178ef7bec7396d4ab1625f0cd1bc22601706c41716ad41fd6ed7997`  
		Last Modified: Tue, 06 Dec 2022 04:45:31 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7c763cf1f3faeb13290eab77b6c732fb470241c3f08ae15aa2afb2ce4b9f08`  
		Last Modified: Tue, 06 Dec 2022 04:45:32 GMT  
		Size: 4.4 MB (4415501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6573edc9d11c3b9ba9b7e36d71a9f4f3476e2fcab4df04c46141d423010c0a9`  
		Last Modified: Tue, 06 Dec 2022 04:45:30 GMT  
		Size: 1.4 MB (1419524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fa379afc883c76128c375a3775cccc6ff43b65024f8030c50f81497f9744a2`  
		Last Modified: Tue, 06 Dec 2022 04:45:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7dc5e954004a23948497385b01f41ca9ebc8a87d1c8e7dfed71908b0b02e8e`  
		Last Modified: Tue, 06 Dec 2022 04:45:32 GMT  
		Size: 12.7 MB (12662783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175608a80561089726550674683fb7e3ffb2a973aa073b8d5112c016c99d16f4`  
		Last Modified: Tue, 06 Dec 2022 04:45:29 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c1c50fc1c65d0022b93a5f2b349b2252b35fd4ea2216837ca09882e90911f3`  
		Last Modified: Tue, 06 Dec 2022 04:45:27 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7994408f08442812e6ec85316ce37ddb00ace1cbc75c2bb67e1389506742eac`  
		Last Modified: Tue, 06 Dec 2022 04:45:47 GMT  
		Size: 127.6 MB (127645374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9037ec04597974c12673f8ad3ef29e29b9d18efbc199dba45c867c1785a111b`  
		Last Modified: Tue, 06 Dec 2022 04:45:27 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f623bf92911bcd1dcefebf323e6557fbaec875298ca5e7a1996eed6b1730c37c`  
		Last Modified: Tue, 06 Dec 2022 04:45:28 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f752a92ec102003df70542567485b80303c188d8320ed466c49ae0250be4ea`  
		Last Modified: Tue, 06 Dec 2022 04:45:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31-oracle`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.31-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.31-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:d4f67ded44fb6b55965f589d265009cb3069ddd332d77446bcd5d52db78d5394
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:1628361373b1fb29bdfedabddb5e5af829daea710c3df004f4ce84579adf1954
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177567069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c0ef1d0be535fbfd666a69b560596c725caf7f29e26bb5bf0d980370bc2a983`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:43:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 06 Dec 2022 04:43:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:43:22 GMT
ENV GOSU_VERSION=1.14
# Tue, 06 Dec 2022 04:43:31 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 06 Dec 2022 04:43:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 06 Dec 2022 04:43:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:43:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 06 Dec 2022 04:43:38 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 06 Dec 2022 04:43:38 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Tue, 06 Dec 2022 04:43:39 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 06 Dec 2022 04:43:55 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 06 Dec 2022 04:43:56 GMT
VOLUME [/var/lib/mysql]
# Tue, 06 Dec 2022 04:43:56 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 06 Dec 2022 04:43:56 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:43:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 04:43:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 04:43:57 GMT
EXPOSE 3306 33060
# Tue, 06 Dec 2022 04:43:57 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f557800178ef7bec7396d4ab1625f0cd1bc22601706c41716ad41fd6ed7997`  
		Last Modified: Tue, 06 Dec 2022 04:45:31 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7c763cf1f3faeb13290eab77b6c732fb470241c3f08ae15aa2afb2ce4b9f08`  
		Last Modified: Tue, 06 Dec 2022 04:45:32 GMT  
		Size: 4.4 MB (4415501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6573edc9d11c3b9ba9b7e36d71a9f4f3476e2fcab4df04c46141d423010c0a9`  
		Last Modified: Tue, 06 Dec 2022 04:45:30 GMT  
		Size: 1.4 MB (1419524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fa379afc883c76128c375a3775cccc6ff43b65024f8030c50f81497f9744a2`  
		Last Modified: Tue, 06 Dec 2022 04:45:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7dc5e954004a23948497385b01f41ca9ebc8a87d1c8e7dfed71908b0b02e8e`  
		Last Modified: Tue, 06 Dec 2022 04:45:32 GMT  
		Size: 12.7 MB (12662783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175608a80561089726550674683fb7e3ffb2a973aa073b8d5112c016c99d16f4`  
		Last Modified: Tue, 06 Dec 2022 04:45:29 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c1c50fc1c65d0022b93a5f2b349b2252b35fd4ea2216837ca09882e90911f3`  
		Last Modified: Tue, 06 Dec 2022 04:45:27 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7994408f08442812e6ec85316ce37ddb00ace1cbc75c2bb67e1389506742eac`  
		Last Modified: Tue, 06 Dec 2022 04:45:47 GMT  
		Size: 127.6 MB (127645374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9037ec04597974c12673f8ad3ef29e29b9d18efbc199dba45c867c1785a111b`  
		Last Modified: Tue, 06 Dec 2022 04:45:27 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f623bf92911bcd1dcefebf323e6557fbaec875298ca5e7a1996eed6b1730c37c`  
		Last Modified: Tue, 06 Dec 2022 04:45:28 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f752a92ec102003df70542567485b80303c188d8320ed466c49ae0250be4ea`  
		Last Modified: Tue, 06 Dec 2022 04:45:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
