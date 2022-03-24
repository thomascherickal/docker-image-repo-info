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
$ docker pull mysql@sha256:c8f68301981a7224cc9c063fc7a97b6ef13cfc4142b4871d1a35c95777ce96f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:cac49b06d95908bde09e2dcdadb4fa915c3fb3b0228e4e79e44f67b4024eb571
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155419411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05311a87aeb4d7f98b2726c39d4d29d6a174d20953a6d1ceaa236bfa177f5fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:06:24 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 18 Mar 2022 08:06:24 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Fri, 18 Mar 2022 08:06:25 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:53 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:54 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f242378e320c364d16b6d056493d7a6d02ccb0d0214cd43a092c09c2d196a89`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65503c01868a3fb0c4046bd568e0753952da09a77ee7b6babd5adf12c762ce`  
		Last Modified: Fri, 18 Mar 2022 08:09:14 GMT  
		Size: 108.6 MB (108637241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8944d50437c0d3db8b41c6f67af3c5a2fabccea9da92b293f4bbff80e5ca95`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 5.1 KB (5138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597d59a9a4245232eb602d93945953ad5217c782e5f3f62b4501905e68d54fdf`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:c8f68301981a7224cc9c063fc7a97b6ef13cfc4142b4871d1a35c95777ce96f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:cac49b06d95908bde09e2dcdadb4fa915c3fb3b0228e4e79e44f67b4024eb571
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155419411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05311a87aeb4d7f98b2726c39d4d29d6a174d20953a6d1ceaa236bfa177f5fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:06:24 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 18 Mar 2022 08:06:24 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Fri, 18 Mar 2022 08:06:25 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:53 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:54 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f242378e320c364d16b6d056493d7a6d02ccb0d0214cd43a092c09c2d196a89`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65503c01868a3fb0c4046bd568e0753952da09a77ee7b6babd5adf12c762ce`  
		Last Modified: Fri, 18 Mar 2022 08:09:14 GMT  
		Size: 108.6 MB (108637241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8944d50437c0d3db8b41c6f67af3c5a2fabccea9da92b293f4bbff80e5ca95`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 5.1 KB (5138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597d59a9a4245232eb602d93945953ad5217c782e5f3f62b4501905e68d54fdf`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:b8f8f1dca06f0f2bd4da7b7d3d0c98695afa55e495f274b279848b7eb786dec1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:90a57271a77fb51cb5e9062e6a4cc773c09ebb94693b382b728d4dc5b56d3344
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125156125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec092eca2e6f869c1b54d9098aad6f688b13e60bcbe5c5904100048ea30e0d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 18 Mar 2022 23:22:25 GMT
ADD file:19ae95221a518b3855b98aeb91f6c13f250d6caa59ee16bf155d73f7f5cdcc41 in / 
# Fri, 18 Mar 2022 23:22:26 GMT
CMD ["/bin/bash"]
# Sun, 20 Mar 2022 08:35:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Sun, 20 Mar 2022 08:35:33 GMT
ENV GOSU_VERSION=1.14
# Sun, 20 Mar 2022 08:35:37 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 20 Mar 2022 08:35:47 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sun, 20 Mar 2022 08:36:19 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sun, 20 Mar 2022 08:36:20 GMT
ENV MYSQL_MAJOR=5.7
# Sun, 20 Mar 2022 08:36:20 GMT
ENV MYSQL_VERSION=5.7.37-1.el7
# Sun, 20 Mar 2022 08:36:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sun, 20 Mar 2022 08:36:33 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Sun, 20 Mar 2022 08:36:34 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sun, 20 Mar 2022 08:36:34 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el7
# Sun, 20 Mar 2022 08:36:51 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sun, 20 Mar 2022 08:36:51 GMT
VOLUME [/var/lib/mysql]
# Sun, 20 Mar 2022 08:36:52 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Sun, 20 Mar 2022 08:36:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Mar 2022 08:36:52 GMT
EXPOSE 3306 33060
# Sun, 20 Mar 2022 08:36:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fb9cda09c679c7a8d70feb22223b7546c2d4d46d555312571fa2e3cc65347d9b`  
		Last Modified: Fri, 18 Mar 2022 23:23:20 GMT  
		Size: 48.7 MB (48745506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d92a669ae78e0afaed3ce5d7163161e8474e15d2847ae5d9238d773c805576`  
		Last Modified: Sun, 20 Mar 2022 08:37:27 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfca26c0cabc2152239d9d72138b28ee3a1352202681c195ad2ae9a44a35af5`  
		Last Modified: Sun, 20 Mar 2022 08:37:25 GMT  
		Size: 930.2 KB (930229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de8369545cab0fde8edb54d4280763d4ee1de6dfc159d36d14fb7838ba79d2`  
		Last Modified: Sun, 20 Mar 2022 08:37:26 GMT  
		Size: 3.7 MB (3713941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf98060af6cd1ba7d59edef4a89d04b75b819c6acb45de8350876db42877cb1f`  
		Last Modified: Sun, 20 Mar 2022 08:37:25 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abb0a38f4d7a31ace7a425d81577b64f34f1b662edb818e49c8f96cd974857`  
		Last Modified: Sun, 20 Mar 2022 08:37:23 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cab76a4536462713131d2b807d18360174f99ae81d5c415c68784df1e105eaf`  
		Last Modified: Sun, 20 Mar 2022 08:37:27 GMT  
		Size: 25.4 MB (25446301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0444456e33532f83e529c8c5526778a9ff87c60f334af9ed449ec94903fa4e40`  
		Last Modified: Sun, 20 Mar 2022 08:37:23 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9616457d9652fc11c5b9fd8f772a6d20a93aa805dc2a1c86e25671bad6e94eec`  
		Last Modified: Sun, 20 Mar 2022 08:37:31 GMT  
		Size: 46.3 MB (46310641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60c87db894a953c328163baa113579d7555cf47f8daf5ef088fae109065cbe`  
		Last Modified: Sun, 20 Mar 2022 08:37:23 GMT  
		Size: 5.1 KB (5138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:c8f68301981a7224cc9c063fc7a97b6ef13cfc4142b4871d1a35c95777ce96f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:cac49b06d95908bde09e2dcdadb4fa915c3fb3b0228e4e79e44f67b4024eb571
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155419411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05311a87aeb4d7f98b2726c39d4d29d6a174d20953a6d1ceaa236bfa177f5fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:06:24 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 18 Mar 2022 08:06:24 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Fri, 18 Mar 2022 08:06:25 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:53 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:54 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f242378e320c364d16b6d056493d7a6d02ccb0d0214cd43a092c09c2d196a89`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65503c01868a3fb0c4046bd568e0753952da09a77ee7b6babd5adf12c762ce`  
		Last Modified: Fri, 18 Mar 2022 08:09:14 GMT  
		Size: 108.6 MB (108637241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8944d50437c0d3db8b41c6f67af3c5a2fabccea9da92b293f4bbff80e5ca95`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 5.1 KB (5138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597d59a9a4245232eb602d93945953ad5217c782e5f3f62b4501905e68d54fdf`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:c8f68301981a7224cc9c063fc7a97b6ef13cfc4142b4871d1a35c95777ce96f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:cac49b06d95908bde09e2dcdadb4fa915c3fb3b0228e4e79e44f67b4024eb571
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155419411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05311a87aeb4d7f98b2726c39d4d29d6a174d20953a6d1ceaa236bfa177f5fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:06:24 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 18 Mar 2022 08:06:24 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Fri, 18 Mar 2022 08:06:25 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:53 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:54 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f242378e320c364d16b6d056493d7a6d02ccb0d0214cd43a092c09c2d196a89`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65503c01868a3fb0c4046bd568e0753952da09a77ee7b6babd5adf12c762ce`  
		Last Modified: Fri, 18 Mar 2022 08:09:14 GMT  
		Size: 108.6 MB (108637241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8944d50437c0d3db8b41c6f67af3c5a2fabccea9da92b293f4bbff80e5ca95`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 5.1 KB (5138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597d59a9a4245232eb602d93945953ad5217c782e5f3f62b4501905e68d54fdf`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:b8f8f1dca06f0f2bd4da7b7d3d0c98695afa55e495f274b279848b7eb786dec1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:90a57271a77fb51cb5e9062e6a4cc773c09ebb94693b382b728d4dc5b56d3344
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125156125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec092eca2e6f869c1b54d9098aad6f688b13e60bcbe5c5904100048ea30e0d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 18 Mar 2022 23:22:25 GMT
ADD file:19ae95221a518b3855b98aeb91f6c13f250d6caa59ee16bf155d73f7f5cdcc41 in / 
# Fri, 18 Mar 2022 23:22:26 GMT
CMD ["/bin/bash"]
# Sun, 20 Mar 2022 08:35:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Sun, 20 Mar 2022 08:35:33 GMT
ENV GOSU_VERSION=1.14
# Sun, 20 Mar 2022 08:35:37 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 20 Mar 2022 08:35:47 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sun, 20 Mar 2022 08:36:19 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sun, 20 Mar 2022 08:36:20 GMT
ENV MYSQL_MAJOR=5.7
# Sun, 20 Mar 2022 08:36:20 GMT
ENV MYSQL_VERSION=5.7.37-1.el7
# Sun, 20 Mar 2022 08:36:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sun, 20 Mar 2022 08:36:33 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Sun, 20 Mar 2022 08:36:34 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sun, 20 Mar 2022 08:36:34 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el7
# Sun, 20 Mar 2022 08:36:51 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sun, 20 Mar 2022 08:36:51 GMT
VOLUME [/var/lib/mysql]
# Sun, 20 Mar 2022 08:36:52 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Sun, 20 Mar 2022 08:36:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Mar 2022 08:36:52 GMT
EXPOSE 3306 33060
# Sun, 20 Mar 2022 08:36:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fb9cda09c679c7a8d70feb22223b7546c2d4d46d555312571fa2e3cc65347d9b`  
		Last Modified: Fri, 18 Mar 2022 23:23:20 GMT  
		Size: 48.7 MB (48745506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d92a669ae78e0afaed3ce5d7163161e8474e15d2847ae5d9238d773c805576`  
		Last Modified: Sun, 20 Mar 2022 08:37:27 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfca26c0cabc2152239d9d72138b28ee3a1352202681c195ad2ae9a44a35af5`  
		Last Modified: Sun, 20 Mar 2022 08:37:25 GMT  
		Size: 930.2 KB (930229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de8369545cab0fde8edb54d4280763d4ee1de6dfc159d36d14fb7838ba79d2`  
		Last Modified: Sun, 20 Mar 2022 08:37:26 GMT  
		Size: 3.7 MB (3713941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf98060af6cd1ba7d59edef4a89d04b75b819c6acb45de8350876db42877cb1f`  
		Last Modified: Sun, 20 Mar 2022 08:37:25 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abb0a38f4d7a31ace7a425d81577b64f34f1b662edb818e49c8f96cd974857`  
		Last Modified: Sun, 20 Mar 2022 08:37:23 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cab76a4536462713131d2b807d18360174f99ae81d5c415c68784df1e105eaf`  
		Last Modified: Sun, 20 Mar 2022 08:37:27 GMT  
		Size: 25.4 MB (25446301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0444456e33532f83e529c8c5526778a9ff87c60f334af9ed449ec94903fa4e40`  
		Last Modified: Sun, 20 Mar 2022 08:37:23 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9616457d9652fc11c5b9fd8f772a6d20a93aa805dc2a1c86e25671bad6e94eec`  
		Last Modified: Sun, 20 Mar 2022 08:37:31 GMT  
		Size: 46.3 MB (46310641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60c87db894a953c328163baa113579d7555cf47f8daf5ef088fae109065cbe`  
		Last Modified: Sun, 20 Mar 2022 08:37:23 GMT  
		Size: 5.1 KB (5138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.37`

```console
$ docker pull mysql@sha256:c8f68301981a7224cc9c063fc7a97b6ef13cfc4142b4871d1a35c95777ce96f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.37` - linux; amd64

```console
$ docker pull mysql@sha256:cac49b06d95908bde09e2dcdadb4fa915c3fb3b0228e4e79e44f67b4024eb571
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155419411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05311a87aeb4d7f98b2726c39d4d29d6a174d20953a6d1ceaa236bfa177f5fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:06:24 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 18 Mar 2022 08:06:24 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Fri, 18 Mar 2022 08:06:25 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:53 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:54 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f242378e320c364d16b6d056493d7a6d02ccb0d0214cd43a092c09c2d196a89`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65503c01868a3fb0c4046bd568e0753952da09a77ee7b6babd5adf12c762ce`  
		Last Modified: Fri, 18 Mar 2022 08:09:14 GMT  
		Size: 108.6 MB (108637241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8944d50437c0d3db8b41c6f67af3c5a2fabccea9da92b293f4bbff80e5ca95`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 5.1 KB (5138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597d59a9a4245232eb602d93945953ad5217c782e5f3f62b4501905e68d54fdf`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.37-debian`

```console
$ docker pull mysql@sha256:c8f68301981a7224cc9c063fc7a97b6ef13cfc4142b4871d1a35c95777ce96f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.37-debian` - linux; amd64

```console
$ docker pull mysql@sha256:cac49b06d95908bde09e2dcdadb4fa915c3fb3b0228e4e79e44f67b4024eb571
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155419411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05311a87aeb4d7f98b2726c39d4d29d6a174d20953a6d1ceaa236bfa177f5fb6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:06:24 GMT
ENV MYSQL_MAJOR=5.7
# Fri, 18 Mar 2022 08:06:24 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Fri, 18 Mar 2022 08:06:25 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:52 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:53 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:54 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f242378e320c364d16b6d056493d7a6d02ccb0d0214cd43a092c09c2d196a89`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65503c01868a3fb0c4046bd568e0753952da09a77ee7b6babd5adf12c762ce`  
		Last Modified: Fri, 18 Mar 2022 08:09:14 GMT  
		Size: 108.6 MB (108637241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8944d50437c0d3db8b41c6f67af3c5a2fabccea9da92b293f4bbff80e5ca95`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 5.1 KB (5138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597d59a9a4245232eb602d93945953ad5217c782e5f3f62b4501905e68d54fdf`  
		Last Modified: Fri, 18 Mar 2022 08:08:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.37-oracle`

```console
$ docker pull mysql@sha256:b8f8f1dca06f0f2bd4da7b7d3d0c98695afa55e495f274b279848b7eb786dec1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.37-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:90a57271a77fb51cb5e9062e6a4cc773c09ebb94693b382b728d4dc5b56d3344
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125156125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ec092eca2e6f869c1b54d9098aad6f688b13e60bcbe5c5904100048ea30e0d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 18 Mar 2022 23:22:25 GMT
ADD file:19ae95221a518b3855b98aeb91f6c13f250d6caa59ee16bf155d73f7f5cdcc41 in / 
# Fri, 18 Mar 2022 23:22:26 GMT
CMD ["/bin/bash"]
# Sun, 20 Mar 2022 08:35:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Sun, 20 Mar 2022 08:35:33 GMT
ENV GOSU_VERSION=1.14
# Sun, 20 Mar 2022 08:35:37 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 20 Mar 2022 08:35:47 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Sun, 20 Mar 2022 08:36:19 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sun, 20 Mar 2022 08:36:20 GMT
ENV MYSQL_MAJOR=5.7
# Sun, 20 Mar 2022 08:36:20 GMT
ENV MYSQL_VERSION=5.7.37-1.el7
# Sun, 20 Mar 2022 08:36:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sun, 20 Mar 2022 08:36:33 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Sun, 20 Mar 2022 08:36:34 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sun, 20 Mar 2022 08:36:34 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el7
# Sun, 20 Mar 2022 08:36:51 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Sun, 20 Mar 2022 08:36:51 GMT
VOLUME [/var/lib/mysql]
# Sun, 20 Mar 2022 08:36:52 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Sun, 20 Mar 2022 08:36:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Mar 2022 08:36:52 GMT
EXPOSE 3306 33060
# Sun, 20 Mar 2022 08:36:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fb9cda09c679c7a8d70feb22223b7546c2d4d46d555312571fa2e3cc65347d9b`  
		Last Modified: Fri, 18 Mar 2022 23:23:20 GMT  
		Size: 48.7 MB (48745506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d92a669ae78e0afaed3ce5d7163161e8474e15d2847ae5d9238d773c805576`  
		Last Modified: Sun, 20 Mar 2022 08:37:27 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfca26c0cabc2152239d9d72138b28ee3a1352202681c195ad2ae9a44a35af5`  
		Last Modified: Sun, 20 Mar 2022 08:37:25 GMT  
		Size: 930.2 KB (930229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de8369545cab0fde8edb54d4280763d4ee1de6dfc159d36d14fb7838ba79d2`  
		Last Modified: Sun, 20 Mar 2022 08:37:26 GMT  
		Size: 3.7 MB (3713941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf98060af6cd1ba7d59edef4a89d04b75b819c6acb45de8350876db42877cb1f`  
		Last Modified: Sun, 20 Mar 2022 08:37:25 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0abb0a38f4d7a31ace7a425d81577b64f34f1b662edb818e49c8f96cd974857`  
		Last Modified: Sun, 20 Mar 2022 08:37:23 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cab76a4536462713131d2b807d18360174f99ae81d5c415c68784df1e105eaf`  
		Last Modified: Sun, 20 Mar 2022 08:37:27 GMT  
		Size: 25.4 MB (25446301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0444456e33532f83e529c8c5526778a9ff87c60f334af9ed449ec94903fa4e40`  
		Last Modified: Sun, 20 Mar 2022 08:37:23 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9616457d9652fc11c5b9fd8f772a6d20a93aa805dc2a1c86e25671bad6e94eec`  
		Last Modified: Sun, 20 Mar 2022 08:37:31 GMT  
		Size: 46.3 MB (46310641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60c87db894a953c328163baa113579d7555cf47f8daf5ef088fae109065cbe`  
		Last Modified: Sun, 20 Mar 2022 08:37:23 GMT  
		Size: 5.1 KB (5138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:b2ae0f527005d99bacdf3a220958ed171e1eb0676377174f0323e0a10912408a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:00f9eb474bf3c508d79292234abc60dae082290445f44e38d9fcd844c2cd3372
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154588164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562c9bc24a0883226e994aabbd09fcb5621a4eadb510df749bc6dac40fa991e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:05:46 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 18 Mar 2022 08:05:47 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Fri, 18 Mar 2022 08:05:48 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:12 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:12 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 18 Mar 2022 08:06:12 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:14 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aa1710465f892ce62ad802679f4052567ab6da737d520da7f8a01f6251774d`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2d5722b8f34e9bf522099069d23bfbccfdb49063febf5d440f242fa89e57b0`  
		Last Modified: Fri, 18 Mar 2022 08:08:22 GMT  
		Size: 107.8 MB (107805152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a246e8d7cac973ac8c6dbf8a9d2c7c15c95ee700602d152f56194331e8a2a8f`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f834692d7cccae00681493349f623ffc62226e8a4af1e6ce0b08799e4a8b670`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 5.1 KB (5137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a374095680229f498cd512f25bc465fe563353f70ea395cc9eb4709f0177e5f1`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:b2ae0f527005d99bacdf3a220958ed171e1eb0676377174f0323e0a10912408a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:00f9eb474bf3c508d79292234abc60dae082290445f44e38d9fcd844c2cd3372
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154588164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562c9bc24a0883226e994aabbd09fcb5621a4eadb510df749bc6dac40fa991e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:05:46 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 18 Mar 2022 08:05:47 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Fri, 18 Mar 2022 08:05:48 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:12 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:12 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 18 Mar 2022 08:06:12 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:14 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aa1710465f892ce62ad802679f4052567ab6da737d520da7f8a01f6251774d`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2d5722b8f34e9bf522099069d23bfbccfdb49063febf5d440f242fa89e57b0`  
		Last Modified: Fri, 18 Mar 2022 08:08:22 GMT  
		Size: 107.8 MB (107805152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a246e8d7cac973ac8c6dbf8a9d2c7c15c95ee700602d152f56194331e8a2a8f`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f834692d7cccae00681493349f623ffc62226e8a4af1e6ce0b08799e4a8b670`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 5.1 KB (5137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a374095680229f498cd512f25bc465fe563353f70ea395cc9eb4709f0177e5f1`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:5aeabca77ff42a3e47dec06f38546a7bcfce2f851ff967355201bf36fc072682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:7393ba5c8671f58923b3798cf4bf1be4143830bd7d42f656befa3eade6d862b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133138390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396873955d6abc41308a7d35c3a1d23c775d7f13231a126848c73ce736f388e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 01:39:10 GMT
ADD file:c0f0a367bc612431ac9286b506fef5505e0b5f3969515486d8052ec381524261 in / 
# Thu, 24 Mar 2022 01:39:10 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 02:12:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 24 Mar 2022 02:12:04 GMT
ENV GOSU_VERSION=1.14
# Thu, 24 Mar 2022 02:12:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 24 Mar 2022 02:12:26 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 24 Mar 2022 02:12:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 24 Mar 2022 02:12:27 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 24 Mar 2022 02:12:27 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 02:12:28 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 24 Mar 2022 02:12:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 24 Mar 2022 02:12:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 24 Mar 2022 02:12:53 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 02:13:23 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 24 Mar 2022 02:13:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Mar 2022 02:13:24 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Thu, 24 Mar 2022 02:13:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 02:13:24 GMT
EXPOSE 3306 33060
# Thu, 24 Mar 2022 02:13:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a9d3d14d30b79ab021a558da3520be505bd2c5ab0f4c85aa07a3ed43524cea2f`  
		Last Modified: Thu, 24 Mar 2022 01:40:02 GMT  
		Size: 42.1 MB (42111482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c34c1c3d334fb2ab9c8d9c0195c46a22a08dc4d53f5cd8260dfa8c9130527c`  
		Last Modified: Thu, 24 Mar 2022 02:13:59 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edd8203272bf73c540c0edcdca1c2668dba76d53fed2a0ab5e67da19b7afe8c`  
		Last Modified: Thu, 24 Mar 2022 02:13:58 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4579ce2fbc2e8b1f50e6db4baccf038f1339415e4e4f205b6525ac976c896d`  
		Last Modified: Thu, 24 Mar 2022 02:13:58 GMT  
		Size: 4.5 MB (4546975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fbf1e34da756947373b1c081a452ca1bd648aee10625d68f255dfaa626c016`  
		Last Modified: Thu, 24 Mar 2022 02:13:57 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e1e95a4b5094db5db1154008980c898c0715849fbc8c4a5fc3dbed6073c2ef`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0074abeebc046de5186ef3d222c170beb09629607dd93bfce85be128a9a07633`  
		Last Modified: Thu, 24 Mar 2022 02:14:03 GMT  
		Size: 47.3 MB (47267258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c727cb58a0450cb56a6d163e0b5418430e30f7c276592763809016e6f7e04f3e`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fb1a877d961ee9a8d5ee2171e6167ca917f03075cda3e6d49e11ce5bc06cba`  
		Last Modified: Thu, 24 Mar 2022 02:14:02 GMT  
		Size: 38.3 MB (38274331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386346d38ca10d69f485b26793e5ba51e680934d8528ca250b7829a645a7d371`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:e9b456391b4bb798292b6a959f0d3a992911fc1f9c21cb1bee563096d9015f6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141172027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b353a72fcab60e6c13412fdafe5840a37e7dad38f5c36f7374eff8b8321151`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 18 Mar 2022 00:35:35 GMT
ADD file:b16af05882bd38ac02b1f1cba2cc7e80bfbe467ce57f3cf35f1f5a551cee90fa in / 
# Fri, 18 Mar 2022 00:35:36 GMT
CMD ["/bin/bash"]
# Sat, 19 Mar 2022 14:48:31 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Sat, 19 Mar 2022 14:48:32 GMT
ENV GOSU_VERSION=1.14
# Sat, 19 Mar 2022 14:48:35 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 14:49:02 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 19 Mar 2022 14:49:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 19 Mar 2022 14:49:47 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 19 Mar 2022 14:49:48 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Sat, 19 Mar 2022 14:49:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 19 Mar 2022 14:50:16 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Sat, 19 Mar 2022 14:50:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 19 Mar 2022 14:50:17 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Sat, 19 Mar 2022 14:50:46 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 19 Mar 2022 14:50:46 GMT
VOLUME [/var/lib/mysql]
# Sat, 19 Mar 2022 14:50:48 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Sat, 19 Mar 2022 14:50:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 14:50:49 GMT
EXPOSE 3306 33060
# Sat, 19 Mar 2022 14:50:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2f8e506fd7c6683f24250871efec36e3fe21cc71090a2f5c59dccdcdfeed2311`  
		Last Modified: Fri, 18 Mar 2022 00:36:38 GMT  
		Size: 42.0 MB (42017883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2e303329ed7fcb9aeb4e6a5e5e8ff70c5ecaca6b4004efe7c5538f98ae073e`  
		Last Modified: Sat, 19 Mar 2022 14:51:14 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43a54926eb5a7901c559b6766eb23666ade02e931708faf2888edadac9e1851`  
		Last Modified: Sat, 19 Mar 2022 14:51:13 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0039e24d8493013955f1061869d44fbdb472434d801986ac8140f0b1846bf4a`  
		Last Modified: Sat, 19 Mar 2022 14:51:12 GMT  
		Size: 4.4 MB (4376516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d112a79f85ef077e50966e6ff296393952c4e854cabca838a2ae8ea52346dd`  
		Last Modified: Sat, 19 Mar 2022 14:51:12 GMT  
		Size: 2.6 KB (2610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a816874cae3d0e7af62a465c20b10528a92dedfae97f28912f66a1e05d2eb35`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cf3e7c1e5610eed17336f2c459440bddfc67726e3c7fb87fafa6d6b69621d5`  
		Last Modified: Sat, 19 Mar 2022 14:51:17 GMT  
		Size: 53.4 MB (53429849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd2d8bfe6537a1ff984d2f0af8a1ca0efeb31774cec4a12f966f708d51cb479`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380e2f8b0a3606c651c20ab98460614d53fb50d4b9a9f7b33eff69eebc508ab1`  
		Last Modified: Sat, 19 Mar 2022 14:51:17 GMT  
		Size: 40.5 MB (40481210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9d4712db09dae7f88b55a0497883dc40d43f805f6a22a8c289b92a5a6a5398`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:b2ae0f527005d99bacdf3a220958ed171e1eb0676377174f0323e0a10912408a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:00f9eb474bf3c508d79292234abc60dae082290445f44e38d9fcd844c2cd3372
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154588164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562c9bc24a0883226e994aabbd09fcb5621a4eadb510df749bc6dac40fa991e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:05:46 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 18 Mar 2022 08:05:47 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Fri, 18 Mar 2022 08:05:48 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:12 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:12 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 18 Mar 2022 08:06:12 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:14 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aa1710465f892ce62ad802679f4052567ab6da737d520da7f8a01f6251774d`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2d5722b8f34e9bf522099069d23bfbccfdb49063febf5d440f242fa89e57b0`  
		Last Modified: Fri, 18 Mar 2022 08:08:22 GMT  
		Size: 107.8 MB (107805152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a246e8d7cac973ac8c6dbf8a9d2c7c15c95ee700602d152f56194331e8a2a8f`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f834692d7cccae00681493349f623ffc62226e8a4af1e6ce0b08799e4a8b670`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 5.1 KB (5137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a374095680229f498cd512f25bc465fe563353f70ea395cc9eb4709f0177e5f1`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:b2ae0f527005d99bacdf3a220958ed171e1eb0676377174f0323e0a10912408a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:00f9eb474bf3c508d79292234abc60dae082290445f44e38d9fcd844c2cd3372
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154588164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562c9bc24a0883226e994aabbd09fcb5621a4eadb510df749bc6dac40fa991e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:05:46 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 18 Mar 2022 08:05:47 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Fri, 18 Mar 2022 08:05:48 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:12 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:12 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 18 Mar 2022 08:06:12 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:14 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aa1710465f892ce62ad802679f4052567ab6da737d520da7f8a01f6251774d`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2d5722b8f34e9bf522099069d23bfbccfdb49063febf5d440f242fa89e57b0`  
		Last Modified: Fri, 18 Mar 2022 08:08:22 GMT  
		Size: 107.8 MB (107805152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a246e8d7cac973ac8c6dbf8a9d2c7c15c95ee700602d152f56194331e8a2a8f`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f834692d7cccae00681493349f623ffc62226e8a4af1e6ce0b08799e4a8b670`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 5.1 KB (5137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a374095680229f498cd512f25bc465fe563353f70ea395cc9eb4709f0177e5f1`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:5aeabca77ff42a3e47dec06f38546a7bcfce2f851ff967355201bf36fc072682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:7393ba5c8671f58923b3798cf4bf1be4143830bd7d42f656befa3eade6d862b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133138390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396873955d6abc41308a7d35c3a1d23c775d7f13231a126848c73ce736f388e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 01:39:10 GMT
ADD file:c0f0a367bc612431ac9286b506fef5505e0b5f3969515486d8052ec381524261 in / 
# Thu, 24 Mar 2022 01:39:10 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 02:12:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 24 Mar 2022 02:12:04 GMT
ENV GOSU_VERSION=1.14
# Thu, 24 Mar 2022 02:12:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 24 Mar 2022 02:12:26 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 24 Mar 2022 02:12:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 24 Mar 2022 02:12:27 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 24 Mar 2022 02:12:27 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 02:12:28 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 24 Mar 2022 02:12:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 24 Mar 2022 02:12:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 24 Mar 2022 02:12:53 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 02:13:23 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 24 Mar 2022 02:13:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Mar 2022 02:13:24 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Thu, 24 Mar 2022 02:13:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 02:13:24 GMT
EXPOSE 3306 33060
# Thu, 24 Mar 2022 02:13:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a9d3d14d30b79ab021a558da3520be505bd2c5ab0f4c85aa07a3ed43524cea2f`  
		Last Modified: Thu, 24 Mar 2022 01:40:02 GMT  
		Size: 42.1 MB (42111482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c34c1c3d334fb2ab9c8d9c0195c46a22a08dc4d53f5cd8260dfa8c9130527c`  
		Last Modified: Thu, 24 Mar 2022 02:13:59 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edd8203272bf73c540c0edcdca1c2668dba76d53fed2a0ab5e67da19b7afe8c`  
		Last Modified: Thu, 24 Mar 2022 02:13:58 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4579ce2fbc2e8b1f50e6db4baccf038f1339415e4e4f205b6525ac976c896d`  
		Last Modified: Thu, 24 Mar 2022 02:13:58 GMT  
		Size: 4.5 MB (4546975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fbf1e34da756947373b1c081a452ca1bd648aee10625d68f255dfaa626c016`  
		Last Modified: Thu, 24 Mar 2022 02:13:57 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e1e95a4b5094db5db1154008980c898c0715849fbc8c4a5fc3dbed6073c2ef`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0074abeebc046de5186ef3d222c170beb09629607dd93bfce85be128a9a07633`  
		Last Modified: Thu, 24 Mar 2022 02:14:03 GMT  
		Size: 47.3 MB (47267258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c727cb58a0450cb56a6d163e0b5418430e30f7c276592763809016e6f7e04f3e`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fb1a877d961ee9a8d5ee2171e6167ca917f03075cda3e6d49e11ce5bc06cba`  
		Last Modified: Thu, 24 Mar 2022 02:14:02 GMT  
		Size: 38.3 MB (38274331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386346d38ca10d69f485b26793e5ba51e680934d8528ca250b7829a645a7d371`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:e9b456391b4bb798292b6a959f0d3a992911fc1f9c21cb1bee563096d9015f6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141172027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b353a72fcab60e6c13412fdafe5840a37e7dad38f5c36f7374eff8b8321151`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 18 Mar 2022 00:35:35 GMT
ADD file:b16af05882bd38ac02b1f1cba2cc7e80bfbe467ce57f3cf35f1f5a551cee90fa in / 
# Fri, 18 Mar 2022 00:35:36 GMT
CMD ["/bin/bash"]
# Sat, 19 Mar 2022 14:48:31 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Sat, 19 Mar 2022 14:48:32 GMT
ENV GOSU_VERSION=1.14
# Sat, 19 Mar 2022 14:48:35 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 14:49:02 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 19 Mar 2022 14:49:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 19 Mar 2022 14:49:47 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 19 Mar 2022 14:49:48 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Sat, 19 Mar 2022 14:49:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 19 Mar 2022 14:50:16 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Sat, 19 Mar 2022 14:50:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 19 Mar 2022 14:50:17 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Sat, 19 Mar 2022 14:50:46 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 19 Mar 2022 14:50:46 GMT
VOLUME [/var/lib/mysql]
# Sat, 19 Mar 2022 14:50:48 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Sat, 19 Mar 2022 14:50:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 14:50:49 GMT
EXPOSE 3306 33060
# Sat, 19 Mar 2022 14:50:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2f8e506fd7c6683f24250871efec36e3fe21cc71090a2f5c59dccdcdfeed2311`  
		Last Modified: Fri, 18 Mar 2022 00:36:38 GMT  
		Size: 42.0 MB (42017883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2e303329ed7fcb9aeb4e6a5e5e8ff70c5ecaca6b4004efe7c5538f98ae073e`  
		Last Modified: Sat, 19 Mar 2022 14:51:14 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43a54926eb5a7901c559b6766eb23666ade02e931708faf2888edadac9e1851`  
		Last Modified: Sat, 19 Mar 2022 14:51:13 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0039e24d8493013955f1061869d44fbdb472434d801986ac8140f0b1846bf4a`  
		Last Modified: Sat, 19 Mar 2022 14:51:12 GMT  
		Size: 4.4 MB (4376516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d112a79f85ef077e50966e6ff296393952c4e854cabca838a2ae8ea52346dd`  
		Last Modified: Sat, 19 Mar 2022 14:51:12 GMT  
		Size: 2.6 KB (2610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a816874cae3d0e7af62a465c20b10528a92dedfae97f28912f66a1e05d2eb35`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cf3e7c1e5610eed17336f2c459440bddfc67726e3c7fb87fafa6d6b69621d5`  
		Last Modified: Sat, 19 Mar 2022 14:51:17 GMT  
		Size: 53.4 MB (53429849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd2d8bfe6537a1ff984d2f0af8a1ca0efeb31774cec4a12f966f708d51cb479`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380e2f8b0a3606c651c20ab98460614d53fb50d4b9a9f7b33eff69eebc508ab1`  
		Last Modified: Sat, 19 Mar 2022 14:51:17 GMT  
		Size: 40.5 MB (40481210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9d4712db09dae7f88b55a0497883dc40d43f805f6a22a8c289b92a5a6a5398`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.28`

```console
$ docker pull mysql@sha256:b2ae0f527005d99bacdf3a220958ed171e1eb0676377174f0323e0a10912408a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.28` - linux; amd64

```console
$ docker pull mysql@sha256:00f9eb474bf3c508d79292234abc60dae082290445f44e38d9fcd844c2cd3372
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154588164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562c9bc24a0883226e994aabbd09fcb5621a4eadb510df749bc6dac40fa991e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:05:46 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 18 Mar 2022 08:05:47 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Fri, 18 Mar 2022 08:05:48 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:12 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:12 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 18 Mar 2022 08:06:12 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:14 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aa1710465f892ce62ad802679f4052567ab6da737d520da7f8a01f6251774d`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2d5722b8f34e9bf522099069d23bfbccfdb49063febf5d440f242fa89e57b0`  
		Last Modified: Fri, 18 Mar 2022 08:08:22 GMT  
		Size: 107.8 MB (107805152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a246e8d7cac973ac8c6dbf8a9d2c7c15c95ee700602d152f56194331e8a2a8f`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f834692d7cccae00681493349f623ffc62226e8a4af1e6ce0b08799e4a8b670`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 5.1 KB (5137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a374095680229f498cd512f25bc465fe563353f70ea395cc9eb4709f0177e5f1`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.28-debian`

```console
$ docker pull mysql@sha256:b2ae0f527005d99bacdf3a220958ed171e1eb0676377174f0323e0a10912408a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.28-debian` - linux; amd64

```console
$ docker pull mysql@sha256:00f9eb474bf3c508d79292234abc60dae082290445f44e38d9fcd844c2cd3372
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154588164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562c9bc24a0883226e994aabbd09fcb5621a4eadb510df749bc6dac40fa991e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:05:46 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 18 Mar 2022 08:05:47 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Fri, 18 Mar 2022 08:05:48 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:12 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:12 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 18 Mar 2022 08:06:12 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:14 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aa1710465f892ce62ad802679f4052567ab6da737d520da7f8a01f6251774d`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2d5722b8f34e9bf522099069d23bfbccfdb49063febf5d440f242fa89e57b0`  
		Last Modified: Fri, 18 Mar 2022 08:08:22 GMT  
		Size: 107.8 MB (107805152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a246e8d7cac973ac8c6dbf8a9d2c7c15c95ee700602d152f56194331e8a2a8f`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f834692d7cccae00681493349f623ffc62226e8a4af1e6ce0b08799e4a8b670`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 5.1 KB (5137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a374095680229f498cd512f25bc465fe563353f70ea395cc9eb4709f0177e5f1`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.28-oracle`

```console
$ docker pull mysql@sha256:5aeabca77ff42a3e47dec06f38546a7bcfce2f851ff967355201bf36fc072682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.28-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:7393ba5c8671f58923b3798cf4bf1be4143830bd7d42f656befa3eade6d862b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133138390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396873955d6abc41308a7d35c3a1d23c775d7f13231a126848c73ce736f388e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 01:39:10 GMT
ADD file:c0f0a367bc612431ac9286b506fef5505e0b5f3969515486d8052ec381524261 in / 
# Thu, 24 Mar 2022 01:39:10 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 02:12:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 24 Mar 2022 02:12:04 GMT
ENV GOSU_VERSION=1.14
# Thu, 24 Mar 2022 02:12:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 24 Mar 2022 02:12:26 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 24 Mar 2022 02:12:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 24 Mar 2022 02:12:27 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 24 Mar 2022 02:12:27 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 02:12:28 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 24 Mar 2022 02:12:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 24 Mar 2022 02:12:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 24 Mar 2022 02:12:53 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 02:13:23 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 24 Mar 2022 02:13:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Mar 2022 02:13:24 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Thu, 24 Mar 2022 02:13:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 02:13:24 GMT
EXPOSE 3306 33060
# Thu, 24 Mar 2022 02:13:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a9d3d14d30b79ab021a558da3520be505bd2c5ab0f4c85aa07a3ed43524cea2f`  
		Last Modified: Thu, 24 Mar 2022 01:40:02 GMT  
		Size: 42.1 MB (42111482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c34c1c3d334fb2ab9c8d9c0195c46a22a08dc4d53f5cd8260dfa8c9130527c`  
		Last Modified: Thu, 24 Mar 2022 02:13:59 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edd8203272bf73c540c0edcdca1c2668dba76d53fed2a0ab5e67da19b7afe8c`  
		Last Modified: Thu, 24 Mar 2022 02:13:58 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4579ce2fbc2e8b1f50e6db4baccf038f1339415e4e4f205b6525ac976c896d`  
		Last Modified: Thu, 24 Mar 2022 02:13:58 GMT  
		Size: 4.5 MB (4546975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fbf1e34da756947373b1c081a452ca1bd648aee10625d68f255dfaa626c016`  
		Last Modified: Thu, 24 Mar 2022 02:13:57 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e1e95a4b5094db5db1154008980c898c0715849fbc8c4a5fc3dbed6073c2ef`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0074abeebc046de5186ef3d222c170beb09629607dd93bfce85be128a9a07633`  
		Last Modified: Thu, 24 Mar 2022 02:14:03 GMT  
		Size: 47.3 MB (47267258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c727cb58a0450cb56a6d163e0b5418430e30f7c276592763809016e6f7e04f3e`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fb1a877d961ee9a8d5ee2171e6167ca917f03075cda3e6d49e11ce5bc06cba`  
		Last Modified: Thu, 24 Mar 2022 02:14:02 GMT  
		Size: 38.3 MB (38274331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386346d38ca10d69f485b26793e5ba51e680934d8528ca250b7829a645a7d371`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.28-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:e9b456391b4bb798292b6a959f0d3a992911fc1f9c21cb1bee563096d9015f6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141172027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b353a72fcab60e6c13412fdafe5840a37e7dad38f5c36f7374eff8b8321151`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 18 Mar 2022 00:35:35 GMT
ADD file:b16af05882bd38ac02b1f1cba2cc7e80bfbe467ce57f3cf35f1f5a551cee90fa in / 
# Fri, 18 Mar 2022 00:35:36 GMT
CMD ["/bin/bash"]
# Sat, 19 Mar 2022 14:48:31 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Sat, 19 Mar 2022 14:48:32 GMT
ENV GOSU_VERSION=1.14
# Sat, 19 Mar 2022 14:48:35 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 14:49:02 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 19 Mar 2022 14:49:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 19 Mar 2022 14:49:47 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 19 Mar 2022 14:49:48 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Sat, 19 Mar 2022 14:49:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 19 Mar 2022 14:50:16 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Sat, 19 Mar 2022 14:50:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 19 Mar 2022 14:50:17 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Sat, 19 Mar 2022 14:50:46 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 19 Mar 2022 14:50:46 GMT
VOLUME [/var/lib/mysql]
# Sat, 19 Mar 2022 14:50:48 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Sat, 19 Mar 2022 14:50:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 14:50:49 GMT
EXPOSE 3306 33060
# Sat, 19 Mar 2022 14:50:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2f8e506fd7c6683f24250871efec36e3fe21cc71090a2f5c59dccdcdfeed2311`  
		Last Modified: Fri, 18 Mar 2022 00:36:38 GMT  
		Size: 42.0 MB (42017883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2e303329ed7fcb9aeb4e6a5e5e8ff70c5ecaca6b4004efe7c5538f98ae073e`  
		Last Modified: Sat, 19 Mar 2022 14:51:14 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43a54926eb5a7901c559b6766eb23666ade02e931708faf2888edadac9e1851`  
		Last Modified: Sat, 19 Mar 2022 14:51:13 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0039e24d8493013955f1061869d44fbdb472434d801986ac8140f0b1846bf4a`  
		Last Modified: Sat, 19 Mar 2022 14:51:12 GMT  
		Size: 4.4 MB (4376516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d112a79f85ef077e50966e6ff296393952c4e854cabca838a2ae8ea52346dd`  
		Last Modified: Sat, 19 Mar 2022 14:51:12 GMT  
		Size: 2.6 KB (2610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a816874cae3d0e7af62a465c20b10528a92dedfae97f28912f66a1e05d2eb35`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cf3e7c1e5610eed17336f2c459440bddfc67726e3c7fb87fafa6d6b69621d5`  
		Last Modified: Sat, 19 Mar 2022 14:51:17 GMT  
		Size: 53.4 MB (53429849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd2d8bfe6537a1ff984d2f0af8a1ca0efeb31774cec4a12f966f708d51cb479`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380e2f8b0a3606c651c20ab98460614d53fb50d4b9a9f7b33eff69eebc508ab1`  
		Last Modified: Sat, 19 Mar 2022 14:51:17 GMT  
		Size: 40.5 MB (40481210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9d4712db09dae7f88b55a0497883dc40d43f805f6a22a8c289b92a5a6a5398`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:b2ae0f527005d99bacdf3a220958ed171e1eb0676377174f0323e0a10912408a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:00f9eb474bf3c508d79292234abc60dae082290445f44e38d9fcd844c2cd3372
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154588164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562c9bc24a0883226e994aabbd09fcb5621a4eadb510df749bc6dac40fa991e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:05:46 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 18 Mar 2022 08:05:47 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Fri, 18 Mar 2022 08:05:48 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:12 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:12 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 18 Mar 2022 08:06:12 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:14 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aa1710465f892ce62ad802679f4052567ab6da737d520da7f8a01f6251774d`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2d5722b8f34e9bf522099069d23bfbccfdb49063febf5d440f242fa89e57b0`  
		Last Modified: Fri, 18 Mar 2022 08:08:22 GMT  
		Size: 107.8 MB (107805152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a246e8d7cac973ac8c6dbf8a9d2c7c15c95ee700602d152f56194331e8a2a8f`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f834692d7cccae00681493349f623ffc62226e8a4af1e6ce0b08799e4a8b670`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 5.1 KB (5137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a374095680229f498cd512f25bc465fe563353f70ea395cc9eb4709f0177e5f1`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:b2ae0f527005d99bacdf3a220958ed171e1eb0676377174f0323e0a10912408a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:00f9eb474bf3c508d79292234abc60dae082290445f44e38d9fcd844c2cd3372
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154588164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562c9bc24a0883226e994aabbd09fcb5621a4eadb510df749bc6dac40fa991e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:05:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Mar 2022 08:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:17 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 08:05:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 08:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 08:05:46 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 18 Mar 2022 08:05:47 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Fri, 18 Mar 2022 08:05:48 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 18 Mar 2022 08:06:11 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 18 Mar 2022 08:06:12 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Mar 2022 08:06:12 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 18 Mar 2022 08:06:12 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:06:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 18 Mar 2022 08:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:14 GMT
EXPOSE 3306 33060
# Fri, 18 Mar 2022 08:06:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b610d88fd99d32cc566df2799696e4c382585071097a00051274edd5aba2a2`  
		Last Modified: Fri, 18 Mar 2022 08:08:01 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38567843b438528aec2e445daf0b2f45d468e92718c73612926e8b6c8f2ebe10`  
		Last Modified: Fri, 18 Mar 2022 08:08:02 GMT  
		Size: 4.2 MB (4179316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc423bf9558fc1c7102977e94d1f95331ff2b7e2e5e02e0a32346e1217ce4b3`  
		Last Modified: Fri, 18 Mar 2022 08:08:00 GMT  
		Size: 1.4 MB (1386669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8241dfe8280a8f86bacace41eda0644b04ee0696bd32e9a6b95bafd2d48f8b`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc662311610e8df5f42ff626b5db6d179f9c894c73ab0cccf719dd7848d5222a`  
		Last Modified: Fri, 18 Mar 2022 08:08:04 GMT  
		Size: 14.1 MB (14052414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9832d1192cf2fe8622425e18f9f868f2efbe0e78fe3724d999f3521ff2da8363`  
		Last Modified: Fri, 18 Mar 2022 08:07:59 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aa1710465f892ce62ad802679f4052567ab6da737d520da7f8a01f6251774d`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2d5722b8f34e9bf522099069d23bfbccfdb49063febf5d440f242fa89e57b0`  
		Last Modified: Fri, 18 Mar 2022 08:08:22 GMT  
		Size: 107.8 MB (107805152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a246e8d7cac973ac8c6dbf8a9d2c7c15c95ee700602d152f56194331e8a2a8f`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f834692d7cccae00681493349f623ffc62226e8a4af1e6ce0b08799e4a8b670`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 5.1 KB (5137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a374095680229f498cd512f25bc465fe563353f70ea395cc9eb4709f0177e5f1`  
		Last Modified: Fri, 18 Mar 2022 08:07:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:5aeabca77ff42a3e47dec06f38546a7bcfce2f851ff967355201bf36fc072682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:7393ba5c8671f58923b3798cf4bf1be4143830bd7d42f656befa3eade6d862b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133138390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396873955d6abc41308a7d35c3a1d23c775d7f13231a126848c73ce736f388e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 01:39:10 GMT
ADD file:c0f0a367bc612431ac9286b506fef5505e0b5f3969515486d8052ec381524261 in / 
# Thu, 24 Mar 2022 01:39:10 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 02:12:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 24 Mar 2022 02:12:04 GMT
ENV GOSU_VERSION=1.14
# Thu, 24 Mar 2022 02:12:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 24 Mar 2022 02:12:26 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 24 Mar 2022 02:12:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 24 Mar 2022 02:12:27 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 24 Mar 2022 02:12:27 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 02:12:28 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 24 Mar 2022 02:12:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 24 Mar 2022 02:12:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 24 Mar 2022 02:12:53 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 02:13:23 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 24 Mar 2022 02:13:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Mar 2022 02:13:24 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Thu, 24 Mar 2022 02:13:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 02:13:24 GMT
EXPOSE 3306 33060
# Thu, 24 Mar 2022 02:13:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a9d3d14d30b79ab021a558da3520be505bd2c5ab0f4c85aa07a3ed43524cea2f`  
		Last Modified: Thu, 24 Mar 2022 01:40:02 GMT  
		Size: 42.1 MB (42111482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c34c1c3d334fb2ab9c8d9c0195c46a22a08dc4d53f5cd8260dfa8c9130527c`  
		Last Modified: Thu, 24 Mar 2022 02:13:59 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edd8203272bf73c540c0edcdca1c2668dba76d53fed2a0ab5e67da19b7afe8c`  
		Last Modified: Thu, 24 Mar 2022 02:13:58 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4579ce2fbc2e8b1f50e6db4baccf038f1339415e4e4f205b6525ac976c896d`  
		Last Modified: Thu, 24 Mar 2022 02:13:58 GMT  
		Size: 4.5 MB (4546975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fbf1e34da756947373b1c081a452ca1bd648aee10625d68f255dfaa626c016`  
		Last Modified: Thu, 24 Mar 2022 02:13:57 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e1e95a4b5094db5db1154008980c898c0715849fbc8c4a5fc3dbed6073c2ef`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0074abeebc046de5186ef3d222c170beb09629607dd93bfce85be128a9a07633`  
		Last Modified: Thu, 24 Mar 2022 02:14:03 GMT  
		Size: 47.3 MB (47267258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c727cb58a0450cb56a6d163e0b5418430e30f7c276592763809016e6f7e04f3e`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fb1a877d961ee9a8d5ee2171e6167ca917f03075cda3e6d49e11ce5bc06cba`  
		Last Modified: Thu, 24 Mar 2022 02:14:02 GMT  
		Size: 38.3 MB (38274331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386346d38ca10d69f485b26793e5ba51e680934d8528ca250b7829a645a7d371`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:e9b456391b4bb798292b6a959f0d3a992911fc1f9c21cb1bee563096d9015f6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141172027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b353a72fcab60e6c13412fdafe5840a37e7dad38f5c36f7374eff8b8321151`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 18 Mar 2022 00:35:35 GMT
ADD file:b16af05882bd38ac02b1f1cba2cc7e80bfbe467ce57f3cf35f1f5a551cee90fa in / 
# Fri, 18 Mar 2022 00:35:36 GMT
CMD ["/bin/bash"]
# Sat, 19 Mar 2022 14:48:31 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Sat, 19 Mar 2022 14:48:32 GMT
ENV GOSU_VERSION=1.14
# Sat, 19 Mar 2022 14:48:35 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 14:49:02 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 19 Mar 2022 14:49:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 19 Mar 2022 14:49:47 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 19 Mar 2022 14:49:48 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Sat, 19 Mar 2022 14:49:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 19 Mar 2022 14:50:16 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Sat, 19 Mar 2022 14:50:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 19 Mar 2022 14:50:17 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Sat, 19 Mar 2022 14:50:46 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 19 Mar 2022 14:50:46 GMT
VOLUME [/var/lib/mysql]
# Sat, 19 Mar 2022 14:50:48 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Sat, 19 Mar 2022 14:50:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 14:50:49 GMT
EXPOSE 3306 33060
# Sat, 19 Mar 2022 14:50:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2f8e506fd7c6683f24250871efec36e3fe21cc71090a2f5c59dccdcdfeed2311`  
		Last Modified: Fri, 18 Mar 2022 00:36:38 GMT  
		Size: 42.0 MB (42017883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2e303329ed7fcb9aeb4e6a5e5e8ff70c5ecaca6b4004efe7c5538f98ae073e`  
		Last Modified: Sat, 19 Mar 2022 14:51:14 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43a54926eb5a7901c559b6766eb23666ade02e931708faf2888edadac9e1851`  
		Last Modified: Sat, 19 Mar 2022 14:51:13 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0039e24d8493013955f1061869d44fbdb472434d801986ac8140f0b1846bf4a`  
		Last Modified: Sat, 19 Mar 2022 14:51:12 GMT  
		Size: 4.4 MB (4376516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d112a79f85ef077e50966e6ff296393952c4e854cabca838a2ae8ea52346dd`  
		Last Modified: Sat, 19 Mar 2022 14:51:12 GMT  
		Size: 2.6 KB (2610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a816874cae3d0e7af62a465c20b10528a92dedfae97f28912f66a1e05d2eb35`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cf3e7c1e5610eed17336f2c459440bddfc67726e3c7fb87fafa6d6b69621d5`  
		Last Modified: Sat, 19 Mar 2022 14:51:17 GMT  
		Size: 53.4 MB (53429849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd2d8bfe6537a1ff984d2f0af8a1ca0efeb31774cec4a12f966f708d51cb479`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380e2f8b0a3606c651c20ab98460614d53fb50d4b9a9f7b33eff69eebc508ab1`  
		Last Modified: Sat, 19 Mar 2022 14:51:17 GMT  
		Size: 40.5 MB (40481210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9d4712db09dae7f88b55a0497883dc40d43f805f6a22a8c289b92a5a6a5398`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
