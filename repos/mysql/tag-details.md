<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5-debian`](#mysql5-debian)
-	[`mysql:5-oracle`](#mysql5-oracle)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7-debian`](#mysql57-debian)
-	[`mysql:5.7-oracle`](#mysql57-oracle)
-	[`mysql:5.7.37`](#mysql5737)
-	[`mysql:5.7.37-debian`](#mysql5737-debian)
-	[`mysql:5.7.37-oracle`](#mysql5737-oracle)
-	[`mysql:8`](#mysql8)
-	[`mysql:8-debian`](#mysql8-debian)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0.28`](#mysql8028)
-	[`mysql:8.0.28-debian`](#mysql8028-debian)
-	[`mysql:8.0.28-oracle`](#mysql8028-oracle)
-	[`mysql:debian`](#mysqldebian)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)

## `mysql:5`

```console
$ docker pull mysql@sha256:ea24ddf1116d6e5053919748d2c27c8200e39ac0dbe9540f213a2d9141b66167
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:5adbbb05d43e67a7ed5f4856d3831b22ece5178d23c565b31cef61f92e3467ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154804997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538ec2c8721c073370299bf83ae46b940c83899f44cc90d89799a046afc5816b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Wed, 23 Feb 2022 22:27:55 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:28:14 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:28:15 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:28:15 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:28:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:28:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:28:16 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:28:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45b9a309e746ae5e6074efb8d35490146b3188f1375fd6abe60763a4b13b79`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90242da46c5709e3df233b61e042de5002a59567de7c18a68c75935d386195d9`  
		Last Modified: Wed, 23 Feb 2022 22:30:30 GMT  
		Size: 108.6 MB (108636729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d822d1293bf6661e4e6c69c425a5e9fca7b43bbf1201c1c66effbebd275d4`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 5.0 KB (4954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1704bf9fa7759625eeda74bcf484357dd06e4ef8d46319f09b59d4fd4c154eab`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:ea24ddf1116d6e5053919748d2c27c8200e39ac0dbe9540f213a2d9141b66167
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:5adbbb05d43e67a7ed5f4856d3831b22ece5178d23c565b31cef61f92e3467ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154804997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538ec2c8721c073370299bf83ae46b940c83899f44cc90d89799a046afc5816b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Wed, 23 Feb 2022 22:27:55 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:28:14 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:28:15 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:28:15 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:28:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:28:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:28:16 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:28:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45b9a309e746ae5e6074efb8d35490146b3188f1375fd6abe60763a4b13b79`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90242da46c5709e3df233b61e042de5002a59567de7c18a68c75935d386195d9`  
		Last Modified: Wed, 23 Feb 2022 22:30:30 GMT  
		Size: 108.6 MB (108636729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d822d1293bf6661e4e6c69c425a5e9fca7b43bbf1201c1c66effbebd275d4`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 5.0 KB (4954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1704bf9fa7759625eeda74bcf484357dd06e4ef8d46319f09b59d4fd4c154eab`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:898fe77fb3df7a9aff1d4e48eede7a7346998bd95f897ec27f0b484c5eb3c7bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:76435a59768a5de70e77a98036eb59806557c6afd16a473fb421022a30d791a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123656656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:250ac1974470ba054ae919a1731e92dab69ada7fc78f9c7bcd2a42c67dd5b56a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Jan 2022 22:34:30 GMT
ADD file:18acb1f3ef1ffe1aeaff1aa22861026180d22104f6f14dd8bc4656777800fd9f in / 
# Wed, 12 Jan 2022 22:34:30 GMT
CMD ["/bin/bash"]
# Fri, 18 Feb 2022 01:23:36 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 18 Feb 2022 01:23:36 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Feb 2022 01:23:40 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Feb 2022 22:26:27 GMT
RUN set -eux; 	yum install -y 		gzip 		xz 	; 	yum clean all
# Wed, 23 Feb 2022 22:27:06 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:27:07 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 23 Feb 2022 22:27:07 GMT
ENV MYSQL_VERSION=5.7.37-1.el7
# Wed, 23 Feb 2022 22:27:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 23 Feb 2022 22:27:27 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 23 Feb 2022 22:27:28 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 23 Feb 2022 22:27:28 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el7
# Wed, 23 Feb 2022 22:27:46 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 23 Feb 2022 22:27:46 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:27:47 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:27:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:27:47 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:27:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1e1d49338f200e5dab7ef55f9d3a37259af48812603e07ae59e43615f9038b27`  
		Last Modified: Wed, 12 Jan 2022 22:35:18 GMT  
		Size: 48.3 MB (48330956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66218a3b537b220bfcc60a7592e8334f387d5189667b2364be8266fdf038a03f`  
		Last Modified: Fri, 18 Feb 2022 01:26:48 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e2fa6d94c92997a80329028540d0f0e421e44aa0d58069d03944a79c152089`  
		Last Modified: Fri, 18 Feb 2022 01:26:48 GMT  
		Size: 930.2 KB (930228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6800d2a84cbc0ba3c39d909b1631f8c89a5a82c9b63c3173a31b013910a64a`  
		Last Modified: Wed, 23 Feb 2022 22:29:56 GMT  
		Size: 2.7 MB (2667220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665a131c9d2e9f51044d6b456f6227d3bc51f50eb33ecf44ae8acee1ee70d25d`  
		Last Modified: Wed, 23 Feb 2022 22:29:55 GMT  
		Size: 2.7 KB (2666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc57f84c66d58cef52bb795f8686a4b762dd6d61af0f5fac16a1ec7df93546da`  
		Last Modified: Wed, 23 Feb 2022 22:29:53 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27f40f7b5b424896da7dd2f9b1faff3c2360119811ce0c77cd5f753d17e1c35`  
		Last Modified: Wed, 23 Feb 2022 22:29:57 GMT  
		Size: 25.4 MB (25401979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc3e6d094d9b21f9e3636bb95d3dc8387a1a8b2f5c284420cf97c7898b07270`  
		Last Modified: Wed, 23 Feb 2022 22:29:53 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468635081a56d4d4c9d48a88541026ee0cfc22513a1b53ac29da0f306c5229c0`  
		Last Modified: Wed, 23 Feb 2022 22:30:02 GMT  
		Size: 46.3 MB (46316937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96812f7d9d74f531f52dc68d110c830f4e4fad982a1c082ec775b380999b2bc`  
		Last Modified: Wed, 23 Feb 2022 22:29:53 GMT  
		Size: 5.0 KB (4953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:ea24ddf1116d6e5053919748d2c27c8200e39ac0dbe9540f213a2d9141b66167
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:5adbbb05d43e67a7ed5f4856d3831b22ece5178d23c565b31cef61f92e3467ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154804997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538ec2c8721c073370299bf83ae46b940c83899f44cc90d89799a046afc5816b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Wed, 23 Feb 2022 22:27:55 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:28:14 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:28:15 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:28:15 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:28:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:28:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:28:16 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:28:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45b9a309e746ae5e6074efb8d35490146b3188f1375fd6abe60763a4b13b79`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90242da46c5709e3df233b61e042de5002a59567de7c18a68c75935d386195d9`  
		Last Modified: Wed, 23 Feb 2022 22:30:30 GMT  
		Size: 108.6 MB (108636729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d822d1293bf6661e4e6c69c425a5e9fca7b43bbf1201c1c66effbebd275d4`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 5.0 KB (4954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1704bf9fa7759625eeda74bcf484357dd06e4ef8d46319f09b59d4fd4c154eab`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:ea24ddf1116d6e5053919748d2c27c8200e39ac0dbe9540f213a2d9141b66167
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:5adbbb05d43e67a7ed5f4856d3831b22ece5178d23c565b31cef61f92e3467ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154804997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538ec2c8721c073370299bf83ae46b940c83899f44cc90d89799a046afc5816b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Wed, 23 Feb 2022 22:27:55 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:28:14 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:28:15 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:28:15 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:28:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:28:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:28:16 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:28:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45b9a309e746ae5e6074efb8d35490146b3188f1375fd6abe60763a4b13b79`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90242da46c5709e3df233b61e042de5002a59567de7c18a68c75935d386195d9`  
		Last Modified: Wed, 23 Feb 2022 22:30:30 GMT  
		Size: 108.6 MB (108636729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d822d1293bf6661e4e6c69c425a5e9fca7b43bbf1201c1c66effbebd275d4`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 5.0 KB (4954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1704bf9fa7759625eeda74bcf484357dd06e4ef8d46319f09b59d4fd4c154eab`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:898fe77fb3df7a9aff1d4e48eede7a7346998bd95f897ec27f0b484c5eb3c7bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:76435a59768a5de70e77a98036eb59806557c6afd16a473fb421022a30d791a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123656656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:250ac1974470ba054ae919a1731e92dab69ada7fc78f9c7bcd2a42c67dd5b56a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Jan 2022 22:34:30 GMT
ADD file:18acb1f3ef1ffe1aeaff1aa22861026180d22104f6f14dd8bc4656777800fd9f in / 
# Wed, 12 Jan 2022 22:34:30 GMT
CMD ["/bin/bash"]
# Fri, 18 Feb 2022 01:23:36 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 18 Feb 2022 01:23:36 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Feb 2022 01:23:40 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Feb 2022 22:26:27 GMT
RUN set -eux; 	yum install -y 		gzip 		xz 	; 	yum clean all
# Wed, 23 Feb 2022 22:27:06 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:27:07 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 23 Feb 2022 22:27:07 GMT
ENV MYSQL_VERSION=5.7.37-1.el7
# Wed, 23 Feb 2022 22:27:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 23 Feb 2022 22:27:27 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 23 Feb 2022 22:27:28 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 23 Feb 2022 22:27:28 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el7
# Wed, 23 Feb 2022 22:27:46 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 23 Feb 2022 22:27:46 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:27:47 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:27:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:27:47 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:27:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1e1d49338f200e5dab7ef55f9d3a37259af48812603e07ae59e43615f9038b27`  
		Last Modified: Wed, 12 Jan 2022 22:35:18 GMT  
		Size: 48.3 MB (48330956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66218a3b537b220bfcc60a7592e8334f387d5189667b2364be8266fdf038a03f`  
		Last Modified: Fri, 18 Feb 2022 01:26:48 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e2fa6d94c92997a80329028540d0f0e421e44aa0d58069d03944a79c152089`  
		Last Modified: Fri, 18 Feb 2022 01:26:48 GMT  
		Size: 930.2 KB (930228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6800d2a84cbc0ba3c39d909b1631f8c89a5a82c9b63c3173a31b013910a64a`  
		Last Modified: Wed, 23 Feb 2022 22:29:56 GMT  
		Size: 2.7 MB (2667220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665a131c9d2e9f51044d6b456f6227d3bc51f50eb33ecf44ae8acee1ee70d25d`  
		Last Modified: Wed, 23 Feb 2022 22:29:55 GMT  
		Size: 2.7 KB (2666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc57f84c66d58cef52bb795f8686a4b762dd6d61af0f5fac16a1ec7df93546da`  
		Last Modified: Wed, 23 Feb 2022 22:29:53 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27f40f7b5b424896da7dd2f9b1faff3c2360119811ce0c77cd5f753d17e1c35`  
		Last Modified: Wed, 23 Feb 2022 22:29:57 GMT  
		Size: 25.4 MB (25401979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc3e6d094d9b21f9e3636bb95d3dc8387a1a8b2f5c284420cf97c7898b07270`  
		Last Modified: Wed, 23 Feb 2022 22:29:53 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468635081a56d4d4c9d48a88541026ee0cfc22513a1b53ac29da0f306c5229c0`  
		Last Modified: Wed, 23 Feb 2022 22:30:02 GMT  
		Size: 46.3 MB (46316937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96812f7d9d74f531f52dc68d110c830f4e4fad982a1c082ec775b380999b2bc`  
		Last Modified: Wed, 23 Feb 2022 22:29:53 GMT  
		Size: 5.0 KB (4953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.37`

```console
$ docker pull mysql@sha256:ea24ddf1116d6e5053919748d2c27c8200e39ac0dbe9540f213a2d9141b66167
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.37` - linux; amd64

```console
$ docker pull mysql@sha256:5adbbb05d43e67a7ed5f4856d3831b22ece5178d23c565b31cef61f92e3467ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154804997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538ec2c8721c073370299bf83ae46b940c83899f44cc90d89799a046afc5816b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Wed, 23 Feb 2022 22:27:55 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:28:14 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:28:15 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:28:15 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:28:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:28:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:28:16 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:28:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45b9a309e746ae5e6074efb8d35490146b3188f1375fd6abe60763a4b13b79`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90242da46c5709e3df233b61e042de5002a59567de7c18a68c75935d386195d9`  
		Last Modified: Wed, 23 Feb 2022 22:30:30 GMT  
		Size: 108.6 MB (108636729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d822d1293bf6661e4e6c69c425a5e9fca7b43bbf1201c1c66effbebd275d4`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 5.0 KB (4954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1704bf9fa7759625eeda74bcf484357dd06e4ef8d46319f09b59d4fd4c154eab`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.37-debian`

```console
$ docker pull mysql@sha256:ea24ddf1116d6e5053919748d2c27c8200e39ac0dbe9540f213a2d9141b66167
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.37-debian` - linux; amd64

```console
$ docker pull mysql@sha256:5adbbb05d43e67a7ed5f4856d3831b22ece5178d23c565b31cef61f92e3467ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154804997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538ec2c8721c073370299bf83ae46b940c83899f44cc90d89799a046afc5816b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Wed, 23 Feb 2022 22:27:55 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:28:14 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:28:15 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:28:15 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:28:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:28:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:28:16 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:28:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45b9a309e746ae5e6074efb8d35490146b3188f1375fd6abe60763a4b13b79`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90242da46c5709e3df233b61e042de5002a59567de7c18a68c75935d386195d9`  
		Last Modified: Wed, 23 Feb 2022 22:30:30 GMT  
		Size: 108.6 MB (108636729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d822d1293bf6661e4e6c69c425a5e9fca7b43bbf1201c1c66effbebd275d4`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 5.0 KB (4954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1704bf9fa7759625eeda74bcf484357dd06e4ef8d46319f09b59d4fd4c154eab`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.37-oracle`

```console
$ docker pull mysql@sha256:898fe77fb3df7a9aff1d4e48eede7a7346998bd95f897ec27f0b484c5eb3c7bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.37-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:76435a59768a5de70e77a98036eb59806557c6afd16a473fb421022a30d791a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123656656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:250ac1974470ba054ae919a1731e92dab69ada7fc78f9c7bcd2a42c67dd5b56a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Jan 2022 22:34:30 GMT
ADD file:18acb1f3ef1ffe1aeaff1aa22861026180d22104f6f14dd8bc4656777800fd9f in / 
# Wed, 12 Jan 2022 22:34:30 GMT
CMD ["/bin/bash"]
# Fri, 18 Feb 2022 01:23:36 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 18 Feb 2022 01:23:36 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Feb 2022 01:23:40 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Feb 2022 22:26:27 GMT
RUN set -eux; 	yum install -y 		gzip 		xz 	; 	yum clean all
# Wed, 23 Feb 2022 22:27:06 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:27:07 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 23 Feb 2022 22:27:07 GMT
ENV MYSQL_VERSION=5.7.37-1.el7
# Wed, 23 Feb 2022 22:27:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 23 Feb 2022 22:27:27 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 23 Feb 2022 22:27:28 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 23 Feb 2022 22:27:28 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el7
# Wed, 23 Feb 2022 22:27:46 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 23 Feb 2022 22:27:46 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:27:47 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:27:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:27:47 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:27:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1e1d49338f200e5dab7ef55f9d3a37259af48812603e07ae59e43615f9038b27`  
		Last Modified: Wed, 12 Jan 2022 22:35:18 GMT  
		Size: 48.3 MB (48330956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66218a3b537b220bfcc60a7592e8334f387d5189667b2364be8266fdf038a03f`  
		Last Modified: Fri, 18 Feb 2022 01:26:48 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e2fa6d94c92997a80329028540d0f0e421e44aa0d58069d03944a79c152089`  
		Last Modified: Fri, 18 Feb 2022 01:26:48 GMT  
		Size: 930.2 KB (930228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6800d2a84cbc0ba3c39d909b1631f8c89a5a82c9b63c3173a31b013910a64a`  
		Last Modified: Wed, 23 Feb 2022 22:29:56 GMT  
		Size: 2.7 MB (2667220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665a131c9d2e9f51044d6b456f6227d3bc51f50eb33ecf44ae8acee1ee70d25d`  
		Last Modified: Wed, 23 Feb 2022 22:29:55 GMT  
		Size: 2.7 KB (2666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc57f84c66d58cef52bb795f8686a4b762dd6d61af0f5fac16a1ec7df93546da`  
		Last Modified: Wed, 23 Feb 2022 22:29:53 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27f40f7b5b424896da7dd2f9b1faff3c2360119811ce0c77cd5f753d17e1c35`  
		Last Modified: Wed, 23 Feb 2022 22:29:57 GMT  
		Size: 25.4 MB (25401979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc3e6d094d9b21f9e3636bb95d3dc8387a1a8b2f5c284420cf97c7898b07270`  
		Last Modified: Wed, 23 Feb 2022 22:29:53 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468635081a56d4d4c9d48a88541026ee0cfc22513a1b53ac29da0f306c5229c0`  
		Last Modified: Wed, 23 Feb 2022 22:30:02 GMT  
		Size: 46.3 MB (46316937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96812f7d9d74f531f52dc68d110c830f4e4fad982a1c082ec775b380999b2bc`  
		Last Modified: Wed, 23 Feb 2022 22:29:53 GMT  
		Size: 5.0 KB (4953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:0962b771c2398c6dcddbbe77b3cf6658408396229b612035d938fb7c8d11c23c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:cb4641c97c8f216961b223f676fc68bd376b5197d64d2657b5c331a89af6c08b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153973656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6126b4587b1b7a4ecbfcbabfa34164ca060416d0b58b2aa55d5a7e8f5e336761`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:25:52 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 22:25:53 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Wed, 23 Feb 2022 22:25:53 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:26:08 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:26:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:26:09 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 23 Feb 2022 22:26:09 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:26:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:26:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:26:10 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:26:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71174f5fcbee70701ee49220cb1c6dc17c80ecccd06f591416a72bedfcd84e37`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e368ab37acf00b9102e4ad1989d99174aba158de3348550f244de2bc96d7d7`  
		Last Modified: Wed, 23 Feb 2022 22:29:25 GMT  
		Size: 107.8 MB (107804538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dd10975b5ee27e41ce108ad67ad33b3f3d71590588e46336fd6785602e0e82`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e9459cbd3ebfd000d9ed6f515804cad2e3d81e2782387e0e7dbdab8b0de1e7`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 5.0 KB (4955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c49252794494c412bf391410f784ed593bd5f41693a1fd1d9de50c8f60db1f`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:0962b771c2398c6dcddbbe77b3cf6658408396229b612035d938fb7c8d11c23c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:cb4641c97c8f216961b223f676fc68bd376b5197d64d2657b5c331a89af6c08b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153973656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6126b4587b1b7a4ecbfcbabfa34164ca060416d0b58b2aa55d5a7e8f5e336761`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:25:52 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 22:25:53 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Wed, 23 Feb 2022 22:25:53 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:26:08 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:26:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:26:09 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 23 Feb 2022 22:26:09 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:26:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:26:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:26:10 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:26:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71174f5fcbee70701ee49220cb1c6dc17c80ecccd06f591416a72bedfcd84e37`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e368ab37acf00b9102e4ad1989d99174aba158de3348550f244de2bc96d7d7`  
		Last Modified: Wed, 23 Feb 2022 22:29:25 GMT  
		Size: 107.8 MB (107804538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dd10975b5ee27e41ce108ad67ad33b3f3d71590588e46336fd6785602e0e82`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e9459cbd3ebfd000d9ed6f515804cad2e3d81e2782387e0e7dbdab8b0de1e7`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 5.0 KB (4955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c49252794494c412bf391410f784ed593bd5f41693a1fd1d9de50c8f60db1f`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:2eb7bc58b17710d284336d820a405713b34567e7a5334fe43a25fc8bb15adcd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:eed6e430fd994c63855936d54e9b0bf0ce19c49b05d69885dd6f829a26e51863
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131617605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f183b9246e187b0853e41a46e4dc8ea5435c80cf1e57eb4874230de890003fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 11 Feb 2022 18:20:31 GMT
ADD file:636d5d8575ec6ddd380a3bbf41530219d37249378b4abd151d94842377cc55d9 in / 
# Fri, 11 Feb 2022 18:20:32 GMT
CMD ["/bin/bash"]
# Fri, 18 Feb 2022 01:20:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 18 Feb 2022 01:20:09 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Feb 2022 01:20:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Feb 2022 22:23:32 GMT
RUN set -eux; 	microdnf install -y 		gzip 		xz 		findutils 	; 	microdnf clean all
# Wed, 23 Feb 2022 22:24:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:24:04 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 22:24:04 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 22:24:05 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 23 Feb 2022 22:24:31 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 23 Feb 2022 22:24:32 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 23 Feb 2022 22:24:32 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 22:25:01 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 23 Feb 2022 22:25:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:25:02 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:25:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:25:03 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:25:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:010357f4c091049bd23724817a1881f575ff94d35f4c621b4f87b2876049650b`  
		Last Modified: Fri, 11 Feb 2022 18:21:24 GMT  
		Size: 42.1 MB (42105112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efa408bcdb6fa7a3da670da56c2117a4fc7969a39ab0e37db4bb4e52b1d38ba`  
		Last Modified: Fri, 18 Feb 2022 01:25:39 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290fe0478d05d79d3ad6a2676a72d0ba98072c8e9fad91f0ff027c0db9e7d5e8`  
		Last Modified: Fri, 18 Feb 2022 01:25:38 GMT  
		Size: 928.8 KB (928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa56e25ec4a3c7323416334e4a4793cf96e15c41a932dea7f53c1e4108257350`  
		Last Modified: Wed, 23 Feb 2022 22:28:48 GMT  
		Size: 3.1 MB (3113953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10c6a4a3a0ad6f0500c05bb769e3ecc16377abcdc9c5a5304733802ee0bde4`  
		Last Modified: Wed, 23 Feb 2022 22:28:47 GMT  
		Size: 2.6 KB (2632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034a3d622cdea03f8379a45c247082878562bc7f065ea5086174d82cf8bd496f`  
		Last Modified: Wed, 23 Feb 2022 22:28:45 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc047b4f4b9360b5d4a0a79c5b6cf947abe3dfde63341994704a4009dd07c7b4`  
		Last Modified: Wed, 23 Feb 2022 22:28:53 GMT  
		Size: 47.2 MB (47224498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7c5f631597f88f38162bfa0184433689ff5b9cb48f4a689a77bba96d512ab0`  
		Last Modified: Wed, 23 Feb 2022 22:28:45 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a7de42af515f14c2391b8e7f228c660a47a7264e3d55d2dbe79fe0b8bf85fa`  
		Last Modified: Wed, 23 Feb 2022 22:28:53 GMT  
		Size: 38.2 MB (38235885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b92fe8f855ead02f0b27b7b73a057519f0fbe787e546659341a10c057ccb07`  
		Last Modified: Wed, 23 Feb 2022 22:28:46 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:b156b996b09d1509a78a84dd5a71cf673b5ff60c3ae22c27194e62ac2a7d1266
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (139997480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b3b1d5bc990340c2df8472a7a78af238dfb761ace123d9b13ccd4d3dfc4332`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 11 Feb 2022 18:58:36 GMT
ADD file:8d5a0dcc45ab23c7b507e80b63e5752d94837f490600ce95fb8ba8ed2f7baa2d in / 
# Fri, 11 Feb 2022 18:58:37 GMT
CMD ["/bin/bash"]
# Fri, 18 Feb 2022 01:40:08 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 18 Feb 2022 01:40:09 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Feb 2022 01:40:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Feb 2022 21:40:19 GMT
RUN set -eux; 	microdnf install -y 		gzip 		xz 		findutils 	; 	microdnf clean all
# Wed, 23 Feb 2022 21:41:00 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 21:41:01 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 21:41:02 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 21:41:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 23 Feb 2022 21:41:25 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 23 Feb 2022 21:41:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 23 Feb 2022 21:41:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 21:41:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 23 Feb 2022 21:41:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 21:41:56 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 21:41:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 21:41:57 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 21:41:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ffdd659a9f05cadeed9c2d5cead839f585163662ca7f847a41fd64bb4e503f0c`  
		Last Modified: Fri, 11 Feb 2022 18:59:38 GMT  
		Size: 42.0 MB (42018804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0160f0527322be235d3dfdb8e677d5ef11bf2da725fc7a4c77f93c96d3d43c`  
		Last Modified: Fri, 18 Feb 2022 01:42:53 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4f9628b4dd4430ea84a7c1a9fc0c2c79a4528061ce123f84f5c31588ebe3aa`  
		Last Modified: Fri, 18 Feb 2022 01:42:51 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af70585b7a192f4e200798deae1a8cba89afbc03b7097032112e5bc4571f2660`  
		Last Modified: Wed, 23 Feb 2022 21:42:28 GMT  
		Size: 3.3 MB (3258221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a63cf661d5c4d9057b557f1268efa4cf1770596543728a33c76e31c3c38bf7`  
		Last Modified: Wed, 23 Feb 2022 21:42:27 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20f69348b09e5a78b36c179334aed779d534c322ee73c63149283f619fdf480`  
		Last Modified: Wed, 23 Feb 2022 21:42:25 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165d6f7910557f5385a0a152ca459c4a3a513a0be5091c54bea6c889e1093911`  
		Last Modified: Wed, 23 Feb 2022 21:42:33 GMT  
		Size: 53.4 MB (53382212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496a314c288f953196b7101c88f8b67bf0ae5a07cbc362202f3ec30fddc9ac2f`  
		Last Modified: Wed, 23 Feb 2022 21:42:25 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef4c71a5c7ada2f9db19897deb642356f81aa03dbf6811019ae506d089cad2e`  
		Last Modified: Wed, 23 Feb 2022 21:42:32 GMT  
		Size: 40.5 MB (40471863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb56c1084a5c94c7e6a9ee9e65bb8cbbe3fccf7193667900469ff5fa3756bc77`  
		Last Modified: Wed, 23 Feb 2022 21:42:25 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:0962b771c2398c6dcddbbe77b3cf6658408396229b612035d938fb7c8d11c23c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:cb4641c97c8f216961b223f676fc68bd376b5197d64d2657b5c331a89af6c08b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153973656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6126b4587b1b7a4ecbfcbabfa34164ca060416d0b58b2aa55d5a7e8f5e336761`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:25:52 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 22:25:53 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Wed, 23 Feb 2022 22:25:53 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:26:08 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:26:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:26:09 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 23 Feb 2022 22:26:09 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:26:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:26:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:26:10 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:26:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71174f5fcbee70701ee49220cb1c6dc17c80ecccd06f591416a72bedfcd84e37`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e368ab37acf00b9102e4ad1989d99174aba158de3348550f244de2bc96d7d7`  
		Last Modified: Wed, 23 Feb 2022 22:29:25 GMT  
		Size: 107.8 MB (107804538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dd10975b5ee27e41ce108ad67ad33b3f3d71590588e46336fd6785602e0e82`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e9459cbd3ebfd000d9ed6f515804cad2e3d81e2782387e0e7dbdab8b0de1e7`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 5.0 KB (4955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c49252794494c412bf391410f784ed593bd5f41693a1fd1d9de50c8f60db1f`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:0962b771c2398c6dcddbbe77b3cf6658408396229b612035d938fb7c8d11c23c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:cb4641c97c8f216961b223f676fc68bd376b5197d64d2657b5c331a89af6c08b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153973656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6126b4587b1b7a4ecbfcbabfa34164ca060416d0b58b2aa55d5a7e8f5e336761`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:25:52 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 22:25:53 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Wed, 23 Feb 2022 22:25:53 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:26:08 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:26:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:26:09 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 23 Feb 2022 22:26:09 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:26:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:26:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:26:10 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:26:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71174f5fcbee70701ee49220cb1c6dc17c80ecccd06f591416a72bedfcd84e37`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e368ab37acf00b9102e4ad1989d99174aba158de3348550f244de2bc96d7d7`  
		Last Modified: Wed, 23 Feb 2022 22:29:25 GMT  
		Size: 107.8 MB (107804538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dd10975b5ee27e41ce108ad67ad33b3f3d71590588e46336fd6785602e0e82`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e9459cbd3ebfd000d9ed6f515804cad2e3d81e2782387e0e7dbdab8b0de1e7`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 5.0 KB (4955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c49252794494c412bf391410f784ed593bd5f41693a1fd1d9de50c8f60db1f`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:2eb7bc58b17710d284336d820a405713b34567e7a5334fe43a25fc8bb15adcd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:eed6e430fd994c63855936d54e9b0bf0ce19c49b05d69885dd6f829a26e51863
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131617605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f183b9246e187b0853e41a46e4dc8ea5435c80cf1e57eb4874230de890003fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 11 Feb 2022 18:20:31 GMT
ADD file:636d5d8575ec6ddd380a3bbf41530219d37249378b4abd151d94842377cc55d9 in / 
# Fri, 11 Feb 2022 18:20:32 GMT
CMD ["/bin/bash"]
# Fri, 18 Feb 2022 01:20:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 18 Feb 2022 01:20:09 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Feb 2022 01:20:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Feb 2022 22:23:32 GMT
RUN set -eux; 	microdnf install -y 		gzip 		xz 		findutils 	; 	microdnf clean all
# Wed, 23 Feb 2022 22:24:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:24:04 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 22:24:04 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 22:24:05 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 23 Feb 2022 22:24:31 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 23 Feb 2022 22:24:32 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 23 Feb 2022 22:24:32 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 22:25:01 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 23 Feb 2022 22:25:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:25:02 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:25:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:25:03 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:25:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:010357f4c091049bd23724817a1881f575ff94d35f4c621b4f87b2876049650b`  
		Last Modified: Fri, 11 Feb 2022 18:21:24 GMT  
		Size: 42.1 MB (42105112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efa408bcdb6fa7a3da670da56c2117a4fc7969a39ab0e37db4bb4e52b1d38ba`  
		Last Modified: Fri, 18 Feb 2022 01:25:39 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290fe0478d05d79d3ad6a2676a72d0ba98072c8e9fad91f0ff027c0db9e7d5e8`  
		Last Modified: Fri, 18 Feb 2022 01:25:38 GMT  
		Size: 928.8 KB (928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa56e25ec4a3c7323416334e4a4793cf96e15c41a932dea7f53c1e4108257350`  
		Last Modified: Wed, 23 Feb 2022 22:28:48 GMT  
		Size: 3.1 MB (3113953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10c6a4a3a0ad6f0500c05bb769e3ecc16377abcdc9c5a5304733802ee0bde4`  
		Last Modified: Wed, 23 Feb 2022 22:28:47 GMT  
		Size: 2.6 KB (2632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034a3d622cdea03f8379a45c247082878562bc7f065ea5086174d82cf8bd496f`  
		Last Modified: Wed, 23 Feb 2022 22:28:45 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc047b4f4b9360b5d4a0a79c5b6cf947abe3dfde63341994704a4009dd07c7b4`  
		Last Modified: Wed, 23 Feb 2022 22:28:53 GMT  
		Size: 47.2 MB (47224498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7c5f631597f88f38162bfa0184433689ff5b9cb48f4a689a77bba96d512ab0`  
		Last Modified: Wed, 23 Feb 2022 22:28:45 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a7de42af515f14c2391b8e7f228c660a47a7264e3d55d2dbe79fe0b8bf85fa`  
		Last Modified: Wed, 23 Feb 2022 22:28:53 GMT  
		Size: 38.2 MB (38235885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b92fe8f855ead02f0b27b7b73a057519f0fbe787e546659341a10c057ccb07`  
		Last Modified: Wed, 23 Feb 2022 22:28:46 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:b156b996b09d1509a78a84dd5a71cf673b5ff60c3ae22c27194e62ac2a7d1266
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (139997480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b3b1d5bc990340c2df8472a7a78af238dfb761ace123d9b13ccd4d3dfc4332`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 11 Feb 2022 18:58:36 GMT
ADD file:8d5a0dcc45ab23c7b507e80b63e5752d94837f490600ce95fb8ba8ed2f7baa2d in / 
# Fri, 11 Feb 2022 18:58:37 GMT
CMD ["/bin/bash"]
# Fri, 18 Feb 2022 01:40:08 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 18 Feb 2022 01:40:09 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Feb 2022 01:40:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Feb 2022 21:40:19 GMT
RUN set -eux; 	microdnf install -y 		gzip 		xz 		findutils 	; 	microdnf clean all
# Wed, 23 Feb 2022 21:41:00 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 21:41:01 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 21:41:02 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 21:41:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 23 Feb 2022 21:41:25 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 23 Feb 2022 21:41:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 23 Feb 2022 21:41:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 21:41:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 23 Feb 2022 21:41:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 21:41:56 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 21:41:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 21:41:57 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 21:41:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ffdd659a9f05cadeed9c2d5cead839f585163662ca7f847a41fd64bb4e503f0c`  
		Last Modified: Fri, 11 Feb 2022 18:59:38 GMT  
		Size: 42.0 MB (42018804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0160f0527322be235d3dfdb8e677d5ef11bf2da725fc7a4c77f93c96d3d43c`  
		Last Modified: Fri, 18 Feb 2022 01:42:53 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4f9628b4dd4430ea84a7c1a9fc0c2c79a4528061ce123f84f5c31588ebe3aa`  
		Last Modified: Fri, 18 Feb 2022 01:42:51 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af70585b7a192f4e200798deae1a8cba89afbc03b7097032112e5bc4571f2660`  
		Last Modified: Wed, 23 Feb 2022 21:42:28 GMT  
		Size: 3.3 MB (3258221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a63cf661d5c4d9057b557f1268efa4cf1770596543728a33c76e31c3c38bf7`  
		Last Modified: Wed, 23 Feb 2022 21:42:27 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20f69348b09e5a78b36c179334aed779d534c322ee73c63149283f619fdf480`  
		Last Modified: Wed, 23 Feb 2022 21:42:25 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165d6f7910557f5385a0a152ca459c4a3a513a0be5091c54bea6c889e1093911`  
		Last Modified: Wed, 23 Feb 2022 21:42:33 GMT  
		Size: 53.4 MB (53382212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496a314c288f953196b7101c88f8b67bf0ae5a07cbc362202f3ec30fddc9ac2f`  
		Last Modified: Wed, 23 Feb 2022 21:42:25 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef4c71a5c7ada2f9db19897deb642356f81aa03dbf6811019ae506d089cad2e`  
		Last Modified: Wed, 23 Feb 2022 21:42:32 GMT  
		Size: 40.5 MB (40471863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb56c1084a5c94c7e6a9ee9e65bb8cbbe3fccf7193667900469ff5fa3756bc77`  
		Last Modified: Wed, 23 Feb 2022 21:42:25 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.28`

```console
$ docker pull mysql@sha256:0962b771c2398c6dcddbbe77b3cf6658408396229b612035d938fb7c8d11c23c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.28` - linux; amd64

```console
$ docker pull mysql@sha256:cb4641c97c8f216961b223f676fc68bd376b5197d64d2657b5c331a89af6c08b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153973656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6126b4587b1b7a4ecbfcbabfa34164ca060416d0b58b2aa55d5a7e8f5e336761`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:25:52 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 22:25:53 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Wed, 23 Feb 2022 22:25:53 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:26:08 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:26:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:26:09 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 23 Feb 2022 22:26:09 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:26:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:26:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:26:10 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:26:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71174f5fcbee70701ee49220cb1c6dc17c80ecccd06f591416a72bedfcd84e37`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e368ab37acf00b9102e4ad1989d99174aba158de3348550f244de2bc96d7d7`  
		Last Modified: Wed, 23 Feb 2022 22:29:25 GMT  
		Size: 107.8 MB (107804538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dd10975b5ee27e41ce108ad67ad33b3f3d71590588e46336fd6785602e0e82`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e9459cbd3ebfd000d9ed6f515804cad2e3d81e2782387e0e7dbdab8b0de1e7`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 5.0 KB (4955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c49252794494c412bf391410f784ed593bd5f41693a1fd1d9de50c8f60db1f`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.28-debian`

```console
$ docker pull mysql@sha256:0962b771c2398c6dcddbbe77b3cf6658408396229b612035d938fb7c8d11c23c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.28-debian` - linux; amd64

```console
$ docker pull mysql@sha256:cb4641c97c8f216961b223f676fc68bd376b5197d64d2657b5c331a89af6c08b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153973656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6126b4587b1b7a4ecbfcbabfa34164ca060416d0b58b2aa55d5a7e8f5e336761`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:25:52 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 22:25:53 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Wed, 23 Feb 2022 22:25:53 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:26:08 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:26:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:26:09 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 23 Feb 2022 22:26:09 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:26:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:26:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:26:10 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:26:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71174f5fcbee70701ee49220cb1c6dc17c80ecccd06f591416a72bedfcd84e37`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e368ab37acf00b9102e4ad1989d99174aba158de3348550f244de2bc96d7d7`  
		Last Modified: Wed, 23 Feb 2022 22:29:25 GMT  
		Size: 107.8 MB (107804538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dd10975b5ee27e41ce108ad67ad33b3f3d71590588e46336fd6785602e0e82`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e9459cbd3ebfd000d9ed6f515804cad2e3d81e2782387e0e7dbdab8b0de1e7`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 5.0 KB (4955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c49252794494c412bf391410f784ed593bd5f41693a1fd1d9de50c8f60db1f`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.28-oracle`

```console
$ docker pull mysql@sha256:2eb7bc58b17710d284336d820a405713b34567e7a5334fe43a25fc8bb15adcd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.28-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:eed6e430fd994c63855936d54e9b0bf0ce19c49b05d69885dd6f829a26e51863
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131617605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f183b9246e187b0853e41a46e4dc8ea5435c80cf1e57eb4874230de890003fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 11 Feb 2022 18:20:31 GMT
ADD file:636d5d8575ec6ddd380a3bbf41530219d37249378b4abd151d94842377cc55d9 in / 
# Fri, 11 Feb 2022 18:20:32 GMT
CMD ["/bin/bash"]
# Fri, 18 Feb 2022 01:20:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 18 Feb 2022 01:20:09 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Feb 2022 01:20:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Feb 2022 22:23:32 GMT
RUN set -eux; 	microdnf install -y 		gzip 		xz 		findutils 	; 	microdnf clean all
# Wed, 23 Feb 2022 22:24:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:24:04 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 22:24:04 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 22:24:05 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 23 Feb 2022 22:24:31 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 23 Feb 2022 22:24:32 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 23 Feb 2022 22:24:32 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 22:25:01 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 23 Feb 2022 22:25:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:25:02 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:25:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:25:03 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:25:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:010357f4c091049bd23724817a1881f575ff94d35f4c621b4f87b2876049650b`  
		Last Modified: Fri, 11 Feb 2022 18:21:24 GMT  
		Size: 42.1 MB (42105112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efa408bcdb6fa7a3da670da56c2117a4fc7969a39ab0e37db4bb4e52b1d38ba`  
		Last Modified: Fri, 18 Feb 2022 01:25:39 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290fe0478d05d79d3ad6a2676a72d0ba98072c8e9fad91f0ff027c0db9e7d5e8`  
		Last Modified: Fri, 18 Feb 2022 01:25:38 GMT  
		Size: 928.8 KB (928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa56e25ec4a3c7323416334e4a4793cf96e15c41a932dea7f53c1e4108257350`  
		Last Modified: Wed, 23 Feb 2022 22:28:48 GMT  
		Size: 3.1 MB (3113953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10c6a4a3a0ad6f0500c05bb769e3ecc16377abcdc9c5a5304733802ee0bde4`  
		Last Modified: Wed, 23 Feb 2022 22:28:47 GMT  
		Size: 2.6 KB (2632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034a3d622cdea03f8379a45c247082878562bc7f065ea5086174d82cf8bd496f`  
		Last Modified: Wed, 23 Feb 2022 22:28:45 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc047b4f4b9360b5d4a0a79c5b6cf947abe3dfde63341994704a4009dd07c7b4`  
		Last Modified: Wed, 23 Feb 2022 22:28:53 GMT  
		Size: 47.2 MB (47224498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7c5f631597f88f38162bfa0184433689ff5b9cb48f4a689a77bba96d512ab0`  
		Last Modified: Wed, 23 Feb 2022 22:28:45 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a7de42af515f14c2391b8e7f228c660a47a7264e3d55d2dbe79fe0b8bf85fa`  
		Last Modified: Wed, 23 Feb 2022 22:28:53 GMT  
		Size: 38.2 MB (38235885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b92fe8f855ead02f0b27b7b73a057519f0fbe787e546659341a10c057ccb07`  
		Last Modified: Wed, 23 Feb 2022 22:28:46 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.28-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:b156b996b09d1509a78a84dd5a71cf673b5ff60c3ae22c27194e62ac2a7d1266
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (139997480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b3b1d5bc990340c2df8472a7a78af238dfb761ace123d9b13ccd4d3dfc4332`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 11 Feb 2022 18:58:36 GMT
ADD file:8d5a0dcc45ab23c7b507e80b63e5752d94837f490600ce95fb8ba8ed2f7baa2d in / 
# Fri, 11 Feb 2022 18:58:37 GMT
CMD ["/bin/bash"]
# Fri, 18 Feb 2022 01:40:08 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 18 Feb 2022 01:40:09 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Feb 2022 01:40:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Feb 2022 21:40:19 GMT
RUN set -eux; 	microdnf install -y 		gzip 		xz 		findutils 	; 	microdnf clean all
# Wed, 23 Feb 2022 21:41:00 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 21:41:01 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 21:41:02 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 21:41:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 23 Feb 2022 21:41:25 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 23 Feb 2022 21:41:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 23 Feb 2022 21:41:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 21:41:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 23 Feb 2022 21:41:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 21:41:56 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 21:41:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 21:41:57 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 21:41:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ffdd659a9f05cadeed9c2d5cead839f585163662ca7f847a41fd64bb4e503f0c`  
		Last Modified: Fri, 11 Feb 2022 18:59:38 GMT  
		Size: 42.0 MB (42018804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0160f0527322be235d3dfdb8e677d5ef11bf2da725fc7a4c77f93c96d3d43c`  
		Last Modified: Fri, 18 Feb 2022 01:42:53 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4f9628b4dd4430ea84a7c1a9fc0c2c79a4528061ce123f84f5c31588ebe3aa`  
		Last Modified: Fri, 18 Feb 2022 01:42:51 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af70585b7a192f4e200798deae1a8cba89afbc03b7097032112e5bc4571f2660`  
		Last Modified: Wed, 23 Feb 2022 21:42:28 GMT  
		Size: 3.3 MB (3258221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a63cf661d5c4d9057b557f1268efa4cf1770596543728a33c76e31c3c38bf7`  
		Last Modified: Wed, 23 Feb 2022 21:42:27 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20f69348b09e5a78b36c179334aed779d534c322ee73c63149283f619fdf480`  
		Last Modified: Wed, 23 Feb 2022 21:42:25 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165d6f7910557f5385a0a152ca459c4a3a513a0be5091c54bea6c889e1093911`  
		Last Modified: Wed, 23 Feb 2022 21:42:33 GMT  
		Size: 53.4 MB (53382212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496a314c288f953196b7101c88f8b67bf0ae5a07cbc362202f3ec30fddc9ac2f`  
		Last Modified: Wed, 23 Feb 2022 21:42:25 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef4c71a5c7ada2f9db19897deb642356f81aa03dbf6811019ae506d089cad2e`  
		Last Modified: Wed, 23 Feb 2022 21:42:32 GMT  
		Size: 40.5 MB (40471863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb56c1084a5c94c7e6a9ee9e65bb8cbbe3fccf7193667900469ff5fa3756bc77`  
		Last Modified: Wed, 23 Feb 2022 21:42:25 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:0962b771c2398c6dcddbbe77b3cf6658408396229b612035d938fb7c8d11c23c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:cb4641c97c8f216961b223f676fc68bd376b5197d64d2657b5c331a89af6c08b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153973656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6126b4587b1b7a4ecbfcbabfa34164ca060416d0b58b2aa55d5a7e8f5e336761`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:25:52 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 22:25:53 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Wed, 23 Feb 2022 22:25:53 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:26:08 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:26:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:26:09 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 23 Feb 2022 22:26:09 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:26:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:26:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:26:10 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:26:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71174f5fcbee70701ee49220cb1c6dc17c80ecccd06f591416a72bedfcd84e37`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e368ab37acf00b9102e4ad1989d99174aba158de3348550f244de2bc96d7d7`  
		Last Modified: Wed, 23 Feb 2022 22:29:25 GMT  
		Size: 107.8 MB (107804538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dd10975b5ee27e41ce108ad67ad33b3f3d71590588e46336fd6785602e0e82`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e9459cbd3ebfd000d9ed6f515804cad2e3d81e2782387e0e7dbdab8b0de1e7`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 5.0 KB (4955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c49252794494c412bf391410f784ed593bd5f41693a1fd1d9de50c8f60db1f`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:0962b771c2398c6dcddbbe77b3cf6658408396229b612035d938fb7c8d11c23c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:cb4641c97c8f216961b223f676fc68bd376b5197d64d2657b5c331a89af6c08b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153973656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6126b4587b1b7a4ecbfcbabfa34164ca060416d0b58b2aa55d5a7e8f5e336761`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:25:52 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 22:25:53 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Wed, 23 Feb 2022 22:25:53 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:26:08 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:26:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:26:09 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 23 Feb 2022 22:26:09 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:26:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:26:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:26:10 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:26:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71174f5fcbee70701ee49220cb1c6dc17c80ecccd06f591416a72bedfcd84e37`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e368ab37acf00b9102e4ad1989d99174aba158de3348550f244de2bc96d7d7`  
		Last Modified: Wed, 23 Feb 2022 22:29:25 GMT  
		Size: 107.8 MB (107804538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dd10975b5ee27e41ce108ad67ad33b3f3d71590588e46336fd6785602e0e82`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e9459cbd3ebfd000d9ed6f515804cad2e3d81e2782387e0e7dbdab8b0de1e7`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 5.0 KB (4955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c49252794494c412bf391410f784ed593bd5f41693a1fd1d9de50c8f60db1f`  
		Last Modified: Wed, 23 Feb 2022 22:29:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:2eb7bc58b17710d284336d820a405713b34567e7a5334fe43a25fc8bb15adcd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:eed6e430fd994c63855936d54e9b0bf0ce19c49b05d69885dd6f829a26e51863
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131617605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f183b9246e187b0853e41a46e4dc8ea5435c80cf1e57eb4874230de890003fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 11 Feb 2022 18:20:31 GMT
ADD file:636d5d8575ec6ddd380a3bbf41530219d37249378b4abd151d94842377cc55d9 in / 
# Fri, 11 Feb 2022 18:20:32 GMT
CMD ["/bin/bash"]
# Fri, 18 Feb 2022 01:20:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 18 Feb 2022 01:20:09 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Feb 2022 01:20:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Feb 2022 22:23:32 GMT
RUN set -eux; 	microdnf install -y 		gzip 		xz 		findutils 	; 	microdnf clean all
# Wed, 23 Feb 2022 22:24:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:24:04 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 22:24:04 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 22:24:05 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 23 Feb 2022 22:24:31 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 23 Feb 2022 22:24:32 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 23 Feb 2022 22:24:32 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 22:25:01 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 23 Feb 2022 22:25:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:25:02 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:25:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:25:03 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:25:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:010357f4c091049bd23724817a1881f575ff94d35f4c621b4f87b2876049650b`  
		Last Modified: Fri, 11 Feb 2022 18:21:24 GMT  
		Size: 42.1 MB (42105112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efa408bcdb6fa7a3da670da56c2117a4fc7969a39ab0e37db4bb4e52b1d38ba`  
		Last Modified: Fri, 18 Feb 2022 01:25:39 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290fe0478d05d79d3ad6a2676a72d0ba98072c8e9fad91f0ff027c0db9e7d5e8`  
		Last Modified: Fri, 18 Feb 2022 01:25:38 GMT  
		Size: 928.8 KB (928833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa56e25ec4a3c7323416334e4a4793cf96e15c41a932dea7f53c1e4108257350`  
		Last Modified: Wed, 23 Feb 2022 22:28:48 GMT  
		Size: 3.1 MB (3113953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10c6a4a3a0ad6f0500c05bb769e3ecc16377abcdc9c5a5304733802ee0bde4`  
		Last Modified: Wed, 23 Feb 2022 22:28:47 GMT  
		Size: 2.6 KB (2632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034a3d622cdea03f8379a45c247082878562bc7f065ea5086174d82cf8bd496f`  
		Last Modified: Wed, 23 Feb 2022 22:28:45 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc047b4f4b9360b5d4a0a79c5b6cf947abe3dfde63341994704a4009dd07c7b4`  
		Last Modified: Wed, 23 Feb 2022 22:28:53 GMT  
		Size: 47.2 MB (47224498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7c5f631597f88f38162bfa0184433689ff5b9cb48f4a689a77bba96d512ab0`  
		Last Modified: Wed, 23 Feb 2022 22:28:45 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a7de42af515f14c2391b8e7f228c660a47a7264e3d55d2dbe79fe0b8bf85fa`  
		Last Modified: Wed, 23 Feb 2022 22:28:53 GMT  
		Size: 38.2 MB (38235885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b92fe8f855ead02f0b27b7b73a057519f0fbe787e546659341a10c057ccb07`  
		Last Modified: Wed, 23 Feb 2022 22:28:46 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:b156b996b09d1509a78a84dd5a71cf673b5ff60c3ae22c27194e62ac2a7d1266
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (139997480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b3b1d5bc990340c2df8472a7a78af238dfb761ace123d9b13ccd4d3dfc4332`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 11 Feb 2022 18:58:36 GMT
ADD file:8d5a0dcc45ab23c7b507e80b63e5752d94837f490600ce95fb8ba8ed2f7baa2d in / 
# Fri, 11 Feb 2022 18:58:37 GMT
CMD ["/bin/bash"]
# Fri, 18 Feb 2022 01:40:08 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Fri, 18 Feb 2022 01:40:09 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Feb 2022 01:40:13 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Feb 2022 21:40:19 GMT
RUN set -eux; 	microdnf install -y 		gzip 		xz 		findutils 	; 	microdnf clean all
# Wed, 23 Feb 2022 21:41:00 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 21:41:01 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 23 Feb 2022 21:41:02 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 21:41:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 23 Feb 2022 21:41:25 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Wed, 23 Feb 2022 21:41:26 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 23 Feb 2022 21:41:26 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Wed, 23 Feb 2022 21:41:54 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 23 Feb 2022 21:41:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 21:41:56 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 21:41:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 21:41:57 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 21:41:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ffdd659a9f05cadeed9c2d5cead839f585163662ca7f847a41fd64bb4e503f0c`  
		Last Modified: Fri, 11 Feb 2022 18:59:38 GMT  
		Size: 42.0 MB (42018804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0160f0527322be235d3dfdb8e677d5ef11bf2da725fc7a4c77f93c96d3d43c`  
		Last Modified: Fri, 18 Feb 2022 01:42:53 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4f9628b4dd4430ea84a7c1a9fc0c2c79a4528061ce123f84f5c31588ebe3aa`  
		Last Modified: Fri, 18 Feb 2022 01:42:51 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af70585b7a192f4e200798deae1a8cba89afbc03b7097032112e5bc4571f2660`  
		Last Modified: Wed, 23 Feb 2022 21:42:28 GMT  
		Size: 3.3 MB (3258221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a63cf661d5c4d9057b557f1268efa4cf1770596543728a33c76e31c3c38bf7`  
		Last Modified: Wed, 23 Feb 2022 21:42:27 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20f69348b09e5a78b36c179334aed779d534c322ee73c63149283f619fdf480`  
		Last Modified: Wed, 23 Feb 2022 21:42:25 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165d6f7910557f5385a0a152ca459c4a3a513a0be5091c54bea6c889e1093911`  
		Last Modified: Wed, 23 Feb 2022 21:42:33 GMT  
		Size: 53.4 MB (53382212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496a314c288f953196b7101c88f8b67bf0ae5a07cbc362202f3ec30fddc9ac2f`  
		Last Modified: Wed, 23 Feb 2022 21:42:25 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef4c71a5c7ada2f9db19897deb642356f81aa03dbf6811019ae506d089cad2e`  
		Last Modified: Wed, 23 Feb 2022 21:42:32 GMT  
		Size: 40.5 MB (40471863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb56c1084a5c94c7e6a9ee9e65bb8cbbe3fccf7193667900469ff5fa3756bc77`  
		Last Modified: Wed, 23 Feb 2022 21:42:25 GMT  
		Size: 5.0 KB (4956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
