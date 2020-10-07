<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10.1`](#mariadb101)
-	[`mariadb:10.1.47`](#mariadb10147)
-	[`mariadb:10.1.47-bionic`](#mariadb10147-bionic)
-	[`mariadb:10.1-bionic`](#mariadb101-bionic)
-	[`mariadb:10.2`](#mariadb102)
-	[`mariadb:10.2.34`](#mariadb10234)
-	[`mariadb:10.2.34-bionic`](#mariadb10234-bionic)
-	[`mariadb:10.2-bionic`](#mariadb102-bionic)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3.25`](#mariadb10325)
-	[`mariadb:10.3.25-focal`](#mariadb10325-focal)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4.15`](#mariadb10415)
-	[`mariadb:10.4.15-focal`](#mariadb10415-focal)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5.6`](#mariadb1056)
-	[`mariadb:10.5.6-focal`](#mariadb1056-focal)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10-focal`](#mariadb10-focal)
-	[`mariadb:focal`](#mariadbfocal)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:9d27dd15564ba13a8ffa93beee20b39b7c14218c47ea296c6e11878a77962d12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:6955c063991fc6ee57fc0ba1b3b3de70408518df55af0c294323ff7d1ee974ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125549894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41fa9265d4dfb214f0a79ee919392687d09babc3522df21fce946292f9c8149c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:34:27 GMT
ADD file:da80f59399481ffc32f84353830dcf598f31a97785222e75d643bfb8a9aa14e7 in / 
# Fri, 25 Sep 2020 22:34:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:34:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:34:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:34:30 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:52:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:53:04 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:53:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:53:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:53:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:19 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:53:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:53:21 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 26 Sep 2020 00:53:21 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Sat, 26 Sep 2020 00:53:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:53:48 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:53:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:53:49 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:53:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:53:49 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:53:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d72e567cc804d0b637182ba23f8b9ffe101e753a39bf52cd4db6b89eb089f13b`  
		Last Modified: Fri, 25 Sep 2020 15:20:50 GMT  
		Size: 28.6 MB (28558050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3630e5ff08d73b6ec0e22736a5c8d2d666e7b568c16f6a4ffadf8c21b9b1ad`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a83d81d1f4f942d37e1f17195d9c519969ed3040fc3e444740b884e44dec33`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf2111ecf0efaa19887c07ce1ae8332ebff5775482731d8e524898d9fc07e23`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d64978a09242b12c715a8cfda3ce4ac4ef1e086016ccb32edb185f844363`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 5.5 MB (5488523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc9953bffb3c364d00df0e3961c569c5eebc2015cabee42cb7e0b33c4ba6891`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 1.3 MB (1324124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de429570dda5816121294e9251d2cf7f258f2a0c9fdf2a7ba9a7ebe56a763e83`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3652bc6ea9f9147ae99d11202e416c096df524bf3a64b6f483adb8d54e59a4a0`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 1.3 MB (1265989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4bf87041c8ad8ddf97dbbb645685d428963abc9d376dc413e6f7ee202af1ab`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb9bba22391ff2e85884b55109ea43a161c4bc348203f3a388ed71d94544a1c`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de10906fc5c385f1393d3e151fbb623b08796f6ffb8aacc998872c1d2e3805b`  
		Last Modified: Sat, 26 Sep 2020 00:59:06 GMT  
		Size: 88.9 MB (88902466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3a798c7a1f734389ff2ef70f8b27635b57c8cccb49f740e3bbce6c4992d01b`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0c0109b388d5a2b49159cfc84ef349261097968ef7143bd552cfa99297f215c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123202059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:715582b8771e15f883d2a7059abb63449fc21a84740b7c25adefe91051c4d7ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:59 GMT
ADD file:e1079b8987ad959c6a83dae1ea4446405953ab16899c693d57c6214ff888e688 in / 
# Fri, 25 Sep 2020 22:48:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:48:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:48:06 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:26:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:27:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:27:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:27:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:27:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:30 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:27:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:27:33 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Sep 2020 23:27:34 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Fri, 25 Sep 2020 23:27:36 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:28:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:28:13 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:28:14 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:28:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:28:15 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:28:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a25fe36305380fa444fa6bd15b622145ff6076e5b6f81168d6cb4c9fee725863`  
		Last Modified: Fri, 25 Sep 2020 08:25:35 GMT  
		Size: 27.2 MB (27160123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326fa3abf0610ea05b9deb392e05c6c86a7afed0c119987a8d920a2a8dceaffc`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b87601e0a324569be2cebc4c0b9981bd53925a9bee894fad57c93f9bd3d01`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a280fab3f6130dcd17011ffa4ee6cb14fd04623b4c1e16f378026844b8f428`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b33bb77d692ee1db553b82b566c91f41b6dbfd76e9ba9eaa444b7ca545fe6`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 5.5 MB (5456069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c36f1baced17c5bd6b814a182f023308e1b4cda8870bf91756041505870fa2a`  
		Last Modified: Fri, 25 Sep 2020 23:34:27 GMT  
		Size: 1.3 MB (1261421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a2b365d2a0b2769c317ffcde3ef8699d4d7c3256f95021f1da0d979006c1dc`  
		Last Modified: Fri, 25 Sep 2020 23:34:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f8ac108760bfd505fbfd1b252d7cea8e1c95895d04a6de0fb125d757c67f23`  
		Last Modified: Fri, 25 Sep 2020 23:34:25 GMT  
		Size: 1.3 MB (1265577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91718a6772cfde37e00ab454ab0fe8081399c122f22de9c2cc6b578dfe810cf6`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562cf16ec0a88e52ae3c5f14f4a083a1dd7273b805e0071f0f89c51e59048334`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6696e516bd6a98c3918decf8e7d83de51e39abe14588bb4126ea4835ff3da81`  
		Last Modified: Fri, 25 Sep 2020 23:34:49 GMT  
		Size: 88.0 MB (88048066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c1c05478213ecb540b9d3128078c6de920ca362b457bb22c70ba679b7932b`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d25388c779e56637ae42d217e4b826f491165a4d17d590c5d73333c68ef8c37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135600789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7c404662a55bba19439eed02cd8c4c40b348ba4646235804e46169051f2993`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:53:28 GMT
ADD file:5479628763eb7f8cd884270bc1e9bb40ce39f1fb3427e863b086511696fa8107 in / 
# Fri, 25 Sep 2020 23:53:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:54:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:54:31 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:13:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:13:26 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:14:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:14:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:14:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:14:59 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:15:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:15:09 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 26 Sep 2020 04:15:13 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Sat, 26 Sep 2020 04:15:19 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:18:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:18:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:18:16 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:18:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:18:23 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:18:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af5e190551614a549619ca2cb11a237bf566e7b0942eac80adaf05e21644ad12`  
		Last Modified: Sat, 26 Sep 2020 00:06:58 GMT  
		Size: 33.3 MB (33278058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dd7d43fa9f545a3f69e66ff00d1a2773213cdfc18d0c99a71bb1c40bbb1f8c`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1feb93b9aa176877a7ec845345f281fe28c37605e03363dd0fa489bf0bf10ee`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72de4183a4e4f8be028bd4096c22189718c23c7af3d8206f6119c7e672403f5b`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd855440835f9cbdc109164d975673b33c12064da301ac86019019bf4457e2a6`  
		Last Modified: Sat, 26 Sep 2020 04:34:10 GMT  
		Size: 6.7 MB (6668533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc681828d8ea74c541ead13581fa9a5b5aa4c9bd5f23a49edb457fbfef07fad`  
		Last Modified: Sat, 26 Sep 2020 04:34:03 GMT  
		Size: 1.2 MB (1243770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be85c8ddabd72fe111c44f1aa3f8c03e84ab9e12b95ecaf8e14bc19cd8ce63d6`  
		Last Modified: Sat, 26 Sep 2020 04:34:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333eecf00fdea344bb79b6958cbd01f130119d2a12a3b7bcb698262191b0faa`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.3 MB (1273578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b192cad172b5465b46c838d6ed65009da808af10327870e10ca3dc21dfabd797`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219ea6186c99102a7c952eabf22c03f79b9526307599b559a653375cba47467f`  
		Last Modified: Sat, 26 Sep 2020 04:33:55 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3620f102186fd21942b809f0f350a92a5d2206665bf4e1e78b2b4ad71a773101`  
		Last Modified: Sat, 26 Sep 2020 04:34:52 GMT  
		Size: 93.1 MB (93126036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661e28fa187e787cae957c2bc54772ad07a9afca94ecf7c488f10f19fc31d17d`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1`

```console
$ docker pull mariadb@sha256:ff77fd8f8156262c4db4075c2abaeca212a60765a91dc4814cc11060d66ff2f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1` - linux; amd64

```console
$ docker pull mariadb@sha256:f1b8db6f50310f74bfc6344d3a5882061cca0cc2c7bfadc7f0d393c96dd30cf5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113154815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ae24e47e14441d9c39f1c489fd14ec98c0c0146d36f6655cf63d5b84f0e4b54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:55:59 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:56:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:56:11 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:56:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:56:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:56:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:56:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:56:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:57:42 GMT
ENV MARIADB_MAJOR=10.1
# Sat, 26 Sep 2020 00:57:42 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Sat, 26 Sep 2020 00:57:42 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:58:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:58:14 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:58:14 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:58:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 00:58:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:58:15 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:58:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928020f0412e3eba561c742f10581acf4ca64971be9de7c21db53f9375ab82a0`  
		Last Modified: Sat, 26 Sep 2020 01:00:06 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b22d867bcc98722fa20b0feccc8434bed1423ea0d0080e6381ac6e12fd9832`  
		Last Modified: Sat, 26 Sep 2020 01:00:06 GMT  
		Size: 4.8 MB (4811571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5f9e2cc9e34fc162225c6bb7c8bb297112a362d456ad7900c14987c7835a26`  
		Last Modified: Sat, 26 Sep 2020 01:00:08 GMT  
		Size: 1.3 MB (1327238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c978fcde13344ce411d42bad561de5cebf5743c87cc6fc33b25872f6b929eca6`  
		Last Modified: Sat, 26 Sep 2020 01:00:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4d9e93f2fbf36cbabecdede7edbe2ab3fb653f34d8e92e819c9c06ddd3ffa8`  
		Last Modified: Sat, 26 Sep 2020 01:00:01 GMT  
		Size: 930.6 KB (930554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d8ee36e7ef936f57d1a918f47f7cad0121f275966dee17b78458c4c51cd52b`  
		Last Modified: Sat, 26 Sep 2020 01:00:04 GMT  
		Size: 5.2 KB (5168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a31f5f3130dea4d6d5f3a38e0a753dd52c2d6ab9bd62b8d2026ed5cd014b6a`  
		Last Modified: Sat, 26 Sep 2020 01:00:19 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766ae5e0d48c1ad9e04e2131d72be6eeb7b339dc2beae3a4c35710baa3f5a17f`  
		Last Modified: Sat, 26 Sep 2020 01:00:33 GMT  
		Size: 79.4 MB (79370159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a6a06f376dcadd9fd8e6ef1966dd1f1affd6693196e9d7d40cac40792dc4b7`  
		Last Modified: Sat, 26 Sep 2020 01:00:19 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc916d6c5b0e424538b8c22826267ae89150de2367517cf4032e66f9b2235996`  
		Last Modified: Sat, 26 Sep 2020 01:00:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:05a28679caf41c52d9e92cbe79c00eb1add3392d80f94ccddb50f6c1d2b1edbb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105786188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9bb1b5d9a50a9eed5a34f0e3e38a85fbcea0e26485ed4699026f18a059164c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:30:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:31:03 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:04 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:31:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:31:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:31:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:37 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:31:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:32:47 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 25 Sep 2020 23:32:48 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Fri, 25 Sep 2020 23:32:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:33:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:33:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:33:47 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:33:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Sep 2020 23:33:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:33:50 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:33:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b948e33cebad9af1f4cc77312dcfad86464dd571ed4ecb6e3880b64abd285`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d78577b121ac4f4d8a9a8fecaf3c849e9aa15ee980318138e60672a5dd85de`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 4.4 MB (4394361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5fe0c4c88086ceb1b4f120de94964bd6050d51ab27eb80b76f6e71e9eb6fb2`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.3 MB (1263464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456657275618d9347e2c3164308bfd0c90e1995e858896621d3b64c520aac55e`  
		Last Modified: Fri, 25 Sep 2020 23:36:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297f39adae4458e94ebfe715a0dd77d750580f8c6fd7961365c46778f415776c`  
		Last Modified: Fri, 25 Sep 2020 23:36:24 GMT  
		Size: 921.6 KB (921557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381305efa4d2f972fc7b3f6d8da8d7285f7aee1a3f4d6db3cf59e1695dabbc79`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86092c6811f9656d0786c0b4a2b8ffb49becaaa86c0e97b3d18263dba329a6a8`  
		Last Modified: Fri, 25 Sep 2020 23:36:54 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7738332ebbf8721d6d45c7a983aa021a84dc8acb6e3e4eb5c62cc5e8cb921f26`  
		Last Modified: Fri, 25 Sep 2020 23:37:15 GMT  
		Size: 75.5 MB (75470198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c7c350510b29964c8f77a34652c97d9ff708c2e8273809e3ac52df09240dd9`  
		Last Modified: Fri, 25 Sep 2020 23:36:54 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc7f86d096164dff193254ac1a3d5d93d0d53fd96add6f99185d97cf23a88d5`  
		Last Modified: Fri, 25 Sep 2020 23:36:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5c044be112661ae3cc5d8b3c03e9c1cb6be2aa482a628dd9b5d45bbc7831d5e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118183242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365f7b2a8c4fce22908ff56f42df26ab6c5d9a36580c6fe06af32ba205eb5948`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:24:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:26:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:26:16 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:26:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:27:25 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:30:16 GMT
ENV MARIADB_MAJOR=10.1
# Sat, 26 Sep 2020 04:30:21 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Sat, 26 Sep 2020 04:30:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:32:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:33:01 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:33:04 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:33:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 04:33:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:33:14 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:33:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bce23f21744d3f5a1047249d677d9394faaf1f984f7ec4a9c1198277e1f3d18`  
		Last Modified: Sat, 26 Sep 2020 04:36:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d8cd57b26b1e7a1dd53588ecbabb82238fd04c435cabb3aeabc11d7aac7de1`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 5.6 MB (5629583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf63ae75dfbc766239bf488cddba751e125654cb6547cae7ba1227b0036e41`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 1.2 MB (1246387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe7724a4befdb4e6fb4a984e5531a59f4e2f18bca9eb68c1540e5c553d1cbe`  
		Last Modified: Sat, 26 Sep 2020 04:36:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110b905a4cfb8b9a52b8a48813cefc23379dca2ac8f646406490c42fcf4439d`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 931.8 KB (931831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d87b865ce6681ed862606042058bc38215b7d355bd89a5c0f648672f0f23259`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadfac35f0eecf80860c27cefa5339e2eba1e7519b1c327a3d36e9d8a4cfaa87`  
		Last Modified: Sat, 26 Sep 2020 04:37:11 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041adb11c613ca8074519b862f33f75084f6bc654b3eba5ea8aa4fd8b3c5f367`  
		Last Modified: Sat, 26 Sep 2020 04:37:30 GMT  
		Size: 80.0 MB (79953195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbcada6bc209541fd12af7d9b27a29345cd4da14d0bf4b0fe2ddb1024da0811`  
		Last Modified: Sat, 26 Sep 2020 04:37:11 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d761754711586f4fbda10f1e96ee0374d992d18505b2df20c72e12a54a0b9150`  
		Last Modified: Sat, 26 Sep 2020 04:37:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1.47`

**does not exist** (yet?)

## `mariadb:10.1.47-bionic`

**does not exist** (yet?)

## `mariadb:10.1-bionic`

```console
$ docker pull mariadb@sha256:ff77fd8f8156262c4db4075c2abaeca212a60765a91dc4814cc11060d66ff2f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:f1b8db6f50310f74bfc6344d3a5882061cca0cc2c7bfadc7f0d393c96dd30cf5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113154815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ae24e47e14441d9c39f1c489fd14ec98c0c0146d36f6655cf63d5b84f0e4b54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:55:59 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:56:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:56:11 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:56:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:56:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:56:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:56:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:56:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:57:42 GMT
ENV MARIADB_MAJOR=10.1
# Sat, 26 Sep 2020 00:57:42 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Sat, 26 Sep 2020 00:57:42 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:58:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:58:14 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:58:14 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:58:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 00:58:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:58:15 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:58:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928020f0412e3eba561c742f10581acf4ca64971be9de7c21db53f9375ab82a0`  
		Last Modified: Sat, 26 Sep 2020 01:00:06 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b22d867bcc98722fa20b0feccc8434bed1423ea0d0080e6381ac6e12fd9832`  
		Last Modified: Sat, 26 Sep 2020 01:00:06 GMT  
		Size: 4.8 MB (4811571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5f9e2cc9e34fc162225c6bb7c8bb297112a362d456ad7900c14987c7835a26`  
		Last Modified: Sat, 26 Sep 2020 01:00:08 GMT  
		Size: 1.3 MB (1327238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c978fcde13344ce411d42bad561de5cebf5743c87cc6fc33b25872f6b929eca6`  
		Last Modified: Sat, 26 Sep 2020 01:00:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4d9e93f2fbf36cbabecdede7edbe2ab3fb653f34d8e92e819c9c06ddd3ffa8`  
		Last Modified: Sat, 26 Sep 2020 01:00:01 GMT  
		Size: 930.6 KB (930554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d8ee36e7ef936f57d1a918f47f7cad0121f275966dee17b78458c4c51cd52b`  
		Last Modified: Sat, 26 Sep 2020 01:00:04 GMT  
		Size: 5.2 KB (5168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a31f5f3130dea4d6d5f3a38e0a753dd52c2d6ab9bd62b8d2026ed5cd014b6a`  
		Last Modified: Sat, 26 Sep 2020 01:00:19 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766ae5e0d48c1ad9e04e2131d72be6eeb7b339dc2beae3a4c35710baa3f5a17f`  
		Last Modified: Sat, 26 Sep 2020 01:00:33 GMT  
		Size: 79.4 MB (79370159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a6a06f376dcadd9fd8e6ef1966dd1f1affd6693196e9d7d40cac40792dc4b7`  
		Last Modified: Sat, 26 Sep 2020 01:00:19 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc916d6c5b0e424538b8c22826267ae89150de2367517cf4032e66f9b2235996`  
		Last Modified: Sat, 26 Sep 2020 01:00:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:05a28679caf41c52d9e92cbe79c00eb1add3392d80f94ccddb50f6c1d2b1edbb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105786188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9bb1b5d9a50a9eed5a34f0e3e38a85fbcea0e26485ed4699026f18a059164c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:30:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:31:03 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:04 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:31:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:31:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:31:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:37 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:31:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:32:47 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 25 Sep 2020 23:32:48 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Fri, 25 Sep 2020 23:32:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:33:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:33:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:33:47 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:33:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Sep 2020 23:33:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:33:50 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:33:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b948e33cebad9af1f4cc77312dcfad86464dd571ed4ecb6e3880b64abd285`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d78577b121ac4f4d8a9a8fecaf3c849e9aa15ee980318138e60672a5dd85de`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 4.4 MB (4394361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5fe0c4c88086ceb1b4f120de94964bd6050d51ab27eb80b76f6e71e9eb6fb2`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.3 MB (1263464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456657275618d9347e2c3164308bfd0c90e1995e858896621d3b64c520aac55e`  
		Last Modified: Fri, 25 Sep 2020 23:36:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297f39adae4458e94ebfe715a0dd77d750580f8c6fd7961365c46778f415776c`  
		Last Modified: Fri, 25 Sep 2020 23:36:24 GMT  
		Size: 921.6 KB (921557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381305efa4d2f972fc7b3f6d8da8d7285f7aee1a3f4d6db3cf59e1695dabbc79`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86092c6811f9656d0786c0b4a2b8ffb49becaaa86c0e97b3d18263dba329a6a8`  
		Last Modified: Fri, 25 Sep 2020 23:36:54 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7738332ebbf8721d6d45c7a983aa021a84dc8acb6e3e4eb5c62cc5e8cb921f26`  
		Last Modified: Fri, 25 Sep 2020 23:37:15 GMT  
		Size: 75.5 MB (75470198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c7c350510b29964c8f77a34652c97d9ff708c2e8273809e3ac52df09240dd9`  
		Last Modified: Fri, 25 Sep 2020 23:36:54 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc7f86d096164dff193254ac1a3d5d93d0d53fd96add6f99185d97cf23a88d5`  
		Last Modified: Fri, 25 Sep 2020 23:36:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5c044be112661ae3cc5d8b3c03e9c1cb6be2aa482a628dd9b5d45bbc7831d5e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118183242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365f7b2a8c4fce22908ff56f42df26ab6c5d9a36580c6fe06af32ba205eb5948`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:24:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:26:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:26:16 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:26:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:27:25 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:30:16 GMT
ENV MARIADB_MAJOR=10.1
# Sat, 26 Sep 2020 04:30:21 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Sat, 26 Sep 2020 04:30:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:32:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:33:01 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:33:04 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:33:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 04:33:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:33:14 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:33:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bce23f21744d3f5a1047249d677d9394faaf1f984f7ec4a9c1198277e1f3d18`  
		Last Modified: Sat, 26 Sep 2020 04:36:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d8cd57b26b1e7a1dd53588ecbabb82238fd04c435cabb3aeabc11d7aac7de1`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 5.6 MB (5629583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf63ae75dfbc766239bf488cddba751e125654cb6547cae7ba1227b0036e41`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 1.2 MB (1246387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe7724a4befdb4e6fb4a984e5531a59f4e2f18bca9eb68c1540e5c553d1cbe`  
		Last Modified: Sat, 26 Sep 2020 04:36:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110b905a4cfb8b9a52b8a48813cefc23379dca2ac8f646406490c42fcf4439d`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 931.8 KB (931831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d87b865ce6681ed862606042058bc38215b7d355bd89a5c0f648672f0f23259`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadfac35f0eecf80860c27cefa5339e2eba1e7519b1c327a3d36e9d8a4cfaa87`  
		Last Modified: Sat, 26 Sep 2020 04:37:11 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041adb11c613ca8074519b862f33f75084f6bc654b3eba5ea8aa4fd8b3c5f367`  
		Last Modified: Sat, 26 Sep 2020 04:37:30 GMT  
		Size: 80.0 MB (79953195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbcada6bc209541fd12af7d9b27a29345cd4da14d0bf4b0fe2ddb1024da0811`  
		Last Modified: Sat, 26 Sep 2020 04:37:11 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d761754711586f4fbda10f1e96ee0374d992d18505b2df20c72e12a54a0b9150`  
		Last Modified: Sat, 26 Sep 2020 04:37:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:9343e2d69f0a85cc022a22a5b0b28fb5aed0b1960a2644b46fdb6a2bb91ad248
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:36eaffe55e4a4525c97fc4f25be29f83a82ac04ae2ee25984cea7a121b3622a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109006740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36837551a279ce8b8a30fd7cac385ad17656a7dd219f3e5bb6a29bef51acc5c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:55:59 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:56:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:56:11 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:56:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:56:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:56:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:56:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:56:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:56:29 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 26 Sep 2020 00:56:29 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Sat, 26 Sep 2020 00:56:30 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:57:00 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:57:01 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:57:01 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:57:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 00:57:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:57:02 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:57:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928020f0412e3eba561c742f10581acf4ca64971be9de7c21db53f9375ab82a0`  
		Last Modified: Sat, 26 Sep 2020 01:00:06 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b22d867bcc98722fa20b0feccc8434bed1423ea0d0080e6381ac6e12fd9832`  
		Last Modified: Sat, 26 Sep 2020 01:00:06 GMT  
		Size: 4.8 MB (4811571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5f9e2cc9e34fc162225c6bb7c8bb297112a362d456ad7900c14987c7835a26`  
		Last Modified: Sat, 26 Sep 2020 01:00:08 GMT  
		Size: 1.3 MB (1327238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c978fcde13344ce411d42bad561de5cebf5743c87cc6fc33b25872f6b929eca6`  
		Last Modified: Sat, 26 Sep 2020 01:00:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4d9e93f2fbf36cbabecdede7edbe2ab3fb653f34d8e92e819c9c06ddd3ffa8`  
		Last Modified: Sat, 26 Sep 2020 01:00:01 GMT  
		Size: 930.6 KB (930554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d8ee36e7ef936f57d1a918f47f7cad0121f275966dee17b78458c4c51cd52b`  
		Last Modified: Sat, 26 Sep 2020 01:00:04 GMT  
		Size: 5.2 KB (5168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ea59d1afe609d30922eab2494f1f60941ca1d7b2a601968d54f87c675b9efb`  
		Last Modified: Sat, 26 Sep 2020 01:00:00 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a812a06ef94cc083151c58fb69789bd69c362db0bb6a1112366075062669b68`  
		Last Modified: Sat, 26 Sep 2020 01:00:13 GMT  
		Size: 75.2 MB (75222083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c81f4db87054e73d49a583ffe754762bf7a8a653302505594b2ec6190a5bdf`  
		Last Modified: Sat, 26 Sep 2020 01:00:04 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec83ea16bd61caeb859d335ffbebc91ef79c732716d721c977e3cbeefc9ddfa8`  
		Last Modified: Sat, 26 Sep 2020 01:00:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:e90d2a5d2ed40852d33081de2743a91a8bca2b893f53c5c4598ee519351aa089
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104060373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7f41b5afb1ba8843ff8bd2060ad427287660e7de655bae83695a26e32abd31a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:30:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:31:03 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:04 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:31:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:31:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:31:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:37 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:31:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:31:40 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 25 Sep 2020 23:31:41 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Fri, 25 Sep 2020 23:31:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:32:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:32:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:32:32 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:32:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Sep 2020 23:32:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:32:37 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:32:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b948e33cebad9af1f4cc77312dcfad86464dd571ed4ecb6e3880b64abd285`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d78577b121ac4f4d8a9a8fecaf3c849e9aa15ee980318138e60672a5dd85de`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 4.4 MB (4394361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5fe0c4c88086ceb1b4f120de94964bd6050d51ab27eb80b76f6e71e9eb6fb2`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.3 MB (1263464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456657275618d9347e2c3164308bfd0c90e1995e858896621d3b64c520aac55e`  
		Last Modified: Fri, 25 Sep 2020 23:36:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297f39adae4458e94ebfe715a0dd77d750580f8c6fd7961365c46778f415776c`  
		Last Modified: Fri, 25 Sep 2020 23:36:24 GMT  
		Size: 921.6 KB (921557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381305efa4d2f972fc7b3f6d8da8d7285f7aee1a3f4d6db3cf59e1695dabbc79`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5860d883603b149f973b1cebe9be77e420c51a55b54d56ac61e3c7f093ce5ee`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0492ab6ce270dd49e197687a1ffdf83c593a30daf50dcbe94cb660c20af332cf`  
		Last Modified: Fri, 25 Sep 2020 23:36:43 GMT  
		Size: 73.7 MB (73744384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb5c9a367d116ca1638ccd7bb10f62d4543b10838c034c7c3feab48dff700f0`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593619234f646eea562fcfa5a3efcfe95f21fe11739d612dbb1e3f02338d02c9`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ae8a47017b1c0c8b734e9602ccbbae99f30612c1d43e19d448e29629c252e06a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116233000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac0485f662c908bd3341e2edbeb68b441535f9cc85c106d1d52c1e10bd9564f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:24:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:26:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:26:16 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:26:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:27:25 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:27:33 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 26 Sep 2020 04:27:36 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Sat, 26 Sep 2020 04:27:43 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:29:39 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:29:47 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:29:48 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:29:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 04:29:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:29:57 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:30:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bce23f21744d3f5a1047249d677d9394faaf1f984f7ec4a9c1198277e1f3d18`  
		Last Modified: Sat, 26 Sep 2020 04:36:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d8cd57b26b1e7a1dd53588ecbabb82238fd04c435cabb3aeabc11d7aac7de1`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 5.6 MB (5629583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf63ae75dfbc766239bf488cddba751e125654cb6547cae7ba1227b0036e41`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 1.2 MB (1246387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe7724a4befdb4e6fb4a984e5531a59f4e2f18bca9eb68c1540e5c553d1cbe`  
		Last Modified: Sat, 26 Sep 2020 04:36:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110b905a4cfb8b9a52b8a48813cefc23379dca2ac8f646406490c42fcf4439d`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 931.8 KB (931831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d87b865ce6681ed862606042058bc38215b7d355bd89a5c0f648672f0f23259`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a388de4edb8f8d49edba8a50e386252eabdaa4b8f61d2397c31c467702fbb93c`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883b0979dd90d7f6e421404dcd6e35e68ed29f489d699b409d802ff29eb53219`  
		Last Modified: Sat, 26 Sep 2020 04:36:54 GMT  
		Size: 78.0 MB (78002955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fd2daeb5a4fcd32442ebef0b8b6c9a8f8b4631710cf954c917f420b043e361`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e8bd4a5ffdd03c7788503a5e63dc4e8bbdd166cca9fe2dab8ad13c21ebd0a9`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.34`

**does not exist** (yet?)

## `mariadb:10.2.34-bionic`

**does not exist** (yet?)

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:9343e2d69f0a85cc022a22a5b0b28fb5aed0b1960a2644b46fdb6a2bb91ad248
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:36eaffe55e4a4525c97fc4f25be29f83a82ac04ae2ee25984cea7a121b3622a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109006740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36837551a279ce8b8a30fd7cac385ad17656a7dd219f3e5bb6a29bef51acc5c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:55:59 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:56:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:56:11 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:56:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:56:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:56:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:56:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:56:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:56:29 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 26 Sep 2020 00:56:29 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Sat, 26 Sep 2020 00:56:30 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:57:00 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:57:01 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:57:01 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:57:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 00:57:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:57:02 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:57:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928020f0412e3eba561c742f10581acf4ca64971be9de7c21db53f9375ab82a0`  
		Last Modified: Sat, 26 Sep 2020 01:00:06 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b22d867bcc98722fa20b0feccc8434bed1423ea0d0080e6381ac6e12fd9832`  
		Last Modified: Sat, 26 Sep 2020 01:00:06 GMT  
		Size: 4.8 MB (4811571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5f9e2cc9e34fc162225c6bb7c8bb297112a362d456ad7900c14987c7835a26`  
		Last Modified: Sat, 26 Sep 2020 01:00:08 GMT  
		Size: 1.3 MB (1327238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c978fcde13344ce411d42bad561de5cebf5743c87cc6fc33b25872f6b929eca6`  
		Last Modified: Sat, 26 Sep 2020 01:00:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4d9e93f2fbf36cbabecdede7edbe2ab3fb653f34d8e92e819c9c06ddd3ffa8`  
		Last Modified: Sat, 26 Sep 2020 01:00:01 GMT  
		Size: 930.6 KB (930554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d8ee36e7ef936f57d1a918f47f7cad0121f275966dee17b78458c4c51cd52b`  
		Last Modified: Sat, 26 Sep 2020 01:00:04 GMT  
		Size: 5.2 KB (5168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ea59d1afe609d30922eab2494f1f60941ca1d7b2a601968d54f87c675b9efb`  
		Last Modified: Sat, 26 Sep 2020 01:00:00 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a812a06ef94cc083151c58fb69789bd69c362db0bb6a1112366075062669b68`  
		Last Modified: Sat, 26 Sep 2020 01:00:13 GMT  
		Size: 75.2 MB (75222083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c81f4db87054e73d49a583ffe754762bf7a8a653302505594b2ec6190a5bdf`  
		Last Modified: Sat, 26 Sep 2020 01:00:04 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec83ea16bd61caeb859d335ffbebc91ef79c732716d721c977e3cbeefc9ddfa8`  
		Last Modified: Sat, 26 Sep 2020 01:00:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:e90d2a5d2ed40852d33081de2743a91a8bca2b893f53c5c4598ee519351aa089
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104060373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7f41b5afb1ba8843ff8bd2060ad427287660e7de655bae83695a26e32abd31a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:30:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:31:03 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:04 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:31:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:31:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:31:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:37 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:31:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:31:40 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 25 Sep 2020 23:31:41 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Fri, 25 Sep 2020 23:31:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:32:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:32:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:32:32 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:32:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Sep 2020 23:32:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:32:37 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:32:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b948e33cebad9af1f4cc77312dcfad86464dd571ed4ecb6e3880b64abd285`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d78577b121ac4f4d8a9a8fecaf3c849e9aa15ee980318138e60672a5dd85de`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 4.4 MB (4394361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5fe0c4c88086ceb1b4f120de94964bd6050d51ab27eb80b76f6e71e9eb6fb2`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.3 MB (1263464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456657275618d9347e2c3164308bfd0c90e1995e858896621d3b64c520aac55e`  
		Last Modified: Fri, 25 Sep 2020 23:36:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297f39adae4458e94ebfe715a0dd77d750580f8c6fd7961365c46778f415776c`  
		Last Modified: Fri, 25 Sep 2020 23:36:24 GMT  
		Size: 921.6 KB (921557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381305efa4d2f972fc7b3f6d8da8d7285f7aee1a3f4d6db3cf59e1695dabbc79`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5860d883603b149f973b1cebe9be77e420c51a55b54d56ac61e3c7f093ce5ee`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0492ab6ce270dd49e197687a1ffdf83c593a30daf50dcbe94cb660c20af332cf`  
		Last Modified: Fri, 25 Sep 2020 23:36:43 GMT  
		Size: 73.7 MB (73744384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb5c9a367d116ca1638ccd7bb10f62d4543b10838c034c7c3feab48dff700f0`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593619234f646eea562fcfa5a3efcfe95f21fe11739d612dbb1e3f02338d02c9`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ae8a47017b1c0c8b734e9602ccbbae99f30612c1d43e19d448e29629c252e06a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116233000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac0485f662c908bd3341e2edbeb68b441535f9cc85c106d1d52c1e10bd9564f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:24:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:26:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:26:16 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:26:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:27:25 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:27:33 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 26 Sep 2020 04:27:36 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Sat, 26 Sep 2020 04:27:43 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:29:39 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:29:47 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:29:48 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:29:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 04:29:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:29:57 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:30:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bce23f21744d3f5a1047249d677d9394faaf1f984f7ec4a9c1198277e1f3d18`  
		Last Modified: Sat, 26 Sep 2020 04:36:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d8cd57b26b1e7a1dd53588ecbabb82238fd04c435cabb3aeabc11d7aac7de1`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 5.6 MB (5629583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf63ae75dfbc766239bf488cddba751e125654cb6547cae7ba1227b0036e41`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 1.2 MB (1246387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe7724a4befdb4e6fb4a984e5531a59f4e2f18bca9eb68c1540e5c553d1cbe`  
		Last Modified: Sat, 26 Sep 2020 04:36:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110b905a4cfb8b9a52b8a48813cefc23379dca2ac8f646406490c42fcf4439d`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 931.8 KB (931831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d87b865ce6681ed862606042058bc38215b7d355bd89a5c0f648672f0f23259`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a388de4edb8f8d49edba8a50e386252eabdaa4b8f61d2397c31c467702fbb93c`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883b0979dd90d7f6e421404dcd6e35e68ed29f489d699b409d802ff29eb53219`  
		Last Modified: Sat, 26 Sep 2020 04:36:54 GMT  
		Size: 78.0 MB (78002955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fd2daeb5a4fcd32442ebef0b8b6c9a8f8b4631710cf954c917f420b043e361`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e8bd4a5ffdd03c7788503a5e63dc4e8bbdd166cca9fe2dab8ad13c21ebd0a9`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:5adbf9e5943d260914a4821c91fae0e0287d24fdb21b8c8ee7e6529a81d0b9b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:3fb77ad7571d0a5beffae826b2616c05d669c879a3a15b26905164c3d4b100f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119159722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8d45007e59a8c40d62dd810198050ad39aabef86b3fd952835d650c79dcaf8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:34:27 GMT
ADD file:da80f59399481ffc32f84353830dcf598f31a97785222e75d643bfb8a9aa14e7 in / 
# Fri, 25 Sep 2020 22:34:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:34:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:34:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:34:30 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:52:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:53:04 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:53:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:53:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:53:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:19 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:53:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:54:48 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 26 Sep 2020 00:54:49 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Sat, 26 Sep 2020 00:54:49 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:55:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:55:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:55:15 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:55:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 00:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:55:16 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:55:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d72e567cc804d0b637182ba23f8b9ffe101e753a39bf52cd4db6b89eb089f13b`  
		Last Modified: Fri, 25 Sep 2020 15:20:50 GMT  
		Size: 28.6 MB (28558050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3630e5ff08d73b6ec0e22736a5c8d2d666e7b568c16f6a4ffadf8c21b9b1ad`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a83d81d1f4f942d37e1f17195d9c519969ed3040fc3e444740b884e44dec33`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf2111ecf0efaa19887c07ce1ae8332ebff5775482731d8e524898d9fc07e23`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d64978a09242b12c715a8cfda3ce4ac4ef1e086016ccb32edb185f844363`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 5.5 MB (5488523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc9953bffb3c364d00df0e3961c569c5eebc2015cabee42cb7e0b33c4ba6891`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 1.3 MB (1324124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de429570dda5816121294e9251d2cf7f258f2a0c9fdf2a7ba9a7ebe56a763e83`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3652bc6ea9f9147ae99d11202e416c096df524bf3a64b6f483adb8d54e59a4a0`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 1.3 MB (1265989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4bf87041c8ad8ddf97dbbb645685d428963abc9d376dc413e6f7ee202af1ab`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19e8769b9aa9a3e3b505da3d07699451975470b5238870a230759db28a4fbef`  
		Last Modified: Sat, 26 Sep 2020 00:59:39 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8060bddcd610811e8c8158b5dbb004c6ec2cc2575aaba427bc2b4b5a972a0b`  
		Last Modified: Sat, 26 Sep 2020 00:59:54 GMT  
		Size: 82.5 MB (82512174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5d7c67935829a90b01ba828134780ca9beb1d63a5ab4c7a71067906e899be9`  
		Last Modified: Sat, 26 Sep 2020 00:59:39 GMT  
		Size: 5.1 KB (5055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1220fea18c8d320dc7a8002ed6dea2662b665fc78b8fd48612d3f6924318fd2`  
		Last Modified: Sat, 26 Sep 2020 00:59:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:3a41bda0bc74a6db9bea4473eceb94ba8023c6c1a73acd7ffbd20e03986c349b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116817877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16fe3e2c9862a106079f1dc36452e1d7f7e537a40827f1a18145a06e16b99ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:59 GMT
ADD file:e1079b8987ad959c6a83dae1ea4446405953ab16899c693d57c6214ff888e688 in / 
# Fri, 25 Sep 2020 22:48:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:48:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:48:06 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:26:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:27:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:27:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:27:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:27:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:30 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:27:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:29:35 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 25 Sep 2020 23:29:36 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Fri, 25 Sep 2020 23:29:38 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:30:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:30:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:30:31 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:30:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Sep 2020 23:30:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:30:35 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:30:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a25fe36305380fa444fa6bd15b622145ff6076e5b6f81168d6cb4c9fee725863`  
		Last Modified: Fri, 25 Sep 2020 08:25:35 GMT  
		Size: 27.2 MB (27160123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326fa3abf0610ea05b9deb392e05c6c86a7afed0c119987a8d920a2a8dceaffc`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b87601e0a324569be2cebc4c0b9981bd53925a9bee894fad57c93f9bd3d01`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a280fab3f6130dcd17011ffa4ee6cb14fd04623b4c1e16f378026844b8f428`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b33bb77d692ee1db553b82b566c91f41b6dbfd76e9ba9eaa444b7ca545fe6`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 5.5 MB (5456069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c36f1baced17c5bd6b814a182f023308e1b4cda8870bf91756041505870fa2a`  
		Last Modified: Fri, 25 Sep 2020 23:34:27 GMT  
		Size: 1.3 MB (1261421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a2b365d2a0b2769c317ffcde3ef8699d4d7c3256f95021f1da0d979006c1dc`  
		Last Modified: Fri, 25 Sep 2020 23:34:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f8ac108760bfd505fbfd1b252d7cea8e1c95895d04a6de0fb125d757c67f23`  
		Last Modified: Fri, 25 Sep 2020 23:34:25 GMT  
		Size: 1.3 MB (1265577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91718a6772cfde37e00ab454ab0fe8081399c122f22de9c2cc6b578dfe810cf6`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9180e515751ef81810f0dcb9f22bdf534a5d003dd93dde637b01f4be9d82d0`  
		Last Modified: Fri, 25 Sep 2020 23:35:45 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ed9cc93b836f239b68e3dfee306997fa41282a217ccbf20c8f478f1c066827`  
		Last Modified: Fri, 25 Sep 2020 23:36:09 GMT  
		Size: 81.7 MB (81663764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362d51a4bcf8934cce5afc9fc2739802fca52e9e3dacd47a2a4d039c06c6ad84`  
		Last Modified: Fri, 25 Sep 2020 23:35:45 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1011a382f552080a2d65873f40cdfee4d85863201b930d0355debfa4e763c3cc`  
		Last Modified: Fri, 25 Sep 2020 23:35:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c0fffb2e6c717bae5ddf2a2525794a2616a288d129c7b3e420ae2c85f75b481a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (128978297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357081762a2a6a269d9b481c13e24a0dee1904540f6e783ab378793cba53b78d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:53:28 GMT
ADD file:5479628763eb7f8cd884270bc1e9bb40ce39f1fb3427e863b086511696fa8107 in / 
# Fri, 25 Sep 2020 23:53:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:54:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:54:31 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:13:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:13:26 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:14:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:14:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:14:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:14:59 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:15:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:21:21 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 26 Sep 2020 04:21:23 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Sat, 26 Sep 2020 04:21:30 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:23:39 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:23:50 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:23:51 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:24:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 04:24:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:24:12 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:24:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af5e190551614a549619ca2cb11a237bf566e7b0942eac80adaf05e21644ad12`  
		Last Modified: Sat, 26 Sep 2020 00:06:58 GMT  
		Size: 33.3 MB (33278058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dd7d43fa9f545a3f69e66ff00d1a2773213cdfc18d0c99a71bb1c40bbb1f8c`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1feb93b9aa176877a7ec845345f281fe28c37605e03363dd0fa489bf0bf10ee`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72de4183a4e4f8be028bd4096c22189718c23c7af3d8206f6119c7e672403f5b`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd855440835f9cbdc109164d975673b33c12064da301ac86019019bf4457e2a6`  
		Last Modified: Sat, 26 Sep 2020 04:34:10 GMT  
		Size: 6.7 MB (6668533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc681828d8ea74c541ead13581fa9a5b5aa4c9bd5f23a49edb457fbfef07fad`  
		Last Modified: Sat, 26 Sep 2020 04:34:03 GMT  
		Size: 1.2 MB (1243770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be85c8ddabd72fe111c44f1aa3f8c03e84ab9e12b95ecaf8e14bc19cd8ce63d6`  
		Last Modified: Sat, 26 Sep 2020 04:34:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333eecf00fdea344bb79b6958cbd01f130119d2a12a3b7bcb698262191b0faa`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.3 MB (1273578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b192cad172b5465b46c838d6ed65009da808af10327870e10ca3dc21dfabd797`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7c6d985172e26447456f86cea446c5088df881f69708be06e18a565c1070e6`  
		Last Modified: Sat, 26 Sep 2020 04:36:00 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5956f45e688bd2d2d23f578a6212ab209c91564bf319c60306ae51486bb90f49`  
		Last Modified: Sat, 26 Sep 2020 04:36:20 GMT  
		Size: 86.5 MB (86503427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e092d647617ccfd96e1f975a17618418bbc6074f1293d8466ac4d963019ba92`  
		Last Modified: Sat, 26 Sep 2020 04:36:00 GMT  
		Size: 5.1 KB (5054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0c81f91542a308a7ffc81db7dfd08ac0fd6a88944728b67fd279534e8a1cb6`  
		Last Modified: Sat, 26 Sep 2020 04:36:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.25`

**does not exist** (yet?)

## `mariadb:10.3.25-focal`

**does not exist** (yet?)

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:5adbf9e5943d260914a4821c91fae0e0287d24fdb21b8c8ee7e6529a81d0b9b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:3fb77ad7571d0a5beffae826b2616c05d669c879a3a15b26905164c3d4b100f8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119159722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8d45007e59a8c40d62dd810198050ad39aabef86b3fd952835d650c79dcaf8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:34:27 GMT
ADD file:da80f59399481ffc32f84353830dcf598f31a97785222e75d643bfb8a9aa14e7 in / 
# Fri, 25 Sep 2020 22:34:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:34:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:34:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:34:30 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:52:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:53:04 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:53:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:53:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:53:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:19 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:53:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:54:48 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 26 Sep 2020 00:54:49 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Sat, 26 Sep 2020 00:54:49 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:55:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:55:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:55:15 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:55:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 00:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:55:16 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:55:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d72e567cc804d0b637182ba23f8b9ffe101e753a39bf52cd4db6b89eb089f13b`  
		Last Modified: Fri, 25 Sep 2020 15:20:50 GMT  
		Size: 28.6 MB (28558050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3630e5ff08d73b6ec0e22736a5c8d2d666e7b568c16f6a4ffadf8c21b9b1ad`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a83d81d1f4f942d37e1f17195d9c519969ed3040fc3e444740b884e44dec33`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf2111ecf0efaa19887c07ce1ae8332ebff5775482731d8e524898d9fc07e23`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d64978a09242b12c715a8cfda3ce4ac4ef1e086016ccb32edb185f844363`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 5.5 MB (5488523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc9953bffb3c364d00df0e3961c569c5eebc2015cabee42cb7e0b33c4ba6891`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 1.3 MB (1324124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de429570dda5816121294e9251d2cf7f258f2a0c9fdf2a7ba9a7ebe56a763e83`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3652bc6ea9f9147ae99d11202e416c096df524bf3a64b6f483adb8d54e59a4a0`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 1.3 MB (1265989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4bf87041c8ad8ddf97dbbb645685d428963abc9d376dc413e6f7ee202af1ab`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19e8769b9aa9a3e3b505da3d07699451975470b5238870a230759db28a4fbef`  
		Last Modified: Sat, 26 Sep 2020 00:59:39 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8060bddcd610811e8c8158b5dbb004c6ec2cc2575aaba427bc2b4b5a972a0b`  
		Last Modified: Sat, 26 Sep 2020 00:59:54 GMT  
		Size: 82.5 MB (82512174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5d7c67935829a90b01ba828134780ca9beb1d63a5ab4c7a71067906e899be9`  
		Last Modified: Sat, 26 Sep 2020 00:59:39 GMT  
		Size: 5.1 KB (5055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1220fea18c8d320dc7a8002ed6dea2662b665fc78b8fd48612d3f6924318fd2`  
		Last Modified: Sat, 26 Sep 2020 00:59:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:3a41bda0bc74a6db9bea4473eceb94ba8023c6c1a73acd7ffbd20e03986c349b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116817877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16fe3e2c9862a106079f1dc36452e1d7f7e537a40827f1a18145a06e16b99ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:59 GMT
ADD file:e1079b8987ad959c6a83dae1ea4446405953ab16899c693d57c6214ff888e688 in / 
# Fri, 25 Sep 2020 22:48:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:48:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:48:06 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:26:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:27:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:27:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:27:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:27:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:30 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:27:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:29:35 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 25 Sep 2020 23:29:36 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Fri, 25 Sep 2020 23:29:38 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:30:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:30:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:30:31 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:30:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Sep 2020 23:30:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:30:35 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:30:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a25fe36305380fa444fa6bd15b622145ff6076e5b6f81168d6cb4c9fee725863`  
		Last Modified: Fri, 25 Sep 2020 08:25:35 GMT  
		Size: 27.2 MB (27160123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326fa3abf0610ea05b9deb392e05c6c86a7afed0c119987a8d920a2a8dceaffc`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b87601e0a324569be2cebc4c0b9981bd53925a9bee894fad57c93f9bd3d01`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a280fab3f6130dcd17011ffa4ee6cb14fd04623b4c1e16f378026844b8f428`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b33bb77d692ee1db553b82b566c91f41b6dbfd76e9ba9eaa444b7ca545fe6`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 5.5 MB (5456069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c36f1baced17c5bd6b814a182f023308e1b4cda8870bf91756041505870fa2a`  
		Last Modified: Fri, 25 Sep 2020 23:34:27 GMT  
		Size: 1.3 MB (1261421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a2b365d2a0b2769c317ffcde3ef8699d4d7c3256f95021f1da0d979006c1dc`  
		Last Modified: Fri, 25 Sep 2020 23:34:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f8ac108760bfd505fbfd1b252d7cea8e1c95895d04a6de0fb125d757c67f23`  
		Last Modified: Fri, 25 Sep 2020 23:34:25 GMT  
		Size: 1.3 MB (1265577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91718a6772cfde37e00ab454ab0fe8081399c122f22de9c2cc6b578dfe810cf6`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9180e515751ef81810f0dcb9f22bdf534a5d003dd93dde637b01f4be9d82d0`  
		Last Modified: Fri, 25 Sep 2020 23:35:45 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ed9cc93b836f239b68e3dfee306997fa41282a217ccbf20c8f478f1c066827`  
		Last Modified: Fri, 25 Sep 2020 23:36:09 GMT  
		Size: 81.7 MB (81663764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362d51a4bcf8934cce5afc9fc2739802fca52e9e3dacd47a2a4d039c06c6ad84`  
		Last Modified: Fri, 25 Sep 2020 23:35:45 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1011a382f552080a2d65873f40cdfee4d85863201b930d0355debfa4e763c3cc`  
		Last Modified: Fri, 25 Sep 2020 23:35:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c0fffb2e6c717bae5ddf2a2525794a2616a288d129c7b3e420ae2c85f75b481a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (128978297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357081762a2a6a269d9b481c13e24a0dee1904540f6e783ab378793cba53b78d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:53:28 GMT
ADD file:5479628763eb7f8cd884270bc1e9bb40ce39f1fb3427e863b086511696fa8107 in / 
# Fri, 25 Sep 2020 23:53:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:54:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:54:31 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:13:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:13:26 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:14:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:14:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:14:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:14:59 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:15:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:21:21 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 26 Sep 2020 04:21:23 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Sat, 26 Sep 2020 04:21:30 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:23:39 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:23:50 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:23:51 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:24:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 04:24:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:24:12 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:24:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af5e190551614a549619ca2cb11a237bf566e7b0942eac80adaf05e21644ad12`  
		Last Modified: Sat, 26 Sep 2020 00:06:58 GMT  
		Size: 33.3 MB (33278058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dd7d43fa9f545a3f69e66ff00d1a2773213cdfc18d0c99a71bb1c40bbb1f8c`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1feb93b9aa176877a7ec845345f281fe28c37605e03363dd0fa489bf0bf10ee`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72de4183a4e4f8be028bd4096c22189718c23c7af3d8206f6119c7e672403f5b`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd855440835f9cbdc109164d975673b33c12064da301ac86019019bf4457e2a6`  
		Last Modified: Sat, 26 Sep 2020 04:34:10 GMT  
		Size: 6.7 MB (6668533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc681828d8ea74c541ead13581fa9a5b5aa4c9bd5f23a49edb457fbfef07fad`  
		Last Modified: Sat, 26 Sep 2020 04:34:03 GMT  
		Size: 1.2 MB (1243770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be85c8ddabd72fe111c44f1aa3f8c03e84ab9e12b95ecaf8e14bc19cd8ce63d6`  
		Last Modified: Sat, 26 Sep 2020 04:34:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333eecf00fdea344bb79b6958cbd01f130119d2a12a3b7bcb698262191b0faa`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.3 MB (1273578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b192cad172b5465b46c838d6ed65009da808af10327870e10ca3dc21dfabd797`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7c6d985172e26447456f86cea446c5088df881f69708be06e18a565c1070e6`  
		Last Modified: Sat, 26 Sep 2020 04:36:00 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5956f45e688bd2d2d23f578a6212ab209c91564bf319c60306ae51486bb90f49`  
		Last Modified: Sat, 26 Sep 2020 04:36:20 GMT  
		Size: 86.5 MB (86503427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e092d647617ccfd96e1f975a17618418bbc6074f1293d8466ac4d963019ba92`  
		Last Modified: Sat, 26 Sep 2020 04:36:00 GMT  
		Size: 5.1 KB (5054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0c81f91542a308a7ffc81db7dfd08ac0fd6a88944728b67fd279534e8a1cb6`  
		Last Modified: Sat, 26 Sep 2020 04:36:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:3ea7ee73841f5ef93a4788985051dce84f4b936b475cb3c729b836908a6c21e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:1b79717ebf709fb6a15aefd98b54ed8c18137e09b7ac9933b92d6fd9a0fc8134
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123516527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96e797480ac57c2d6ad4cc5e43e9a703dabc85108c44c7223ab05306d1a0b772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:34:27 GMT
ADD file:da80f59399481ffc32f84353830dcf598f31a97785222e75d643bfb8a9aa14e7 in / 
# Fri, 25 Sep 2020 22:34:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:34:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:34:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:34:30 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:52:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:53:04 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:53:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:53:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:53:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:19 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:53:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:54:08 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 26 Sep 2020 00:54:08 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Sat, 26 Sep 2020 00:54:09 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:54:35 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:54:35 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:54:35 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:54:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 00:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:54:37 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:54:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d72e567cc804d0b637182ba23f8b9ffe101e753a39bf52cd4db6b89eb089f13b`  
		Last Modified: Fri, 25 Sep 2020 15:20:50 GMT  
		Size: 28.6 MB (28558050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3630e5ff08d73b6ec0e22736a5c8d2d666e7b568c16f6a4ffadf8c21b9b1ad`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a83d81d1f4f942d37e1f17195d9c519969ed3040fc3e444740b884e44dec33`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf2111ecf0efaa19887c07ce1ae8332ebff5775482731d8e524898d9fc07e23`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d64978a09242b12c715a8cfda3ce4ac4ef1e086016ccb32edb185f844363`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 5.5 MB (5488523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc9953bffb3c364d00df0e3961c569c5eebc2015cabee42cb7e0b33c4ba6891`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 1.3 MB (1324124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de429570dda5816121294e9251d2cf7f258f2a0c9fdf2a7ba9a7ebe56a763e83`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3652bc6ea9f9147ae99d11202e416c096df524bf3a64b6f483adb8d54e59a4a0`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 1.3 MB (1265989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4bf87041c8ad8ddf97dbbb645685d428963abc9d376dc413e6f7ee202af1ab`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ec9133cd3559c8fa558621554b2ea84f1e98c236c7dc8d1bc5f49cc5ab8639`  
		Last Modified: Sat, 26 Sep 2020 00:59:14 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aed66549b8e077f4709e4a810c54d9e77c8a3204b2b7a2b38cc6a75eb167ebd`  
		Last Modified: Sat, 26 Sep 2020 00:59:32 GMT  
		Size: 86.9 MB (86868980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df1086bca2359c48961a6a8509d2a87fbbce4e02d026d2fb6c71979c10ee73d`  
		Last Modified: Sat, 26 Sep 2020 00:59:14 GMT  
		Size: 5.1 KB (5055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eec6d6b82171ba862286f1be69df53aa151d327533c291e4de3b0ff2b1a17db`  
		Last Modified: Sat, 26 Sep 2020 00:59:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dd0778c8a1c593a11d73370ba6e1d667d60d0db647342e7ae06bfcc4eb09fc98
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121149179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1aebd936b3f97280ebde816dc6a608bacc3132c9c2a434b046d1f6b16bbec2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:59 GMT
ADD file:e1079b8987ad959c6a83dae1ea4446405953ab16899c693d57c6214ff888e688 in / 
# Fri, 25 Sep 2020 22:48:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:48:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:48:06 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:26:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:27:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:27:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:27:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:27:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:30 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:27:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:28:28 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 25 Sep 2020 23:28:29 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Fri, 25 Sep 2020 23:28:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:29:17 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:29:19 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:29:20 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:29:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Sep 2020 23:29:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:29:23 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:29:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a25fe36305380fa444fa6bd15b622145ff6076e5b6f81168d6cb4c9fee725863`  
		Last Modified: Fri, 25 Sep 2020 08:25:35 GMT  
		Size: 27.2 MB (27160123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326fa3abf0610ea05b9deb392e05c6c86a7afed0c119987a8d920a2a8dceaffc`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b87601e0a324569be2cebc4c0b9981bd53925a9bee894fad57c93f9bd3d01`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a280fab3f6130dcd17011ffa4ee6cb14fd04623b4c1e16f378026844b8f428`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b33bb77d692ee1db553b82b566c91f41b6dbfd76e9ba9eaa444b7ca545fe6`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 5.5 MB (5456069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c36f1baced17c5bd6b814a182f023308e1b4cda8870bf91756041505870fa2a`  
		Last Modified: Fri, 25 Sep 2020 23:34:27 GMT  
		Size: 1.3 MB (1261421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a2b365d2a0b2769c317ffcde3ef8699d4d7c3256f95021f1da0d979006c1dc`  
		Last Modified: Fri, 25 Sep 2020 23:34:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f8ac108760bfd505fbfd1b252d7cea8e1c95895d04a6de0fb125d757c67f23`  
		Last Modified: Fri, 25 Sep 2020 23:34:25 GMT  
		Size: 1.3 MB (1265577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91718a6772cfde37e00ab454ab0fe8081399c122f22de9c2cc6b578dfe810cf6`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c92fe8fee7a0b55d9e228c7a2fd7a249c8ffae66c8dd4f6e48681d431b905a9`  
		Last Modified: Fri, 25 Sep 2020 23:35:09 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46d6d103a32439e7956459a1d8c564be014d0127d15f6d7601b1547ffb46dcf`  
		Last Modified: Fri, 25 Sep 2020 23:35:34 GMT  
		Size: 86.0 MB (85995064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b55ae113bedf652da33213ca01e2304682c03fab920876bfddd8cb4322751c4`  
		Last Modified: Fri, 25 Sep 2020 23:35:09 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9191be867cd0fbee52b3a634ab8ea2845432c6f5076552c3b8fc4da0b77d3a13`  
		Last Modified: Fri, 25 Sep 2020 23:35:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a4a927d9dc128217cc28e4e023e3d94735aee608926168b5c41057fe3b343e65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133487617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c0223e2d920b5fc07998502f2eb82311985e6c48f30a0f4ad3fc74c7c7c11f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:53:28 GMT
ADD file:5479628763eb7f8cd884270bc1e9bb40ce39f1fb3427e863b086511696fa8107 in / 
# Fri, 25 Sep 2020 23:53:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:54:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:54:31 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:13:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:13:26 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:14:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:14:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:14:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:14:59 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:15:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:18:41 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 26 Sep 2020 04:18:44 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Sat, 26 Sep 2020 04:18:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:20:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:20:56 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:20:57 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:21:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 04:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:21:08 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:21:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af5e190551614a549619ca2cb11a237bf566e7b0942eac80adaf05e21644ad12`  
		Last Modified: Sat, 26 Sep 2020 00:06:58 GMT  
		Size: 33.3 MB (33278058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dd7d43fa9f545a3f69e66ff00d1a2773213cdfc18d0c99a71bb1c40bbb1f8c`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1feb93b9aa176877a7ec845345f281fe28c37605e03363dd0fa489bf0bf10ee`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72de4183a4e4f8be028bd4096c22189718c23c7af3d8206f6119c7e672403f5b`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd855440835f9cbdc109164d975673b33c12064da301ac86019019bf4457e2a6`  
		Last Modified: Sat, 26 Sep 2020 04:34:10 GMT  
		Size: 6.7 MB (6668533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc681828d8ea74c541ead13581fa9a5b5aa4c9bd5f23a49edb457fbfef07fad`  
		Last Modified: Sat, 26 Sep 2020 04:34:03 GMT  
		Size: 1.2 MB (1243770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be85c8ddabd72fe111c44f1aa3f8c03e84ab9e12b95ecaf8e14bc19cd8ce63d6`  
		Last Modified: Sat, 26 Sep 2020 04:34:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333eecf00fdea344bb79b6958cbd01f130119d2a12a3b7bcb698262191b0faa`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.3 MB (1273578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b192cad172b5465b46c838d6ed65009da808af10327870e10ca3dc21dfabd797`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3083778fe68309e214cb27ddc2835f4400ffecbae0307d95e0204edda4a57d45`  
		Last Modified: Sat, 26 Sep 2020 04:35:21 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb33f57f5e78e802612bf5c550f320f5db73a97b30fd59a4a9858e7979ab1563`  
		Last Modified: Sat, 26 Sep 2020 04:35:42 GMT  
		Size: 91.0 MB (91012743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497d7737768b7172015f8a6cc1aa2c78db159dcce10ca6a3ae5a3b5486fed14e`  
		Last Modified: Sat, 26 Sep 2020 04:35:21 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1544c05fda9cafb8d5ee2a9bd7c0435abe9e0143abd38a1d971181084cd882a`  
		Last Modified: Sat, 26 Sep 2020 04:35:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.15`

**does not exist** (yet?)

## `mariadb:10.4.15-focal`

**does not exist** (yet?)

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:3ea7ee73841f5ef93a4788985051dce84f4b936b475cb3c729b836908a6c21e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:1b79717ebf709fb6a15aefd98b54ed8c18137e09b7ac9933b92d6fd9a0fc8134
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123516527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96e797480ac57c2d6ad4cc5e43e9a703dabc85108c44c7223ab05306d1a0b772`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:34:27 GMT
ADD file:da80f59399481ffc32f84353830dcf598f31a97785222e75d643bfb8a9aa14e7 in / 
# Fri, 25 Sep 2020 22:34:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:34:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:34:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:34:30 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:52:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:53:04 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:53:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:53:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:53:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:19 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:53:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:54:08 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 26 Sep 2020 00:54:08 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Sat, 26 Sep 2020 00:54:09 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:54:35 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:54:35 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:54:35 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:54:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 00:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:54:37 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:54:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d72e567cc804d0b637182ba23f8b9ffe101e753a39bf52cd4db6b89eb089f13b`  
		Last Modified: Fri, 25 Sep 2020 15:20:50 GMT  
		Size: 28.6 MB (28558050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3630e5ff08d73b6ec0e22736a5c8d2d666e7b568c16f6a4ffadf8c21b9b1ad`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a83d81d1f4f942d37e1f17195d9c519969ed3040fc3e444740b884e44dec33`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf2111ecf0efaa19887c07ce1ae8332ebff5775482731d8e524898d9fc07e23`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d64978a09242b12c715a8cfda3ce4ac4ef1e086016ccb32edb185f844363`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 5.5 MB (5488523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc9953bffb3c364d00df0e3961c569c5eebc2015cabee42cb7e0b33c4ba6891`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 1.3 MB (1324124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de429570dda5816121294e9251d2cf7f258f2a0c9fdf2a7ba9a7ebe56a763e83`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3652bc6ea9f9147ae99d11202e416c096df524bf3a64b6f483adb8d54e59a4a0`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 1.3 MB (1265989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4bf87041c8ad8ddf97dbbb645685d428963abc9d376dc413e6f7ee202af1ab`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ec9133cd3559c8fa558621554b2ea84f1e98c236c7dc8d1bc5f49cc5ab8639`  
		Last Modified: Sat, 26 Sep 2020 00:59:14 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aed66549b8e077f4709e4a810c54d9e77c8a3204b2b7a2b38cc6a75eb167ebd`  
		Last Modified: Sat, 26 Sep 2020 00:59:32 GMT  
		Size: 86.9 MB (86868980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df1086bca2359c48961a6a8509d2a87fbbce4e02d026d2fb6c71979c10ee73d`  
		Last Modified: Sat, 26 Sep 2020 00:59:14 GMT  
		Size: 5.1 KB (5055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eec6d6b82171ba862286f1be69df53aa151d327533c291e4de3b0ff2b1a17db`  
		Last Modified: Sat, 26 Sep 2020 00:59:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dd0778c8a1c593a11d73370ba6e1d667d60d0db647342e7ae06bfcc4eb09fc98
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121149179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1aebd936b3f97280ebde816dc6a608bacc3132c9c2a434b046d1f6b16bbec2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:59 GMT
ADD file:e1079b8987ad959c6a83dae1ea4446405953ab16899c693d57c6214ff888e688 in / 
# Fri, 25 Sep 2020 22:48:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:48:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:48:06 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:26:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:27:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:27:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:27:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:27:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:30 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:27:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:28:28 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 25 Sep 2020 23:28:29 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Fri, 25 Sep 2020 23:28:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:29:17 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:29:19 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:29:20 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:29:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Sep 2020 23:29:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:29:23 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:29:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a25fe36305380fa444fa6bd15b622145ff6076e5b6f81168d6cb4c9fee725863`  
		Last Modified: Fri, 25 Sep 2020 08:25:35 GMT  
		Size: 27.2 MB (27160123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326fa3abf0610ea05b9deb392e05c6c86a7afed0c119987a8d920a2a8dceaffc`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b87601e0a324569be2cebc4c0b9981bd53925a9bee894fad57c93f9bd3d01`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a280fab3f6130dcd17011ffa4ee6cb14fd04623b4c1e16f378026844b8f428`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b33bb77d692ee1db553b82b566c91f41b6dbfd76e9ba9eaa444b7ca545fe6`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 5.5 MB (5456069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c36f1baced17c5bd6b814a182f023308e1b4cda8870bf91756041505870fa2a`  
		Last Modified: Fri, 25 Sep 2020 23:34:27 GMT  
		Size: 1.3 MB (1261421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a2b365d2a0b2769c317ffcde3ef8699d4d7c3256f95021f1da0d979006c1dc`  
		Last Modified: Fri, 25 Sep 2020 23:34:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f8ac108760bfd505fbfd1b252d7cea8e1c95895d04a6de0fb125d757c67f23`  
		Last Modified: Fri, 25 Sep 2020 23:34:25 GMT  
		Size: 1.3 MB (1265577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91718a6772cfde37e00ab454ab0fe8081399c122f22de9c2cc6b578dfe810cf6`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c92fe8fee7a0b55d9e228c7a2fd7a249c8ffae66c8dd4f6e48681d431b905a9`  
		Last Modified: Fri, 25 Sep 2020 23:35:09 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46d6d103a32439e7956459a1d8c564be014d0127d15f6d7601b1547ffb46dcf`  
		Last Modified: Fri, 25 Sep 2020 23:35:34 GMT  
		Size: 86.0 MB (85995064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b55ae113bedf652da33213ca01e2304682c03fab920876bfddd8cb4322751c4`  
		Last Modified: Fri, 25 Sep 2020 23:35:09 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9191be867cd0fbee52b3a634ab8ea2845432c6f5076552c3b8fc4da0b77d3a13`  
		Last Modified: Fri, 25 Sep 2020 23:35:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a4a927d9dc128217cc28e4e023e3d94735aee608926168b5c41057fe3b343e65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133487617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c0223e2d920b5fc07998502f2eb82311985e6c48f30a0f4ad3fc74c7c7c11f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:53:28 GMT
ADD file:5479628763eb7f8cd884270bc1e9bb40ce39f1fb3427e863b086511696fa8107 in / 
# Fri, 25 Sep 2020 23:53:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:54:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:54:31 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:13:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:13:26 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:14:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:14:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:14:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:14:59 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:15:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:18:41 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 26 Sep 2020 04:18:44 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Sat, 26 Sep 2020 04:18:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:20:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:20:56 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:20:57 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:21:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Sep 2020 04:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:21:08 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:21:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af5e190551614a549619ca2cb11a237bf566e7b0942eac80adaf05e21644ad12`  
		Last Modified: Sat, 26 Sep 2020 00:06:58 GMT  
		Size: 33.3 MB (33278058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dd7d43fa9f545a3f69e66ff00d1a2773213cdfc18d0c99a71bb1c40bbb1f8c`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1feb93b9aa176877a7ec845345f281fe28c37605e03363dd0fa489bf0bf10ee`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72de4183a4e4f8be028bd4096c22189718c23c7af3d8206f6119c7e672403f5b`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd855440835f9cbdc109164d975673b33c12064da301ac86019019bf4457e2a6`  
		Last Modified: Sat, 26 Sep 2020 04:34:10 GMT  
		Size: 6.7 MB (6668533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc681828d8ea74c541ead13581fa9a5b5aa4c9bd5f23a49edb457fbfef07fad`  
		Last Modified: Sat, 26 Sep 2020 04:34:03 GMT  
		Size: 1.2 MB (1243770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be85c8ddabd72fe111c44f1aa3f8c03e84ab9e12b95ecaf8e14bc19cd8ce63d6`  
		Last Modified: Sat, 26 Sep 2020 04:34:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333eecf00fdea344bb79b6958cbd01f130119d2a12a3b7bcb698262191b0faa`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.3 MB (1273578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b192cad172b5465b46c838d6ed65009da808af10327870e10ca3dc21dfabd797`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3083778fe68309e214cb27ddc2835f4400ffecbae0307d95e0204edda4a57d45`  
		Last Modified: Sat, 26 Sep 2020 04:35:21 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb33f57f5e78e802612bf5c550f320f5db73a97b30fd59a4a9858e7979ab1563`  
		Last Modified: Sat, 26 Sep 2020 04:35:42 GMT  
		Size: 91.0 MB (91012743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497d7737768b7172015f8a6cc1aa2c78db159dcce10ca6a3ae5a3b5486fed14e`  
		Last Modified: Sat, 26 Sep 2020 04:35:21 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1544c05fda9cafb8d5ee2a9bd7c0435abe9e0143abd38a1d971181084cd882a`  
		Last Modified: Sat, 26 Sep 2020 04:35:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:9d27dd15564ba13a8ffa93beee20b39b7c14218c47ea296c6e11878a77962d12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:6955c063991fc6ee57fc0ba1b3b3de70408518df55af0c294323ff7d1ee974ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125549894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41fa9265d4dfb214f0a79ee919392687d09babc3522df21fce946292f9c8149c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:34:27 GMT
ADD file:da80f59399481ffc32f84353830dcf598f31a97785222e75d643bfb8a9aa14e7 in / 
# Fri, 25 Sep 2020 22:34:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:34:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:34:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:34:30 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:52:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:53:04 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:53:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:53:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:53:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:19 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:53:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:53:21 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 26 Sep 2020 00:53:21 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Sat, 26 Sep 2020 00:53:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:53:48 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:53:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:53:49 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:53:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:53:49 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:53:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d72e567cc804d0b637182ba23f8b9ffe101e753a39bf52cd4db6b89eb089f13b`  
		Last Modified: Fri, 25 Sep 2020 15:20:50 GMT  
		Size: 28.6 MB (28558050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3630e5ff08d73b6ec0e22736a5c8d2d666e7b568c16f6a4ffadf8c21b9b1ad`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a83d81d1f4f942d37e1f17195d9c519969ed3040fc3e444740b884e44dec33`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf2111ecf0efaa19887c07ce1ae8332ebff5775482731d8e524898d9fc07e23`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d64978a09242b12c715a8cfda3ce4ac4ef1e086016ccb32edb185f844363`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 5.5 MB (5488523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc9953bffb3c364d00df0e3961c569c5eebc2015cabee42cb7e0b33c4ba6891`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 1.3 MB (1324124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de429570dda5816121294e9251d2cf7f258f2a0c9fdf2a7ba9a7ebe56a763e83`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3652bc6ea9f9147ae99d11202e416c096df524bf3a64b6f483adb8d54e59a4a0`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 1.3 MB (1265989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4bf87041c8ad8ddf97dbbb645685d428963abc9d376dc413e6f7ee202af1ab`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb9bba22391ff2e85884b55109ea43a161c4bc348203f3a388ed71d94544a1c`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de10906fc5c385f1393d3e151fbb623b08796f6ffb8aacc998872c1d2e3805b`  
		Last Modified: Sat, 26 Sep 2020 00:59:06 GMT  
		Size: 88.9 MB (88902466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3a798c7a1f734389ff2ef70f8b27635b57c8cccb49f740e3bbce6c4992d01b`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0c0109b388d5a2b49159cfc84ef349261097968ef7143bd552cfa99297f215c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123202059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:715582b8771e15f883d2a7059abb63449fc21a84740b7c25adefe91051c4d7ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:59 GMT
ADD file:e1079b8987ad959c6a83dae1ea4446405953ab16899c693d57c6214ff888e688 in / 
# Fri, 25 Sep 2020 22:48:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:48:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:48:06 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:26:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:27:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:27:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:27:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:27:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:30 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:27:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:27:33 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Sep 2020 23:27:34 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Fri, 25 Sep 2020 23:27:36 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:28:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:28:13 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:28:14 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:28:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:28:15 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:28:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a25fe36305380fa444fa6bd15b622145ff6076e5b6f81168d6cb4c9fee725863`  
		Last Modified: Fri, 25 Sep 2020 08:25:35 GMT  
		Size: 27.2 MB (27160123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326fa3abf0610ea05b9deb392e05c6c86a7afed0c119987a8d920a2a8dceaffc`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b87601e0a324569be2cebc4c0b9981bd53925a9bee894fad57c93f9bd3d01`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a280fab3f6130dcd17011ffa4ee6cb14fd04623b4c1e16f378026844b8f428`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b33bb77d692ee1db553b82b566c91f41b6dbfd76e9ba9eaa444b7ca545fe6`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 5.5 MB (5456069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c36f1baced17c5bd6b814a182f023308e1b4cda8870bf91756041505870fa2a`  
		Last Modified: Fri, 25 Sep 2020 23:34:27 GMT  
		Size: 1.3 MB (1261421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a2b365d2a0b2769c317ffcde3ef8699d4d7c3256f95021f1da0d979006c1dc`  
		Last Modified: Fri, 25 Sep 2020 23:34:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f8ac108760bfd505fbfd1b252d7cea8e1c95895d04a6de0fb125d757c67f23`  
		Last Modified: Fri, 25 Sep 2020 23:34:25 GMT  
		Size: 1.3 MB (1265577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91718a6772cfde37e00ab454ab0fe8081399c122f22de9c2cc6b578dfe810cf6`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562cf16ec0a88e52ae3c5f14f4a083a1dd7273b805e0071f0f89c51e59048334`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6696e516bd6a98c3918decf8e7d83de51e39abe14588bb4126ea4835ff3da81`  
		Last Modified: Fri, 25 Sep 2020 23:34:49 GMT  
		Size: 88.0 MB (88048066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c1c05478213ecb540b9d3128078c6de920ca362b457bb22c70ba679b7932b`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d25388c779e56637ae42d217e4b826f491165a4d17d590c5d73333c68ef8c37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135600789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7c404662a55bba19439eed02cd8c4c40b348ba4646235804e46169051f2993`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:53:28 GMT
ADD file:5479628763eb7f8cd884270bc1e9bb40ce39f1fb3427e863b086511696fa8107 in / 
# Fri, 25 Sep 2020 23:53:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:54:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:54:31 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:13:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:13:26 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:14:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:14:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:14:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:14:59 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:15:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:15:09 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 26 Sep 2020 04:15:13 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Sat, 26 Sep 2020 04:15:19 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:18:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:18:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:18:16 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:18:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:18:23 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:18:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af5e190551614a549619ca2cb11a237bf566e7b0942eac80adaf05e21644ad12`  
		Last Modified: Sat, 26 Sep 2020 00:06:58 GMT  
		Size: 33.3 MB (33278058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dd7d43fa9f545a3f69e66ff00d1a2773213cdfc18d0c99a71bb1c40bbb1f8c`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1feb93b9aa176877a7ec845345f281fe28c37605e03363dd0fa489bf0bf10ee`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72de4183a4e4f8be028bd4096c22189718c23c7af3d8206f6119c7e672403f5b`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd855440835f9cbdc109164d975673b33c12064da301ac86019019bf4457e2a6`  
		Last Modified: Sat, 26 Sep 2020 04:34:10 GMT  
		Size: 6.7 MB (6668533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc681828d8ea74c541ead13581fa9a5b5aa4c9bd5f23a49edb457fbfef07fad`  
		Last Modified: Sat, 26 Sep 2020 04:34:03 GMT  
		Size: 1.2 MB (1243770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be85c8ddabd72fe111c44f1aa3f8c03e84ab9e12b95ecaf8e14bc19cd8ce63d6`  
		Last Modified: Sat, 26 Sep 2020 04:34:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333eecf00fdea344bb79b6958cbd01f130119d2a12a3b7bcb698262191b0faa`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.3 MB (1273578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b192cad172b5465b46c838d6ed65009da808af10327870e10ca3dc21dfabd797`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219ea6186c99102a7c952eabf22c03f79b9526307599b559a653375cba47467f`  
		Last Modified: Sat, 26 Sep 2020 04:33:55 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3620f102186fd21942b809f0f350a92a5d2206665bf4e1e78b2b4ad71a773101`  
		Last Modified: Sat, 26 Sep 2020 04:34:52 GMT  
		Size: 93.1 MB (93126036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661e28fa187e787cae957c2bc54772ad07a9afca94ecf7c488f10f19fc31d17d`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.6`

**does not exist** (yet?)

## `mariadb:10.5.6-focal`

**does not exist** (yet?)

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:9d27dd15564ba13a8ffa93beee20b39b7c14218c47ea296c6e11878a77962d12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:6955c063991fc6ee57fc0ba1b3b3de70408518df55af0c294323ff7d1ee974ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125549894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41fa9265d4dfb214f0a79ee919392687d09babc3522df21fce946292f9c8149c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:34:27 GMT
ADD file:da80f59399481ffc32f84353830dcf598f31a97785222e75d643bfb8a9aa14e7 in / 
# Fri, 25 Sep 2020 22:34:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:34:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:34:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:34:30 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:52:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:53:04 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:53:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:53:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:53:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:19 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:53:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:53:21 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 26 Sep 2020 00:53:21 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Sat, 26 Sep 2020 00:53:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:53:48 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:53:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:53:49 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:53:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:53:49 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:53:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d72e567cc804d0b637182ba23f8b9ffe101e753a39bf52cd4db6b89eb089f13b`  
		Last Modified: Fri, 25 Sep 2020 15:20:50 GMT  
		Size: 28.6 MB (28558050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3630e5ff08d73b6ec0e22736a5c8d2d666e7b568c16f6a4ffadf8c21b9b1ad`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a83d81d1f4f942d37e1f17195d9c519969ed3040fc3e444740b884e44dec33`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf2111ecf0efaa19887c07ce1ae8332ebff5775482731d8e524898d9fc07e23`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d64978a09242b12c715a8cfda3ce4ac4ef1e086016ccb32edb185f844363`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 5.5 MB (5488523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc9953bffb3c364d00df0e3961c569c5eebc2015cabee42cb7e0b33c4ba6891`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 1.3 MB (1324124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de429570dda5816121294e9251d2cf7f258f2a0c9fdf2a7ba9a7ebe56a763e83`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3652bc6ea9f9147ae99d11202e416c096df524bf3a64b6f483adb8d54e59a4a0`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 1.3 MB (1265989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4bf87041c8ad8ddf97dbbb645685d428963abc9d376dc413e6f7ee202af1ab`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb9bba22391ff2e85884b55109ea43a161c4bc348203f3a388ed71d94544a1c`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de10906fc5c385f1393d3e151fbb623b08796f6ffb8aacc998872c1d2e3805b`  
		Last Modified: Sat, 26 Sep 2020 00:59:06 GMT  
		Size: 88.9 MB (88902466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3a798c7a1f734389ff2ef70f8b27635b57c8cccb49f740e3bbce6c4992d01b`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0c0109b388d5a2b49159cfc84ef349261097968ef7143bd552cfa99297f215c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123202059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:715582b8771e15f883d2a7059abb63449fc21a84740b7c25adefe91051c4d7ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:59 GMT
ADD file:e1079b8987ad959c6a83dae1ea4446405953ab16899c693d57c6214ff888e688 in / 
# Fri, 25 Sep 2020 22:48:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:48:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:48:06 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:26:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:27:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:27:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:27:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:27:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:30 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:27:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:27:33 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Sep 2020 23:27:34 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Fri, 25 Sep 2020 23:27:36 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:28:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:28:13 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:28:14 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:28:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:28:15 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:28:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a25fe36305380fa444fa6bd15b622145ff6076e5b6f81168d6cb4c9fee725863`  
		Last Modified: Fri, 25 Sep 2020 08:25:35 GMT  
		Size: 27.2 MB (27160123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326fa3abf0610ea05b9deb392e05c6c86a7afed0c119987a8d920a2a8dceaffc`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b87601e0a324569be2cebc4c0b9981bd53925a9bee894fad57c93f9bd3d01`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a280fab3f6130dcd17011ffa4ee6cb14fd04623b4c1e16f378026844b8f428`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b33bb77d692ee1db553b82b566c91f41b6dbfd76e9ba9eaa444b7ca545fe6`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 5.5 MB (5456069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c36f1baced17c5bd6b814a182f023308e1b4cda8870bf91756041505870fa2a`  
		Last Modified: Fri, 25 Sep 2020 23:34:27 GMT  
		Size: 1.3 MB (1261421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a2b365d2a0b2769c317ffcde3ef8699d4d7c3256f95021f1da0d979006c1dc`  
		Last Modified: Fri, 25 Sep 2020 23:34:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f8ac108760bfd505fbfd1b252d7cea8e1c95895d04a6de0fb125d757c67f23`  
		Last Modified: Fri, 25 Sep 2020 23:34:25 GMT  
		Size: 1.3 MB (1265577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91718a6772cfde37e00ab454ab0fe8081399c122f22de9c2cc6b578dfe810cf6`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562cf16ec0a88e52ae3c5f14f4a083a1dd7273b805e0071f0f89c51e59048334`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6696e516bd6a98c3918decf8e7d83de51e39abe14588bb4126ea4835ff3da81`  
		Last Modified: Fri, 25 Sep 2020 23:34:49 GMT  
		Size: 88.0 MB (88048066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c1c05478213ecb540b9d3128078c6de920ca362b457bb22c70ba679b7932b`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d25388c779e56637ae42d217e4b826f491165a4d17d590c5d73333c68ef8c37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135600789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7c404662a55bba19439eed02cd8c4c40b348ba4646235804e46169051f2993`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:53:28 GMT
ADD file:5479628763eb7f8cd884270bc1e9bb40ce39f1fb3427e863b086511696fa8107 in / 
# Fri, 25 Sep 2020 23:53:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:54:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:54:31 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:13:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:13:26 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:14:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:14:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:14:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:14:59 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:15:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:15:09 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 26 Sep 2020 04:15:13 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Sat, 26 Sep 2020 04:15:19 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:18:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:18:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:18:16 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:18:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:18:23 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:18:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af5e190551614a549619ca2cb11a237bf566e7b0942eac80adaf05e21644ad12`  
		Last Modified: Sat, 26 Sep 2020 00:06:58 GMT  
		Size: 33.3 MB (33278058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dd7d43fa9f545a3f69e66ff00d1a2773213cdfc18d0c99a71bb1c40bbb1f8c`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1feb93b9aa176877a7ec845345f281fe28c37605e03363dd0fa489bf0bf10ee`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72de4183a4e4f8be028bd4096c22189718c23c7af3d8206f6119c7e672403f5b`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd855440835f9cbdc109164d975673b33c12064da301ac86019019bf4457e2a6`  
		Last Modified: Sat, 26 Sep 2020 04:34:10 GMT  
		Size: 6.7 MB (6668533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc681828d8ea74c541ead13581fa9a5b5aa4c9bd5f23a49edb457fbfef07fad`  
		Last Modified: Sat, 26 Sep 2020 04:34:03 GMT  
		Size: 1.2 MB (1243770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be85c8ddabd72fe111c44f1aa3f8c03e84ab9e12b95ecaf8e14bc19cd8ce63d6`  
		Last Modified: Sat, 26 Sep 2020 04:34:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333eecf00fdea344bb79b6958cbd01f130119d2a12a3b7bcb698262191b0faa`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.3 MB (1273578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b192cad172b5465b46c838d6ed65009da808af10327870e10ca3dc21dfabd797`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219ea6186c99102a7c952eabf22c03f79b9526307599b559a653375cba47467f`  
		Last Modified: Sat, 26 Sep 2020 04:33:55 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3620f102186fd21942b809f0f350a92a5d2206665bf4e1e78b2b4ad71a773101`  
		Last Modified: Sat, 26 Sep 2020 04:34:52 GMT  
		Size: 93.1 MB (93126036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661e28fa187e787cae957c2bc54772ad07a9afca94ecf7c488f10f19fc31d17d`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:9d27dd15564ba13a8ffa93beee20b39b7c14218c47ea296c6e11878a77962d12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:6955c063991fc6ee57fc0ba1b3b3de70408518df55af0c294323ff7d1ee974ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125549894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41fa9265d4dfb214f0a79ee919392687d09babc3522df21fce946292f9c8149c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:34:27 GMT
ADD file:da80f59399481ffc32f84353830dcf598f31a97785222e75d643bfb8a9aa14e7 in / 
# Fri, 25 Sep 2020 22:34:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:34:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:34:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:34:30 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:52:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:53:04 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:53:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:53:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:53:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:19 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:53:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:53:21 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 26 Sep 2020 00:53:21 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Sat, 26 Sep 2020 00:53:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:53:48 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:53:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:53:49 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:53:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:53:49 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:53:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d72e567cc804d0b637182ba23f8b9ffe101e753a39bf52cd4db6b89eb089f13b`  
		Last Modified: Fri, 25 Sep 2020 15:20:50 GMT  
		Size: 28.6 MB (28558050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3630e5ff08d73b6ec0e22736a5c8d2d666e7b568c16f6a4ffadf8c21b9b1ad`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a83d81d1f4f942d37e1f17195d9c519969ed3040fc3e444740b884e44dec33`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf2111ecf0efaa19887c07ce1ae8332ebff5775482731d8e524898d9fc07e23`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d64978a09242b12c715a8cfda3ce4ac4ef1e086016ccb32edb185f844363`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 5.5 MB (5488523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc9953bffb3c364d00df0e3961c569c5eebc2015cabee42cb7e0b33c4ba6891`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 1.3 MB (1324124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de429570dda5816121294e9251d2cf7f258f2a0c9fdf2a7ba9a7ebe56a763e83`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3652bc6ea9f9147ae99d11202e416c096df524bf3a64b6f483adb8d54e59a4a0`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 1.3 MB (1265989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4bf87041c8ad8ddf97dbbb645685d428963abc9d376dc413e6f7ee202af1ab`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb9bba22391ff2e85884b55109ea43a161c4bc348203f3a388ed71d94544a1c`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de10906fc5c385f1393d3e151fbb623b08796f6ffb8aacc998872c1d2e3805b`  
		Last Modified: Sat, 26 Sep 2020 00:59:06 GMT  
		Size: 88.9 MB (88902466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3a798c7a1f734389ff2ef70f8b27635b57c8cccb49f740e3bbce6c4992d01b`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0c0109b388d5a2b49159cfc84ef349261097968ef7143bd552cfa99297f215c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123202059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:715582b8771e15f883d2a7059abb63449fc21a84740b7c25adefe91051c4d7ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:59 GMT
ADD file:e1079b8987ad959c6a83dae1ea4446405953ab16899c693d57c6214ff888e688 in / 
# Fri, 25 Sep 2020 22:48:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:48:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:48:06 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:26:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:27:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:27:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:27:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:27:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:30 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:27:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:27:33 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Sep 2020 23:27:34 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Fri, 25 Sep 2020 23:27:36 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:28:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:28:13 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:28:14 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:28:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:28:15 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:28:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a25fe36305380fa444fa6bd15b622145ff6076e5b6f81168d6cb4c9fee725863`  
		Last Modified: Fri, 25 Sep 2020 08:25:35 GMT  
		Size: 27.2 MB (27160123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326fa3abf0610ea05b9deb392e05c6c86a7afed0c119987a8d920a2a8dceaffc`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b87601e0a324569be2cebc4c0b9981bd53925a9bee894fad57c93f9bd3d01`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a280fab3f6130dcd17011ffa4ee6cb14fd04623b4c1e16f378026844b8f428`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b33bb77d692ee1db553b82b566c91f41b6dbfd76e9ba9eaa444b7ca545fe6`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 5.5 MB (5456069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c36f1baced17c5bd6b814a182f023308e1b4cda8870bf91756041505870fa2a`  
		Last Modified: Fri, 25 Sep 2020 23:34:27 GMT  
		Size: 1.3 MB (1261421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a2b365d2a0b2769c317ffcde3ef8699d4d7c3256f95021f1da0d979006c1dc`  
		Last Modified: Fri, 25 Sep 2020 23:34:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f8ac108760bfd505fbfd1b252d7cea8e1c95895d04a6de0fb125d757c67f23`  
		Last Modified: Fri, 25 Sep 2020 23:34:25 GMT  
		Size: 1.3 MB (1265577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91718a6772cfde37e00ab454ab0fe8081399c122f22de9c2cc6b578dfe810cf6`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562cf16ec0a88e52ae3c5f14f4a083a1dd7273b805e0071f0f89c51e59048334`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6696e516bd6a98c3918decf8e7d83de51e39abe14588bb4126ea4835ff3da81`  
		Last Modified: Fri, 25 Sep 2020 23:34:49 GMT  
		Size: 88.0 MB (88048066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c1c05478213ecb540b9d3128078c6de920ca362b457bb22c70ba679b7932b`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d25388c779e56637ae42d217e4b826f491165a4d17d590c5d73333c68ef8c37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135600789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7c404662a55bba19439eed02cd8c4c40b348ba4646235804e46169051f2993`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:53:28 GMT
ADD file:5479628763eb7f8cd884270bc1e9bb40ce39f1fb3427e863b086511696fa8107 in / 
# Fri, 25 Sep 2020 23:53:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:54:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:54:31 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:13:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:13:26 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:14:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:14:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:14:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:14:59 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:15:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:15:09 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 26 Sep 2020 04:15:13 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Sat, 26 Sep 2020 04:15:19 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:18:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:18:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:18:16 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:18:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:18:23 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:18:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af5e190551614a549619ca2cb11a237bf566e7b0942eac80adaf05e21644ad12`  
		Last Modified: Sat, 26 Sep 2020 00:06:58 GMT  
		Size: 33.3 MB (33278058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dd7d43fa9f545a3f69e66ff00d1a2773213cdfc18d0c99a71bb1c40bbb1f8c`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1feb93b9aa176877a7ec845345f281fe28c37605e03363dd0fa489bf0bf10ee`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72de4183a4e4f8be028bd4096c22189718c23c7af3d8206f6119c7e672403f5b`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd855440835f9cbdc109164d975673b33c12064da301ac86019019bf4457e2a6`  
		Last Modified: Sat, 26 Sep 2020 04:34:10 GMT  
		Size: 6.7 MB (6668533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc681828d8ea74c541ead13581fa9a5b5aa4c9bd5f23a49edb457fbfef07fad`  
		Last Modified: Sat, 26 Sep 2020 04:34:03 GMT  
		Size: 1.2 MB (1243770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be85c8ddabd72fe111c44f1aa3f8c03e84ab9e12b95ecaf8e14bc19cd8ce63d6`  
		Last Modified: Sat, 26 Sep 2020 04:34:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333eecf00fdea344bb79b6958cbd01f130119d2a12a3b7bcb698262191b0faa`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.3 MB (1273578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b192cad172b5465b46c838d6ed65009da808af10327870e10ca3dc21dfabd797`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219ea6186c99102a7c952eabf22c03f79b9526307599b559a653375cba47467f`  
		Last Modified: Sat, 26 Sep 2020 04:33:55 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3620f102186fd21942b809f0f350a92a5d2206665bf4e1e78b2b4ad71a773101`  
		Last Modified: Sat, 26 Sep 2020 04:34:52 GMT  
		Size: 93.1 MB (93126036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661e28fa187e787cae957c2bc54772ad07a9afca94ecf7c488f10f19fc31d17d`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:9d27dd15564ba13a8ffa93beee20b39b7c14218c47ea296c6e11878a77962d12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:6955c063991fc6ee57fc0ba1b3b3de70408518df55af0c294323ff7d1ee974ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125549894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41fa9265d4dfb214f0a79ee919392687d09babc3522df21fce946292f9c8149c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:34:27 GMT
ADD file:da80f59399481ffc32f84353830dcf598f31a97785222e75d643bfb8a9aa14e7 in / 
# Fri, 25 Sep 2020 22:34:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:34:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:34:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:34:30 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:52:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:53:04 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:53:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:53:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:53:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:19 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:53:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:53:21 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 26 Sep 2020 00:53:21 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Sat, 26 Sep 2020 00:53:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:53:48 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:53:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:53:49 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:53:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:53:49 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:53:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d72e567cc804d0b637182ba23f8b9ffe101e753a39bf52cd4db6b89eb089f13b`  
		Last Modified: Fri, 25 Sep 2020 15:20:50 GMT  
		Size: 28.6 MB (28558050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3630e5ff08d73b6ec0e22736a5c8d2d666e7b568c16f6a4ffadf8c21b9b1ad`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a83d81d1f4f942d37e1f17195d9c519969ed3040fc3e444740b884e44dec33`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf2111ecf0efaa19887c07ce1ae8332ebff5775482731d8e524898d9fc07e23`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d64978a09242b12c715a8cfda3ce4ac4ef1e086016ccb32edb185f844363`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 5.5 MB (5488523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc9953bffb3c364d00df0e3961c569c5eebc2015cabee42cb7e0b33c4ba6891`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 1.3 MB (1324124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de429570dda5816121294e9251d2cf7f258f2a0c9fdf2a7ba9a7ebe56a763e83`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3652bc6ea9f9147ae99d11202e416c096df524bf3a64b6f483adb8d54e59a4a0`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 1.3 MB (1265989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4bf87041c8ad8ddf97dbbb645685d428963abc9d376dc413e6f7ee202af1ab`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb9bba22391ff2e85884b55109ea43a161c4bc348203f3a388ed71d94544a1c`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de10906fc5c385f1393d3e151fbb623b08796f6ffb8aacc998872c1d2e3805b`  
		Last Modified: Sat, 26 Sep 2020 00:59:06 GMT  
		Size: 88.9 MB (88902466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3a798c7a1f734389ff2ef70f8b27635b57c8cccb49f740e3bbce6c4992d01b`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0c0109b388d5a2b49159cfc84ef349261097968ef7143bd552cfa99297f215c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123202059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:715582b8771e15f883d2a7059abb63449fc21a84740b7c25adefe91051c4d7ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:59 GMT
ADD file:e1079b8987ad959c6a83dae1ea4446405953ab16899c693d57c6214ff888e688 in / 
# Fri, 25 Sep 2020 22:48:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:48:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:48:06 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:26:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:27:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:27:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:27:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:27:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:30 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:27:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:27:33 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Sep 2020 23:27:34 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Fri, 25 Sep 2020 23:27:36 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:28:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:28:13 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:28:14 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:28:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:28:15 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:28:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a25fe36305380fa444fa6bd15b622145ff6076e5b6f81168d6cb4c9fee725863`  
		Last Modified: Fri, 25 Sep 2020 08:25:35 GMT  
		Size: 27.2 MB (27160123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326fa3abf0610ea05b9deb392e05c6c86a7afed0c119987a8d920a2a8dceaffc`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b87601e0a324569be2cebc4c0b9981bd53925a9bee894fad57c93f9bd3d01`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a280fab3f6130dcd17011ffa4ee6cb14fd04623b4c1e16f378026844b8f428`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b33bb77d692ee1db553b82b566c91f41b6dbfd76e9ba9eaa444b7ca545fe6`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 5.5 MB (5456069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c36f1baced17c5bd6b814a182f023308e1b4cda8870bf91756041505870fa2a`  
		Last Modified: Fri, 25 Sep 2020 23:34:27 GMT  
		Size: 1.3 MB (1261421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a2b365d2a0b2769c317ffcde3ef8699d4d7c3256f95021f1da0d979006c1dc`  
		Last Modified: Fri, 25 Sep 2020 23:34:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f8ac108760bfd505fbfd1b252d7cea8e1c95895d04a6de0fb125d757c67f23`  
		Last Modified: Fri, 25 Sep 2020 23:34:25 GMT  
		Size: 1.3 MB (1265577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91718a6772cfde37e00ab454ab0fe8081399c122f22de9c2cc6b578dfe810cf6`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562cf16ec0a88e52ae3c5f14f4a083a1dd7273b805e0071f0f89c51e59048334`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6696e516bd6a98c3918decf8e7d83de51e39abe14588bb4126ea4835ff3da81`  
		Last Modified: Fri, 25 Sep 2020 23:34:49 GMT  
		Size: 88.0 MB (88048066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c1c05478213ecb540b9d3128078c6de920ca362b457bb22c70ba679b7932b`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d25388c779e56637ae42d217e4b826f491165a4d17d590c5d73333c68ef8c37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135600789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7c404662a55bba19439eed02cd8c4c40b348ba4646235804e46169051f2993`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:53:28 GMT
ADD file:5479628763eb7f8cd884270bc1e9bb40ce39f1fb3427e863b086511696fa8107 in / 
# Fri, 25 Sep 2020 23:53:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:54:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:54:31 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:13:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:13:26 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:14:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:14:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:14:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:14:59 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:15:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:15:09 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 26 Sep 2020 04:15:13 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Sat, 26 Sep 2020 04:15:19 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:18:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:18:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:18:16 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:18:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:18:23 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:18:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af5e190551614a549619ca2cb11a237bf566e7b0942eac80adaf05e21644ad12`  
		Last Modified: Sat, 26 Sep 2020 00:06:58 GMT  
		Size: 33.3 MB (33278058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dd7d43fa9f545a3f69e66ff00d1a2773213cdfc18d0c99a71bb1c40bbb1f8c`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1feb93b9aa176877a7ec845345f281fe28c37605e03363dd0fa489bf0bf10ee`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72de4183a4e4f8be028bd4096c22189718c23c7af3d8206f6119c7e672403f5b`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd855440835f9cbdc109164d975673b33c12064da301ac86019019bf4457e2a6`  
		Last Modified: Sat, 26 Sep 2020 04:34:10 GMT  
		Size: 6.7 MB (6668533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc681828d8ea74c541ead13581fa9a5b5aa4c9bd5f23a49edb457fbfef07fad`  
		Last Modified: Sat, 26 Sep 2020 04:34:03 GMT  
		Size: 1.2 MB (1243770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be85c8ddabd72fe111c44f1aa3f8c03e84ab9e12b95ecaf8e14bc19cd8ce63d6`  
		Last Modified: Sat, 26 Sep 2020 04:34:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333eecf00fdea344bb79b6958cbd01f130119d2a12a3b7bcb698262191b0faa`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.3 MB (1273578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b192cad172b5465b46c838d6ed65009da808af10327870e10ca3dc21dfabd797`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219ea6186c99102a7c952eabf22c03f79b9526307599b559a653375cba47467f`  
		Last Modified: Sat, 26 Sep 2020 04:33:55 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3620f102186fd21942b809f0f350a92a5d2206665bf4e1e78b2b4ad71a773101`  
		Last Modified: Sat, 26 Sep 2020 04:34:52 GMT  
		Size: 93.1 MB (93126036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661e28fa187e787cae957c2bc54772ad07a9afca94ecf7c488f10f19fc31d17d`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:9d27dd15564ba13a8ffa93beee20b39b7c14218c47ea296c6e11878a77962d12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:6955c063991fc6ee57fc0ba1b3b3de70408518df55af0c294323ff7d1ee974ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125549894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41fa9265d4dfb214f0a79ee919392687d09babc3522df21fce946292f9c8149c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:34:27 GMT
ADD file:da80f59399481ffc32f84353830dcf598f31a97785222e75d643bfb8a9aa14e7 in / 
# Fri, 25 Sep 2020 22:34:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:34:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:34:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:34:30 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 00:52:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 00:53:04 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 00:53:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 00:53:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 00:53:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 00:53:19 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 00:53:21 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 00:53:21 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 26 Sep 2020 00:53:21 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Sat, 26 Sep 2020 00:53:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 00:53:48 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 00:53:49 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 00:53:49 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 00:53:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 00:53:49 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 00:53:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d72e567cc804d0b637182ba23f8b9ffe101e753a39bf52cd4db6b89eb089f13b`  
		Last Modified: Fri, 25 Sep 2020 15:20:50 GMT  
		Size: 28.6 MB (28558050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3630e5ff08d73b6ec0e22736a5c8d2d666e7b568c16f6a4ffadf8c21b9b1ad`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a83d81d1f4f942d37e1f17195d9c519969ed3040fc3e444740b884e44dec33`  
		Last Modified: Fri, 25 Sep 2020 22:36:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf2111ecf0efaa19887c07ce1ae8332ebff5775482731d8e524898d9fc07e23`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9572d64978a09242b12c715a8cfda3ce4ac4ef1e086016ccb32edb185f844363`  
		Last Modified: Sat, 26 Sep 2020 00:58:53 GMT  
		Size: 5.5 MB (5488523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc9953bffb3c364d00df0e3961c569c5eebc2015cabee42cb7e0b33c4ba6891`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 1.3 MB (1324124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de429570dda5816121294e9251d2cf7f258f2a0c9fdf2a7ba9a7ebe56a763e83`  
		Last Modified: Sat, 26 Sep 2020 00:58:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3652bc6ea9f9147ae99d11202e416c096df524bf3a64b6f483adb8d54e59a4a0`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 1.3 MB (1265989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4bf87041c8ad8ddf97dbbb645685d428963abc9d376dc413e6f7ee202af1ab`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb9bba22391ff2e85884b55109ea43a161c4bc348203f3a388ed71d94544a1c`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de10906fc5c385f1393d3e151fbb623b08796f6ffb8aacc998872c1d2e3805b`  
		Last Modified: Sat, 26 Sep 2020 00:59:06 GMT  
		Size: 88.9 MB (88902466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3a798c7a1f734389ff2ef70f8b27635b57c8cccb49f740e3bbce6c4992d01b`  
		Last Modified: Sat, 26 Sep 2020 00:58:51 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0c0109b388d5a2b49159cfc84ef349261097968ef7143bd552cfa99297f215c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123202059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:715582b8771e15f883d2a7059abb63449fc21a84740b7c25adefe91051c4d7ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:59 GMT
ADD file:e1079b8987ad959c6a83dae1ea4446405953ab16899c693d57c6214ff888e688 in / 
# Fri, 25 Sep 2020 22:48:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:48:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:48:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:48:06 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:26:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:27:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:01 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:27:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:27:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:27:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:27:30 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:27:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:27:33 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Sep 2020 23:27:34 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Fri, 25 Sep 2020 23:27:36 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Sep 2020 23:28:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 25 Sep 2020 23:28:13 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Sep 2020 23:28:14 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:28:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Sep 2020 23:28:15 GMT
EXPOSE 3306
# Fri, 25 Sep 2020 23:28:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a25fe36305380fa444fa6bd15b622145ff6076e5b6f81168d6cb4c9fee725863`  
		Last Modified: Fri, 25 Sep 2020 08:25:35 GMT  
		Size: 27.2 MB (27160123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326fa3abf0610ea05b9deb392e05c6c86a7afed0c119987a8d920a2a8dceaffc`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1b87601e0a324569be2cebc4c0b9981bd53925a9bee894fad57c93f9bd3d01`  
		Last Modified: Fri, 25 Sep 2020 22:49:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a280fab3f6130dcd17011ffa4ee6cb14fd04623b4c1e16f378026844b8f428`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01b33bb77d692ee1db553b82b566c91f41b6dbfd76e9ba9eaa444b7ca545fe6`  
		Last Modified: Fri, 25 Sep 2020 23:34:28 GMT  
		Size: 5.5 MB (5456069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c36f1baced17c5bd6b814a182f023308e1b4cda8870bf91756041505870fa2a`  
		Last Modified: Fri, 25 Sep 2020 23:34:27 GMT  
		Size: 1.3 MB (1261421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a2b365d2a0b2769c317ffcde3ef8699d4d7c3256f95021f1da0d979006c1dc`  
		Last Modified: Fri, 25 Sep 2020 23:34:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f8ac108760bfd505fbfd1b252d7cea8e1c95895d04a6de0fb125d757c67f23`  
		Last Modified: Fri, 25 Sep 2020 23:34:25 GMT  
		Size: 1.3 MB (1265577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91718a6772cfde37e00ab454ab0fe8081399c122f22de9c2cc6b578dfe810cf6`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562cf16ec0a88e52ae3c5f14f4a083a1dd7273b805e0071f0f89c51e59048334`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6696e516bd6a98c3918decf8e7d83de51e39abe14588bb4126ea4835ff3da81`  
		Last Modified: Fri, 25 Sep 2020 23:34:49 GMT  
		Size: 88.0 MB (88048066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c1c05478213ecb540b9d3128078c6de920ca362b457bb22c70ba679b7932b`  
		Last Modified: Fri, 25 Sep 2020 23:34:24 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d25388c779e56637ae42d217e4b826f491165a4d17d590c5d73333c68ef8c37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135600789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7c404662a55bba19439eed02cd8c4c40b348ba4646235804e46169051f2993`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:53:28 GMT
ADD file:5479628763eb7f8cd884270bc1e9bb40ce39f1fb3427e863b086511696fa8107 in / 
# Fri, 25 Sep 2020 23:53:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:54:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:54:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:54:31 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:10:52 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:13:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:13:26 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:14:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:14:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:14:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:14:59 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:15:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:15:09 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 26 Sep 2020 04:15:13 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Sat, 26 Sep 2020 04:15:19 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 26 Sep 2020 04:18:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 26 Sep 2020 04:18:15 GMT
VOLUME [/var/lib/mysql]
# Sat, 26 Sep 2020 04:18:16 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Sat, 26 Sep 2020 04:18:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Sep 2020 04:18:23 GMT
EXPOSE 3306
# Sat, 26 Sep 2020 04:18:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af5e190551614a549619ca2cb11a237bf566e7b0942eac80adaf05e21644ad12`  
		Last Modified: Sat, 26 Sep 2020 00:06:58 GMT  
		Size: 33.3 MB (33278058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dd7d43fa9f545a3f69e66ff00d1a2773213cdfc18d0c99a71bb1c40bbb1f8c`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1feb93b9aa176877a7ec845345f281fe28c37605e03363dd0fa489bf0bf10ee`  
		Last Modified: Sat, 26 Sep 2020 00:06:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72de4183a4e4f8be028bd4096c22189718c23c7af3d8206f6119c7e672403f5b`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd855440835f9cbdc109164d975673b33c12064da301ac86019019bf4457e2a6`  
		Last Modified: Sat, 26 Sep 2020 04:34:10 GMT  
		Size: 6.7 MB (6668533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc681828d8ea74c541ead13581fa9a5b5aa4c9bd5f23a49edb457fbfef07fad`  
		Last Modified: Sat, 26 Sep 2020 04:34:03 GMT  
		Size: 1.2 MB (1243770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be85c8ddabd72fe111c44f1aa3f8c03e84ab9e12b95ecaf8e14bc19cd8ce63d6`  
		Last Modified: Sat, 26 Sep 2020 04:34:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333eecf00fdea344bb79b6958cbd01f130119d2a12a3b7bcb698262191b0faa`  
		Last Modified: Sat, 26 Sep 2020 04:34:05 GMT  
		Size: 1.3 MB (1273578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b192cad172b5465b46c838d6ed65009da808af10327870e10ca3dc21dfabd797`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219ea6186c99102a7c952eabf22c03f79b9526307599b559a653375cba47467f`  
		Last Modified: Sat, 26 Sep 2020 04:33:55 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3620f102186fd21942b809f0f350a92a5d2206665bf4e1e78b2b4ad71a773101`  
		Last Modified: Sat, 26 Sep 2020 04:34:52 GMT  
		Size: 93.1 MB (93126036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661e28fa187e787cae957c2bc54772ad07a9afca94ecf7c488f10f19fc31d17d`  
		Last Modified: Sat, 26 Sep 2020 04:33:56 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
