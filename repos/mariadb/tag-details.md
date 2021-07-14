<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10-focal`](#mariadb10-focal)
-	[`mariadb:10.2`](#mariadb102)
-	[`mariadb:10.2-bionic`](#mariadb102-bionic)
-	[`mariadb:10.2.39`](#mariadb10239)
-	[`mariadb:10.2.39-bionic`](#mariadb10239-bionic)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.3.30`](#mariadb10330)
-	[`mariadb:10.3.30-focal`](#mariadb10330-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.4.20`](#mariadb10420)
-	[`mariadb:10.4.20-focal`](#mariadb10420-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10.5.11`](#mariadb10511)
-	[`mariadb:10.5.11-focal`](#mariadb10511-focal)
-	[`mariadb:10.6`](#mariadb106)
-	[`mariadb:10.6-focal`](#mariadb106-focal)
-	[`mariadb:10.6.3`](#mariadb1063)
-	[`mariadb:10.6.3-focal`](#mariadb1063-focal)
-	[`mariadb:focal`](#mariadbfocal)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:d91a1a362a01a4f26c5ed3b34a861f6c1f22a20176ff4a464902adfe8382bafd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:cc58d2e89470cd6dc792be7eef70f7cf8f5e9da89c00ed01b3a7f41dc31f6297
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127011672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24439278c77038c5acc032f1e40e737db054bd1e36551108b657a31ea9233860`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:22:13 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:22:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:22:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:22:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:22:57 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:22:58 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:22:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bab4b089ce1a692b2cd7379f70920f9bab6969ea344af112a507fa96b17dd7`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992059611ea5389c3a532956c7dccc37c13d8450c6fdb79b3d65f295bdf19c51`  
		Last Modified: Tue, 13 Jul 2021 18:27:08 GMT  
		Size: 87.1 MB (87102268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba030b7d27eab09343a23988d5e00d3bf1880edfb9962197a9c9fbfd89806ffe`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:239e4679d65d9a44c983072b52312f8cbfaf505a805090aa97d1a65266c82669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124305174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5769943918c67f6492a009979e758470c83b2de2a83d1716402f1d4009b78479`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:40:54 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:40:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:41:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:41:17 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:41:17 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:41:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:41:18 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:41:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a44c338f719da6a7548fc4e647b9bd52225c5df3e2302badd4a3636d4ada6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0477462ca83c7a80d659335ac0c0d7eadd33db5bf3497027907f7c417dd036c5`  
		Last Modified: Tue, 13 Jul 2021 23:45:32 GMT  
		Size: 86.1 MB (86099760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85af6cce3f74250abc9bdff500887dc7967e9af3afde38f6d863fde77572ed62`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e83376a3a79780723ee2f77623bca0817d59cac7d5edd216700e596ab9344b2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137504069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d483574e8cdb21e02f00261a7f79687f57f662824805f3a9b2c2d43e35ebf08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:26:26 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:32 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:36 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:41 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:26:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:31:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:32:08 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:32:16 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:32:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:32:27 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:32:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fef03d4d8ec5fdbff5a48b3b0bd2e4b89871abaea39af1025a6c3c13bc5a05`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99414d7cf31143b328d34986107ab9144e1e311e6bae8d5686c17b2a8faa43`  
		Last Modified: Tue, 13 Jul 2021 19:04:55 GMT  
		Size: 91.3 MB (91306505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704b6e12ccce455e8980f637eee2cc9c2dc93e364a9dc504ed7d1073f107f7d2`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:d91a1a362a01a4f26c5ed3b34a861f6c1f22a20176ff4a464902adfe8382bafd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:cc58d2e89470cd6dc792be7eef70f7cf8f5e9da89c00ed01b3a7f41dc31f6297
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127011672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24439278c77038c5acc032f1e40e737db054bd1e36551108b657a31ea9233860`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:22:13 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:22:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:22:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:22:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:22:57 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:22:58 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:22:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bab4b089ce1a692b2cd7379f70920f9bab6969ea344af112a507fa96b17dd7`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992059611ea5389c3a532956c7dccc37c13d8450c6fdb79b3d65f295bdf19c51`  
		Last Modified: Tue, 13 Jul 2021 18:27:08 GMT  
		Size: 87.1 MB (87102268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba030b7d27eab09343a23988d5e00d3bf1880edfb9962197a9c9fbfd89806ffe`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:239e4679d65d9a44c983072b52312f8cbfaf505a805090aa97d1a65266c82669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124305174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5769943918c67f6492a009979e758470c83b2de2a83d1716402f1d4009b78479`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:40:54 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:40:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:41:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:41:17 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:41:17 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:41:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:41:18 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:41:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a44c338f719da6a7548fc4e647b9bd52225c5df3e2302badd4a3636d4ada6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0477462ca83c7a80d659335ac0c0d7eadd33db5bf3497027907f7c417dd036c5`  
		Last Modified: Tue, 13 Jul 2021 23:45:32 GMT  
		Size: 86.1 MB (86099760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85af6cce3f74250abc9bdff500887dc7967e9af3afde38f6d863fde77572ed62`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e83376a3a79780723ee2f77623bca0817d59cac7d5edd216700e596ab9344b2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137504069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d483574e8cdb21e02f00261a7f79687f57f662824805f3a9b2c2d43e35ebf08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:26:26 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:32 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:36 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:41 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:26:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:31:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:32:08 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:32:16 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:32:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:32:27 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:32:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fef03d4d8ec5fdbff5a48b3b0bd2e4b89871abaea39af1025a6c3c13bc5a05`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99414d7cf31143b328d34986107ab9144e1e311e6bae8d5686c17b2a8faa43`  
		Last Modified: Tue, 13 Jul 2021 19:04:55 GMT  
		Size: 91.3 MB (91306505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704b6e12ccce455e8980f637eee2cc9c2dc93e364a9dc504ed7d1073f107f7d2`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:daaf37a722e689a8135b92bd849ef5787655edbc924b890ca8e6cad7fec8cb98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:612d0f034f206958a9c84b941883cb8c0f304109fb5011202e21a3f09d011c9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109301363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3268c71ffc39a8a97d50abc19e5f72880617cd2cb124ab871cbdc10ed2a08db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:59:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:59:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:24:48 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:25:13 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:25:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:23 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:25:23 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:25:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:25:25 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:25:25 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:25:26 GMT
ARG MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:25:26 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:25:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
# Tue, 13 Jul 2021 18:25:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:26:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:26:09 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:26:10 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:26:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:26:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:26:11 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:26:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d7f527a85d567884b86652e590f5d484b9ab84b150e4925b7d87699f93fea1`  
		Last Modified: Fri, 18 Jun 2021 05:03:42 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ffc1a82bccd839baf9aee65bea12f39144d2f71d17f7a478729e5033a3483e`  
		Last Modified: Fri, 18 Jun 2021 05:03:41 GMT  
		Size: 4.8 MB (4813831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11da2f34c9bc7201cc69fc1cd85b9e49e8cbb5294fb5f4ed482c36995965b114`  
		Last Modified: Tue, 13 Jul 2021 18:29:14 GMT  
		Size: 3.5 MB (3548102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa88816ca3dbb95dc4d440388a0689a08adfcae89926efc82e138406d30a6051`  
		Last Modified: Tue, 13 Jul 2021 18:29:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308022251dfd080c48afe0ce2efa6d93a302640ab9c5671ec4b1b13f68e44ff8`  
		Last Modified: Tue, 13 Jul 2021 18:29:14 GMT  
		Size: 1.6 MB (1586331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6e8acfd55976b0551283d6d0b4d5c46b78923604a9702420874604db45fe30`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10ae7435a69928a3372106f98f39a13d2c25c3a34451fdef2ffea69d727949d`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f390ef949f256708ccc20a22257e6709373767b987f19d50e2da894cffad75e1`  
		Last Modified: Tue, 13 Jul 2021 18:29:21 GMT  
		Size: 72.6 MB (72639152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21441c5774195c9692fdc0295f0cec79fa3ecde6d4a1304404a156ca16181b35`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 5.6 KB (5595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f259cb871fbb9dc33aa9d45b6594048c26899de2430e9e1ffcda2bead59110d2`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ed44fdfac14863449badc323af635fd968773eff787cb9894976d77582574d96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104312483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c34c41db269abbf10ab0ed9b5934db68369fe8769012172e052cf52a6dc8a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:43:12 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:43:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:43:23 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:43:37 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:43:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:43:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:43:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:43:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:43:48 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 23:43:48 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 23:43:48 GMT
ARG MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 23:43:49 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 23:43:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
# Tue, 13 Jul 2021 23:43:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:44:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:44:15 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:44:15 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:44:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 23:44:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:44:17 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:44:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502273c3f4d3cca6957ee7ad312fccf2a58f474dd4470f4d57fd81c7ccbbad6f`  
		Last Modified: Tue, 13 Jul 2021 23:47:59 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec2b94cdaf1d8183985236813593ca75ec1a93fd8749766a671eed3cb5084a9`  
		Last Modified: Tue, 13 Jul 2021 23:47:57 GMT  
		Size: 4.4 MB (4395559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235bbb8ac48487daf075dffd4eeb87748124db368791f39c6291097fd8087907`  
		Last Modified: Tue, 13 Jul 2021 23:47:57 GMT  
		Size: 3.2 MB (3204623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab6f216bf65e3ea1463da1a6f3a0c8e6e9a218dccdc525833fd4522258f1d81`  
		Last Modified: Tue, 13 Jul 2021 23:47:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c19647916f33368a8ad9c2261897d199b6c7f12d2fc0c78c68c5e94afc1983`  
		Last Modified: Tue, 13 Jul 2021 23:47:57 GMT  
		Size: 1.5 MB (1532405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d482ed8bb6a6891a996239552a67845de3dd3878f25bebaa82503aa8bc89d47`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a41688a5253433e744ebbe4627c25ab47b0385250213199257226e0cb70bfe`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3143ff3d76f78be60926ec476578c670f933471a9fcf678dfb26104f87ec4248`  
		Last Modified: Tue, 13 Jul 2021 23:48:06 GMT  
		Size: 71.4 MB (71437154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e66adf06926d7de93b5a38027e70481343436196027cc982871cd87684975c9`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 5.6 KB (5595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48b2a34851fd54047498d82409a6366486970136fc7ce3151b38dd1e1a1a660`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a4c79ab4f05d4088c934e62b52f58c794e8c94e73a3dcfad5ded42252aa3df8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117628870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0361d567d7920a770863e8fade1d338b3edae167dd86259883e39141120cb2b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:51:25 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:52:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:53:02 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:53:53 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:54:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:55:22 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:55:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:56:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:56:14 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:56:22 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:56:29 GMT
ARG MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:56:38 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:56:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
# Tue, 13 Jul 2021 18:57:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 19:02:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 19:02:31 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 19:02:35 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 19:02:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 19:03:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 19:03:16 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 19:03:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58409e900735b3af04414a2eac25dcf2479f264457522587a2d3b713cb1d54`  
		Last Modified: Tue, 13 Jul 2021 19:07:28 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0832199508426a244908601f7a3fafb898620be6f90658b526f29fcccc7ccf50`  
		Last Modified: Tue, 13 Jul 2021 19:07:28 GMT  
		Size: 5.6 MB (5630513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c69e1972a6436931f30c95a56fdfc15d48c27ac84d60eedeaf40742b613731`  
		Last Modified: Tue, 13 Jul 2021 19:07:27 GMT  
		Size: 3.5 MB (3528890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea947a3fe9cdc3598e8c581207c216fdb3ff0f0f363d6355e8c3b519679e925`  
		Last Modified: Tue, 13 Jul 2021 19:07:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb53ae5254fffcbc388441f70643e8e1f8d4012f20900d2f38c07ab4bf5092`  
		Last Modified: Tue, 13 Jul 2021 19:07:26 GMT  
		Size: 1.9 MB (1938748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e8ec4a32b9707ce15e0b2615457ebe1363cb69ac9fc661be956c391f800788`  
		Last Modified: Tue, 13 Jul 2021 19:07:24 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166205ee57ab5a5cc638447f66eb909d6180afdc0b8b91422bd6e505c2fa94e8`  
		Last Modified: Tue, 13 Jul 2021 19:07:23 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f0c8ad70d2e4bc7211ce6bff737a24b294e38caac31b81400b9737a4c9665f`  
		Last Modified: Tue, 13 Jul 2021 19:07:39 GMT  
		Size: 76.1 MB (76092107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bb9b897fbedc49e30c200909402110b6f9216b784a0eee10f60f07718e071d`  
		Last Modified: Tue, 13 Jul 2021 19:07:23 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96e91da134b7450e3adf4341191479190b484764c762c49f916f6ebb1b89931`  
		Last Modified: Tue, 13 Jul 2021 19:07:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:daaf37a722e689a8135b92bd849ef5787655edbc924b890ca8e6cad7fec8cb98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:612d0f034f206958a9c84b941883cb8c0f304109fb5011202e21a3f09d011c9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109301363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3268c71ffc39a8a97d50abc19e5f72880617cd2cb124ab871cbdc10ed2a08db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:59:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:59:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:24:48 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:25:13 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:25:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:23 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:25:23 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:25:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:25:25 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:25:25 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:25:26 GMT
ARG MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:25:26 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:25:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
# Tue, 13 Jul 2021 18:25:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:26:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:26:09 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:26:10 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:26:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:26:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:26:11 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:26:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d7f527a85d567884b86652e590f5d484b9ab84b150e4925b7d87699f93fea1`  
		Last Modified: Fri, 18 Jun 2021 05:03:42 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ffc1a82bccd839baf9aee65bea12f39144d2f71d17f7a478729e5033a3483e`  
		Last Modified: Fri, 18 Jun 2021 05:03:41 GMT  
		Size: 4.8 MB (4813831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11da2f34c9bc7201cc69fc1cd85b9e49e8cbb5294fb5f4ed482c36995965b114`  
		Last Modified: Tue, 13 Jul 2021 18:29:14 GMT  
		Size: 3.5 MB (3548102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa88816ca3dbb95dc4d440388a0689a08adfcae89926efc82e138406d30a6051`  
		Last Modified: Tue, 13 Jul 2021 18:29:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308022251dfd080c48afe0ce2efa6d93a302640ab9c5671ec4b1b13f68e44ff8`  
		Last Modified: Tue, 13 Jul 2021 18:29:14 GMT  
		Size: 1.6 MB (1586331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6e8acfd55976b0551283d6d0b4d5c46b78923604a9702420874604db45fe30`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10ae7435a69928a3372106f98f39a13d2c25c3a34451fdef2ffea69d727949d`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f390ef949f256708ccc20a22257e6709373767b987f19d50e2da894cffad75e1`  
		Last Modified: Tue, 13 Jul 2021 18:29:21 GMT  
		Size: 72.6 MB (72639152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21441c5774195c9692fdc0295f0cec79fa3ecde6d4a1304404a156ca16181b35`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 5.6 KB (5595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f259cb871fbb9dc33aa9d45b6594048c26899de2430e9e1ffcda2bead59110d2`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ed44fdfac14863449badc323af635fd968773eff787cb9894976d77582574d96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104312483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c34c41db269abbf10ab0ed9b5934db68369fe8769012172e052cf52a6dc8a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:43:12 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:43:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:43:23 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:43:37 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:43:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:43:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:43:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:43:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:43:48 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 23:43:48 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 23:43:48 GMT
ARG MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 23:43:49 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 23:43:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
# Tue, 13 Jul 2021 23:43:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:44:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:44:15 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:44:15 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:44:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 23:44:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:44:17 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:44:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502273c3f4d3cca6957ee7ad312fccf2a58f474dd4470f4d57fd81c7ccbbad6f`  
		Last Modified: Tue, 13 Jul 2021 23:47:59 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec2b94cdaf1d8183985236813593ca75ec1a93fd8749766a671eed3cb5084a9`  
		Last Modified: Tue, 13 Jul 2021 23:47:57 GMT  
		Size: 4.4 MB (4395559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235bbb8ac48487daf075dffd4eeb87748124db368791f39c6291097fd8087907`  
		Last Modified: Tue, 13 Jul 2021 23:47:57 GMT  
		Size: 3.2 MB (3204623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab6f216bf65e3ea1463da1a6f3a0c8e6e9a218dccdc525833fd4522258f1d81`  
		Last Modified: Tue, 13 Jul 2021 23:47:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c19647916f33368a8ad9c2261897d199b6c7f12d2fc0c78c68c5e94afc1983`  
		Last Modified: Tue, 13 Jul 2021 23:47:57 GMT  
		Size: 1.5 MB (1532405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d482ed8bb6a6891a996239552a67845de3dd3878f25bebaa82503aa8bc89d47`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a41688a5253433e744ebbe4627c25ab47b0385250213199257226e0cb70bfe`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3143ff3d76f78be60926ec476578c670f933471a9fcf678dfb26104f87ec4248`  
		Last Modified: Tue, 13 Jul 2021 23:48:06 GMT  
		Size: 71.4 MB (71437154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e66adf06926d7de93b5a38027e70481343436196027cc982871cd87684975c9`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 5.6 KB (5595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48b2a34851fd54047498d82409a6366486970136fc7ce3151b38dd1e1a1a660`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a4c79ab4f05d4088c934e62b52f58c794e8c94e73a3dcfad5ded42252aa3df8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117628870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0361d567d7920a770863e8fade1d338b3edae167dd86259883e39141120cb2b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:51:25 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:52:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:53:02 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:53:53 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:54:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:55:22 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:55:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:56:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:56:14 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:56:22 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:56:29 GMT
ARG MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:56:38 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:56:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
# Tue, 13 Jul 2021 18:57:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 19:02:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 19:02:31 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 19:02:35 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 19:02:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 19:03:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 19:03:16 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 19:03:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58409e900735b3af04414a2eac25dcf2479f264457522587a2d3b713cb1d54`  
		Last Modified: Tue, 13 Jul 2021 19:07:28 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0832199508426a244908601f7a3fafb898620be6f90658b526f29fcccc7ccf50`  
		Last Modified: Tue, 13 Jul 2021 19:07:28 GMT  
		Size: 5.6 MB (5630513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c69e1972a6436931f30c95a56fdfc15d48c27ac84d60eedeaf40742b613731`  
		Last Modified: Tue, 13 Jul 2021 19:07:27 GMT  
		Size: 3.5 MB (3528890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea947a3fe9cdc3598e8c581207c216fdb3ff0f0f363d6355e8c3b519679e925`  
		Last Modified: Tue, 13 Jul 2021 19:07:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb53ae5254fffcbc388441f70643e8e1f8d4012f20900d2f38c07ab4bf5092`  
		Last Modified: Tue, 13 Jul 2021 19:07:26 GMT  
		Size: 1.9 MB (1938748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e8ec4a32b9707ce15e0b2615457ebe1363cb69ac9fc661be956c391f800788`  
		Last Modified: Tue, 13 Jul 2021 19:07:24 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166205ee57ab5a5cc638447f66eb909d6180afdc0b8b91422bd6e505c2fa94e8`  
		Last Modified: Tue, 13 Jul 2021 19:07:23 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f0c8ad70d2e4bc7211ce6bff737a24b294e38caac31b81400b9737a4c9665f`  
		Last Modified: Tue, 13 Jul 2021 19:07:39 GMT  
		Size: 76.1 MB (76092107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bb9b897fbedc49e30c200909402110b6f9216b784a0eee10f60f07718e071d`  
		Last Modified: Tue, 13 Jul 2021 19:07:23 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96e91da134b7450e3adf4341191479190b484764c762c49f916f6ebb1b89931`  
		Last Modified: Tue, 13 Jul 2021 19:07:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.39`

```console
$ docker pull mariadb@sha256:daaf37a722e689a8135b92bd849ef5787655edbc924b890ca8e6cad7fec8cb98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.39` - linux; amd64

```console
$ docker pull mariadb@sha256:612d0f034f206958a9c84b941883cb8c0f304109fb5011202e21a3f09d011c9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109301363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3268c71ffc39a8a97d50abc19e5f72880617cd2cb124ab871cbdc10ed2a08db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:59:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:59:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:24:48 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:25:13 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:25:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:23 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:25:23 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:25:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:25:25 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:25:25 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:25:26 GMT
ARG MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:25:26 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:25:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
# Tue, 13 Jul 2021 18:25:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:26:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:26:09 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:26:10 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:26:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:26:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:26:11 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:26:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d7f527a85d567884b86652e590f5d484b9ab84b150e4925b7d87699f93fea1`  
		Last Modified: Fri, 18 Jun 2021 05:03:42 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ffc1a82bccd839baf9aee65bea12f39144d2f71d17f7a478729e5033a3483e`  
		Last Modified: Fri, 18 Jun 2021 05:03:41 GMT  
		Size: 4.8 MB (4813831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11da2f34c9bc7201cc69fc1cd85b9e49e8cbb5294fb5f4ed482c36995965b114`  
		Last Modified: Tue, 13 Jul 2021 18:29:14 GMT  
		Size: 3.5 MB (3548102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa88816ca3dbb95dc4d440388a0689a08adfcae89926efc82e138406d30a6051`  
		Last Modified: Tue, 13 Jul 2021 18:29:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308022251dfd080c48afe0ce2efa6d93a302640ab9c5671ec4b1b13f68e44ff8`  
		Last Modified: Tue, 13 Jul 2021 18:29:14 GMT  
		Size: 1.6 MB (1586331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6e8acfd55976b0551283d6d0b4d5c46b78923604a9702420874604db45fe30`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10ae7435a69928a3372106f98f39a13d2c25c3a34451fdef2ffea69d727949d`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f390ef949f256708ccc20a22257e6709373767b987f19d50e2da894cffad75e1`  
		Last Modified: Tue, 13 Jul 2021 18:29:21 GMT  
		Size: 72.6 MB (72639152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21441c5774195c9692fdc0295f0cec79fa3ecde6d4a1304404a156ca16181b35`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 5.6 KB (5595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f259cb871fbb9dc33aa9d45b6594048c26899de2430e9e1ffcda2bead59110d2`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.39` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ed44fdfac14863449badc323af635fd968773eff787cb9894976d77582574d96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104312483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c34c41db269abbf10ab0ed9b5934db68369fe8769012172e052cf52a6dc8a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:43:12 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:43:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:43:23 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:43:37 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:43:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:43:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:43:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:43:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:43:48 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 23:43:48 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 23:43:48 GMT
ARG MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 23:43:49 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 23:43:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
# Tue, 13 Jul 2021 23:43:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:44:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:44:15 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:44:15 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:44:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 23:44:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:44:17 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:44:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502273c3f4d3cca6957ee7ad312fccf2a58f474dd4470f4d57fd81c7ccbbad6f`  
		Last Modified: Tue, 13 Jul 2021 23:47:59 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec2b94cdaf1d8183985236813593ca75ec1a93fd8749766a671eed3cb5084a9`  
		Last Modified: Tue, 13 Jul 2021 23:47:57 GMT  
		Size: 4.4 MB (4395559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235bbb8ac48487daf075dffd4eeb87748124db368791f39c6291097fd8087907`  
		Last Modified: Tue, 13 Jul 2021 23:47:57 GMT  
		Size: 3.2 MB (3204623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab6f216bf65e3ea1463da1a6f3a0c8e6e9a218dccdc525833fd4522258f1d81`  
		Last Modified: Tue, 13 Jul 2021 23:47:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c19647916f33368a8ad9c2261897d199b6c7f12d2fc0c78c68c5e94afc1983`  
		Last Modified: Tue, 13 Jul 2021 23:47:57 GMT  
		Size: 1.5 MB (1532405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d482ed8bb6a6891a996239552a67845de3dd3878f25bebaa82503aa8bc89d47`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a41688a5253433e744ebbe4627c25ab47b0385250213199257226e0cb70bfe`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3143ff3d76f78be60926ec476578c670f933471a9fcf678dfb26104f87ec4248`  
		Last Modified: Tue, 13 Jul 2021 23:48:06 GMT  
		Size: 71.4 MB (71437154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e66adf06926d7de93b5a38027e70481343436196027cc982871cd87684975c9`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 5.6 KB (5595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48b2a34851fd54047498d82409a6366486970136fc7ce3151b38dd1e1a1a660`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.39` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a4c79ab4f05d4088c934e62b52f58c794e8c94e73a3dcfad5ded42252aa3df8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117628870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0361d567d7920a770863e8fade1d338b3edae167dd86259883e39141120cb2b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:51:25 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:52:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:53:02 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:53:53 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:54:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:55:22 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:55:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:56:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:56:14 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:56:22 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:56:29 GMT
ARG MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:56:38 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:56:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
# Tue, 13 Jul 2021 18:57:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 19:02:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 19:02:31 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 19:02:35 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 19:02:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 19:03:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 19:03:16 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 19:03:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58409e900735b3af04414a2eac25dcf2479f264457522587a2d3b713cb1d54`  
		Last Modified: Tue, 13 Jul 2021 19:07:28 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0832199508426a244908601f7a3fafb898620be6f90658b526f29fcccc7ccf50`  
		Last Modified: Tue, 13 Jul 2021 19:07:28 GMT  
		Size: 5.6 MB (5630513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c69e1972a6436931f30c95a56fdfc15d48c27ac84d60eedeaf40742b613731`  
		Last Modified: Tue, 13 Jul 2021 19:07:27 GMT  
		Size: 3.5 MB (3528890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea947a3fe9cdc3598e8c581207c216fdb3ff0f0f363d6355e8c3b519679e925`  
		Last Modified: Tue, 13 Jul 2021 19:07:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb53ae5254fffcbc388441f70643e8e1f8d4012f20900d2f38c07ab4bf5092`  
		Last Modified: Tue, 13 Jul 2021 19:07:26 GMT  
		Size: 1.9 MB (1938748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e8ec4a32b9707ce15e0b2615457ebe1363cb69ac9fc661be956c391f800788`  
		Last Modified: Tue, 13 Jul 2021 19:07:24 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166205ee57ab5a5cc638447f66eb909d6180afdc0b8b91422bd6e505c2fa94e8`  
		Last Modified: Tue, 13 Jul 2021 19:07:23 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f0c8ad70d2e4bc7211ce6bff737a24b294e38caac31b81400b9737a4c9665f`  
		Last Modified: Tue, 13 Jul 2021 19:07:39 GMT  
		Size: 76.1 MB (76092107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bb9b897fbedc49e30c200909402110b6f9216b784a0eee10f60f07718e071d`  
		Last Modified: Tue, 13 Jul 2021 19:07:23 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96e91da134b7450e3adf4341191479190b484764c762c49f916f6ebb1b89931`  
		Last Modified: Tue, 13 Jul 2021 19:07:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.39-bionic`

```console
$ docker pull mariadb@sha256:daaf37a722e689a8135b92bd849ef5787655edbc924b890ca8e6cad7fec8cb98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.39-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:612d0f034f206958a9c84b941883cb8c0f304109fb5011202e21a3f09d011c9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109301363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3268c71ffc39a8a97d50abc19e5f72880617cd2cb124ab871cbdc10ed2a08db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:59:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:59:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:24:48 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:25:13 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:25:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:23 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:25:23 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:25:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:25:25 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:25:25 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:25:26 GMT
ARG MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:25:26 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:25:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
# Tue, 13 Jul 2021 18:25:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:26:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:26:09 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:26:10 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:26:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:26:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:26:11 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:26:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d7f527a85d567884b86652e590f5d484b9ab84b150e4925b7d87699f93fea1`  
		Last Modified: Fri, 18 Jun 2021 05:03:42 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ffc1a82bccd839baf9aee65bea12f39144d2f71d17f7a478729e5033a3483e`  
		Last Modified: Fri, 18 Jun 2021 05:03:41 GMT  
		Size: 4.8 MB (4813831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11da2f34c9bc7201cc69fc1cd85b9e49e8cbb5294fb5f4ed482c36995965b114`  
		Last Modified: Tue, 13 Jul 2021 18:29:14 GMT  
		Size: 3.5 MB (3548102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa88816ca3dbb95dc4d440388a0689a08adfcae89926efc82e138406d30a6051`  
		Last Modified: Tue, 13 Jul 2021 18:29:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308022251dfd080c48afe0ce2efa6d93a302640ab9c5671ec4b1b13f68e44ff8`  
		Last Modified: Tue, 13 Jul 2021 18:29:14 GMT  
		Size: 1.6 MB (1586331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6e8acfd55976b0551283d6d0b4d5c46b78923604a9702420874604db45fe30`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10ae7435a69928a3372106f98f39a13d2c25c3a34451fdef2ffea69d727949d`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f390ef949f256708ccc20a22257e6709373767b987f19d50e2da894cffad75e1`  
		Last Modified: Tue, 13 Jul 2021 18:29:21 GMT  
		Size: 72.6 MB (72639152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21441c5774195c9692fdc0295f0cec79fa3ecde6d4a1304404a156ca16181b35`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 5.6 KB (5595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f259cb871fbb9dc33aa9d45b6594048c26899de2430e9e1ffcda2bead59110d2`  
		Last Modified: Tue, 13 Jul 2021 18:29:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.39-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ed44fdfac14863449badc323af635fd968773eff787cb9894976d77582574d96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104312483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c34c41db269abbf10ab0ed9b5934db68369fe8769012172e052cf52a6dc8a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:09 GMT
ADD file:f5aca23bd8c77beda7e17bb71fc4df34d91662b6179de87029f24d21b9e799ad in / 
# Tue, 13 Jul 2021 23:01:09 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:43:12 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:43:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:43:23 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:43:37 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:43:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:43:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:43:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:43:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:43:48 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 23:43:48 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 23:43:48 GMT
ARG MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 23:43:49 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 23:43:49 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
# Tue, 13 Jul 2021 23:43:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:44:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:44:15 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:44:15 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:44:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 23:44:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:44:17 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:44:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b9bb7af7248f30dd1b1f9807608f5f532133384e4db55caa6dbc69b9cf15ddcc`  
		Last Modified: Tue, 13 Jul 2021 23:03:17 GMT  
		Size: 23.7 MB (23729498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502273c3f4d3cca6957ee7ad312fccf2a58f474dd4470f4d57fd81c7ccbbad6f`  
		Last Modified: Tue, 13 Jul 2021 23:47:59 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec2b94cdaf1d8183985236813593ca75ec1a93fd8749766a671eed3cb5084a9`  
		Last Modified: Tue, 13 Jul 2021 23:47:57 GMT  
		Size: 4.4 MB (4395559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235bbb8ac48487daf075dffd4eeb87748124db368791f39c6291097fd8087907`  
		Last Modified: Tue, 13 Jul 2021 23:47:57 GMT  
		Size: 3.2 MB (3204623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab6f216bf65e3ea1463da1a6f3a0c8e6e9a218dccdc525833fd4522258f1d81`  
		Last Modified: Tue, 13 Jul 2021 23:47:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c19647916f33368a8ad9c2261897d199b6c7f12d2fc0c78c68c5e94afc1983`  
		Last Modified: Tue, 13 Jul 2021 23:47:57 GMT  
		Size: 1.5 MB (1532405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d482ed8bb6a6891a996239552a67845de3dd3878f25bebaa82503aa8bc89d47`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a41688a5253433e744ebbe4627c25ab47b0385250213199257226e0cb70bfe`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3143ff3d76f78be60926ec476578c670f933471a9fcf678dfb26104f87ec4248`  
		Last Modified: Tue, 13 Jul 2021 23:48:06 GMT  
		Size: 71.4 MB (71437154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e66adf06926d7de93b5a38027e70481343436196027cc982871cd87684975c9`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 5.6 KB (5595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48b2a34851fd54047498d82409a6366486970136fc7ce3151b38dd1e1a1a660`  
		Last Modified: Tue, 13 Jul 2021 23:47:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.39-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a4c79ab4f05d4088c934e62b52f58c794e8c94e73a3dcfad5ded42252aa3df8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117628870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0361d567d7920a770863e8fade1d338b3edae167dd86259883e39141120cb2b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:51:25 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:52:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:53:02 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:53:53 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:54:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:55:22 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:55:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:56:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:56:14 GMT
ARG MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:56:22 GMT
ENV MARIADB_MAJOR=10.2
# Tue, 13 Jul 2021 18:56:29 GMT
ARG MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:56:38 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Tue, 13 Jul 2021 18:56:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
# Tue, 13 Jul 2021 18:57:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 19:02:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 19:02:31 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 19:02:35 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 19:02:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.39/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 19:03:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 19:03:16 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 19:03:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58409e900735b3af04414a2eac25dcf2479f264457522587a2d3b713cb1d54`  
		Last Modified: Tue, 13 Jul 2021 19:07:28 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0832199508426a244908601f7a3fafb898620be6f90658b526f29fcccc7ccf50`  
		Last Modified: Tue, 13 Jul 2021 19:07:28 GMT  
		Size: 5.6 MB (5630513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c69e1972a6436931f30c95a56fdfc15d48c27ac84d60eedeaf40742b613731`  
		Last Modified: Tue, 13 Jul 2021 19:07:27 GMT  
		Size: 3.5 MB (3528890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea947a3fe9cdc3598e8c581207c216fdb3ff0f0f363d6355e8c3b519679e925`  
		Last Modified: Tue, 13 Jul 2021 19:07:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cb53ae5254fffcbc388441f70643e8e1f8d4012f20900d2f38c07ab4bf5092`  
		Last Modified: Tue, 13 Jul 2021 19:07:26 GMT  
		Size: 1.9 MB (1938748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e8ec4a32b9707ce15e0b2615457ebe1363cb69ac9fc661be956c391f800788`  
		Last Modified: Tue, 13 Jul 2021 19:07:24 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166205ee57ab5a5cc638447f66eb909d6180afdc0b8b91422bd6e505c2fa94e8`  
		Last Modified: Tue, 13 Jul 2021 19:07:23 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f0c8ad70d2e4bc7211ce6bff737a24b294e38caac31b81400b9737a4c9665f`  
		Last Modified: Tue, 13 Jul 2021 19:07:39 GMT  
		Size: 76.1 MB (76092107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bb9b897fbedc49e30c200909402110b6f9216b784a0eee10f60f07718e071d`  
		Last Modified: Tue, 13 Jul 2021 19:07:23 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96e91da134b7450e3adf4341191479190b484764c762c49f916f6ebb1b89931`  
		Last Modified: Tue, 13 Jul 2021 19:07:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:50c673a56fc2883246c0f746dea6631894c10c5261f8eed19b4e51167672ff9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:75b3c447c4cb9069c588b23dd18f031e41a2a3999e508dc40480fc44b51014d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (119994283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebff5bdfa7a83e229bfd40771e84098b778c542e5c99384f894fb96808e5ae8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:24:12 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:24:12 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:24:12 GMT
ARG MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:24:12 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:24:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:24:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:24:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:24:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:24:40 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:24:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:24:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:24:42 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:24:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebadd2584ad8f9cbf09fcb523f86bd08f30e23a076fafb3552a8b44c92909f3`  
		Last Modified: Tue, 13 Jul 2021 18:28:41 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d7c566e62f683a73e2e927b8772ab0c5265e1a791b7bda0b3d8c48bc80d6bf`  
		Last Modified: Tue, 13 Jul 2021 18:28:54 GMT  
		Size: 80.1 MB (80084759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c123b195c0b9d6d91fdf34339e7448864d5ca311cc1025c0e0c03bab42014f`  
		Last Modified: Tue, 13 Jul 2021 18:28:41 GMT  
		Size: 5.6 KB (5594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b176bcf501f753bcfe1d2298632623ab6f1826362032ac2a5d2b676a5a7b26`  
		Last Modified: Tue, 13 Jul 2021 18:28:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:af7d14ed5d4bdcb5c5ca1ac124c148f0be07eb652c33f0bd5993ece2a9a7a98b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117602195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9125427b1aabfe2b93830624a24746a9305b7c3bcd13f439a772824ec38423bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:42:34 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 23:42:34 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 23:42:35 GMT
ARG MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 23:42:35 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 23:42:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:42:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:43:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:43:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:43:02 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:43:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 23:43:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:43:03 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:43:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43268ea17b1c1d1c8631b184cc5a9f47c2708af140c0cba92c962538b66691bc`  
		Last Modified: Tue, 13 Jul 2021 23:47:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd88600d54d9e6036c96c272728aab05a2a0eac7d3fed68e36aa7017f248cdf`  
		Last Modified: Tue, 13 Jul 2021 23:47:33 GMT  
		Size: 79.4 MB (79396660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db297bf843017efffb82d89c86f3e1640a13434ddbf98cc60cef5362d3b91dd`  
		Last Modified: Tue, 13 Jul 2021 23:47:18 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333b160e7a5511b09d3495174a23d16566dfb2890e931fca35ddc8a40240cd6`  
		Last Modified: Tue, 13 Jul 2021 23:47:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:b2c552fc7a7d6ee5db05ac791788df2bb2e13594e61acdf82847bee9d9533656
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130856605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42d8a560fb11e0a38789e17a75bc49f382ea95c3471fc8cba0beea9bf296253b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:43:32 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:43:40 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:43:44 GMT
ARG MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:43:49 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:43:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:44:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:50:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:50:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:50:26 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:50:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:50:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:50:48 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:50:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c37b77f222c35386cdcdfe28385f12ceab99a56a60ed48e17388733ac9d3e1`  
		Last Modified: Tue, 13 Jul 2021 19:06:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f600a611d6f900d7aacdc5beb2cba123ec10617ec1a46eb579dca2dda784d27c`  
		Last Modified: Tue, 13 Jul 2021 19:07:03 GMT  
		Size: 84.7 MB (84658918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5de95fe32eee38a71f34a6ee41659b4a6d40d7f8c2896548d7e0156b40b9e6`  
		Last Modified: Tue, 13 Jul 2021 19:06:45 GMT  
		Size: 5.6 KB (5595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96a3a3d50a9a9b8b6e2c370b7a0248cb4796da01e3cfdf8cb4a9dcaa61dfb22`  
		Last Modified: Tue, 13 Jul 2021 19:06:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:50c673a56fc2883246c0f746dea6631894c10c5261f8eed19b4e51167672ff9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:75b3c447c4cb9069c588b23dd18f031e41a2a3999e508dc40480fc44b51014d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (119994283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebff5bdfa7a83e229bfd40771e84098b778c542e5c99384f894fb96808e5ae8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:24:12 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:24:12 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:24:12 GMT
ARG MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:24:12 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:24:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:24:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:24:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:24:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:24:40 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:24:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:24:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:24:42 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:24:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebadd2584ad8f9cbf09fcb523f86bd08f30e23a076fafb3552a8b44c92909f3`  
		Last Modified: Tue, 13 Jul 2021 18:28:41 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d7c566e62f683a73e2e927b8772ab0c5265e1a791b7bda0b3d8c48bc80d6bf`  
		Last Modified: Tue, 13 Jul 2021 18:28:54 GMT  
		Size: 80.1 MB (80084759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c123b195c0b9d6d91fdf34339e7448864d5ca311cc1025c0e0c03bab42014f`  
		Last Modified: Tue, 13 Jul 2021 18:28:41 GMT  
		Size: 5.6 KB (5594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b176bcf501f753bcfe1d2298632623ab6f1826362032ac2a5d2b676a5a7b26`  
		Last Modified: Tue, 13 Jul 2021 18:28:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:af7d14ed5d4bdcb5c5ca1ac124c148f0be07eb652c33f0bd5993ece2a9a7a98b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117602195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9125427b1aabfe2b93830624a24746a9305b7c3bcd13f439a772824ec38423bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:42:34 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 23:42:34 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 23:42:35 GMT
ARG MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 23:42:35 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 23:42:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:42:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:43:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:43:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:43:02 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:43:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 23:43:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:43:03 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:43:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43268ea17b1c1d1c8631b184cc5a9f47c2708af140c0cba92c962538b66691bc`  
		Last Modified: Tue, 13 Jul 2021 23:47:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd88600d54d9e6036c96c272728aab05a2a0eac7d3fed68e36aa7017f248cdf`  
		Last Modified: Tue, 13 Jul 2021 23:47:33 GMT  
		Size: 79.4 MB (79396660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db297bf843017efffb82d89c86f3e1640a13434ddbf98cc60cef5362d3b91dd`  
		Last Modified: Tue, 13 Jul 2021 23:47:18 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333b160e7a5511b09d3495174a23d16566dfb2890e931fca35ddc8a40240cd6`  
		Last Modified: Tue, 13 Jul 2021 23:47:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:b2c552fc7a7d6ee5db05ac791788df2bb2e13594e61acdf82847bee9d9533656
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130856605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42d8a560fb11e0a38789e17a75bc49f382ea95c3471fc8cba0beea9bf296253b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:43:32 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:43:40 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:43:44 GMT
ARG MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:43:49 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:43:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:44:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:50:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:50:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:50:26 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:50:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:50:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:50:48 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:50:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c37b77f222c35386cdcdfe28385f12ceab99a56a60ed48e17388733ac9d3e1`  
		Last Modified: Tue, 13 Jul 2021 19:06:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f600a611d6f900d7aacdc5beb2cba123ec10617ec1a46eb579dca2dda784d27c`  
		Last Modified: Tue, 13 Jul 2021 19:07:03 GMT  
		Size: 84.7 MB (84658918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5de95fe32eee38a71f34a6ee41659b4a6d40d7f8c2896548d7e0156b40b9e6`  
		Last Modified: Tue, 13 Jul 2021 19:06:45 GMT  
		Size: 5.6 KB (5595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96a3a3d50a9a9b8b6e2c370b7a0248cb4796da01e3cfdf8cb4a9dcaa61dfb22`  
		Last Modified: Tue, 13 Jul 2021 19:06:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.30`

```console
$ docker pull mariadb@sha256:50c673a56fc2883246c0f746dea6631894c10c5261f8eed19b4e51167672ff9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.30` - linux; amd64

```console
$ docker pull mariadb@sha256:75b3c447c4cb9069c588b23dd18f031e41a2a3999e508dc40480fc44b51014d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (119994283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebff5bdfa7a83e229bfd40771e84098b778c542e5c99384f894fb96808e5ae8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:24:12 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:24:12 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:24:12 GMT
ARG MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:24:12 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:24:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:24:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:24:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:24:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:24:40 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:24:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:24:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:24:42 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:24:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebadd2584ad8f9cbf09fcb523f86bd08f30e23a076fafb3552a8b44c92909f3`  
		Last Modified: Tue, 13 Jul 2021 18:28:41 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d7c566e62f683a73e2e927b8772ab0c5265e1a791b7bda0b3d8c48bc80d6bf`  
		Last Modified: Tue, 13 Jul 2021 18:28:54 GMT  
		Size: 80.1 MB (80084759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c123b195c0b9d6d91fdf34339e7448864d5ca311cc1025c0e0c03bab42014f`  
		Last Modified: Tue, 13 Jul 2021 18:28:41 GMT  
		Size: 5.6 KB (5594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b176bcf501f753bcfe1d2298632623ab6f1826362032ac2a5d2b676a5a7b26`  
		Last Modified: Tue, 13 Jul 2021 18:28:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.30` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:af7d14ed5d4bdcb5c5ca1ac124c148f0be07eb652c33f0bd5993ece2a9a7a98b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117602195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9125427b1aabfe2b93830624a24746a9305b7c3bcd13f439a772824ec38423bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:42:34 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 23:42:34 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 23:42:35 GMT
ARG MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 23:42:35 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 23:42:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:42:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:43:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:43:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:43:02 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:43:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 23:43:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:43:03 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:43:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43268ea17b1c1d1c8631b184cc5a9f47c2708af140c0cba92c962538b66691bc`  
		Last Modified: Tue, 13 Jul 2021 23:47:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd88600d54d9e6036c96c272728aab05a2a0eac7d3fed68e36aa7017f248cdf`  
		Last Modified: Tue, 13 Jul 2021 23:47:33 GMT  
		Size: 79.4 MB (79396660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db297bf843017efffb82d89c86f3e1640a13434ddbf98cc60cef5362d3b91dd`  
		Last Modified: Tue, 13 Jul 2021 23:47:18 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333b160e7a5511b09d3495174a23d16566dfb2890e931fca35ddc8a40240cd6`  
		Last Modified: Tue, 13 Jul 2021 23:47:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.30` - linux; ppc64le

```console
$ docker pull mariadb@sha256:b2c552fc7a7d6ee5db05ac791788df2bb2e13594e61acdf82847bee9d9533656
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130856605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42d8a560fb11e0a38789e17a75bc49f382ea95c3471fc8cba0beea9bf296253b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:43:32 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:43:40 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:43:44 GMT
ARG MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:43:49 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:43:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:44:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:50:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:50:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:50:26 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:50:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:50:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:50:48 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:50:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c37b77f222c35386cdcdfe28385f12ceab99a56a60ed48e17388733ac9d3e1`  
		Last Modified: Tue, 13 Jul 2021 19:06:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f600a611d6f900d7aacdc5beb2cba123ec10617ec1a46eb579dca2dda784d27c`  
		Last Modified: Tue, 13 Jul 2021 19:07:03 GMT  
		Size: 84.7 MB (84658918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5de95fe32eee38a71f34a6ee41659b4a6d40d7f8c2896548d7e0156b40b9e6`  
		Last Modified: Tue, 13 Jul 2021 19:06:45 GMT  
		Size: 5.6 KB (5595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96a3a3d50a9a9b8b6e2c370b7a0248cb4796da01e3cfdf8cb4a9dcaa61dfb22`  
		Last Modified: Tue, 13 Jul 2021 19:06:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.30-focal`

```console
$ docker pull mariadb@sha256:50c673a56fc2883246c0f746dea6631894c10c5261f8eed19b4e51167672ff9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.30-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:75b3c447c4cb9069c588b23dd18f031e41a2a3999e508dc40480fc44b51014d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (119994283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebff5bdfa7a83e229bfd40771e84098b778c542e5c99384f894fb96808e5ae8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:24:12 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:24:12 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:24:12 GMT
ARG MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:24:12 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:24:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:24:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:24:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:24:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:24:40 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:24:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:24:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:24:42 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:24:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebadd2584ad8f9cbf09fcb523f86bd08f30e23a076fafb3552a8b44c92909f3`  
		Last Modified: Tue, 13 Jul 2021 18:28:41 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d7c566e62f683a73e2e927b8772ab0c5265e1a791b7bda0b3d8c48bc80d6bf`  
		Last Modified: Tue, 13 Jul 2021 18:28:54 GMT  
		Size: 80.1 MB (80084759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c123b195c0b9d6d91fdf34339e7448864d5ca311cc1025c0e0c03bab42014f`  
		Last Modified: Tue, 13 Jul 2021 18:28:41 GMT  
		Size: 5.6 KB (5594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b176bcf501f753bcfe1d2298632623ab6f1826362032ac2a5d2b676a5a7b26`  
		Last Modified: Tue, 13 Jul 2021 18:28:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.30-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:af7d14ed5d4bdcb5c5ca1ac124c148f0be07eb652c33f0bd5993ece2a9a7a98b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117602195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9125427b1aabfe2b93830624a24746a9305b7c3bcd13f439a772824ec38423bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:42:34 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 23:42:34 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 23:42:35 GMT
ARG MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 23:42:35 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 23:42:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:42:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:43:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:43:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:43:02 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:43:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 23:43:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:43:03 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:43:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43268ea17b1c1d1c8631b184cc5a9f47c2708af140c0cba92c962538b66691bc`  
		Last Modified: Tue, 13 Jul 2021 23:47:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd88600d54d9e6036c96c272728aab05a2a0eac7d3fed68e36aa7017f248cdf`  
		Last Modified: Tue, 13 Jul 2021 23:47:33 GMT  
		Size: 79.4 MB (79396660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db297bf843017efffb82d89c86f3e1640a13434ddbf98cc60cef5362d3b91dd`  
		Last Modified: Tue, 13 Jul 2021 23:47:18 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4333b160e7a5511b09d3495174a23d16566dfb2890e931fca35ddc8a40240cd6`  
		Last Modified: Tue, 13 Jul 2021 23:47:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.30-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:b2c552fc7a7d6ee5db05ac791788df2bb2e13594e61acdf82847bee9d9533656
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130856605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42d8a560fb11e0a38789e17a75bc49f382ea95c3471fc8cba0beea9bf296253b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:43:32 GMT
ARG MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:43:40 GMT
ENV MARIADB_MAJOR=10.3
# Tue, 13 Jul 2021 18:43:44 GMT
ARG MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:43:49 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Tue, 13 Jul 2021 18:43:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:44:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:50:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:50:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:50:26 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:50:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.30/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:50:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:50:48 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:50:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c37b77f222c35386cdcdfe28385f12ceab99a56a60ed48e17388733ac9d3e1`  
		Last Modified: Tue, 13 Jul 2021 19:06:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f600a611d6f900d7aacdc5beb2cba123ec10617ec1a46eb579dca2dda784d27c`  
		Last Modified: Tue, 13 Jul 2021 19:07:03 GMT  
		Size: 84.7 MB (84658918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5de95fe32eee38a71f34a6ee41659b4a6d40d7f8c2896548d7e0156b40b9e6`  
		Last Modified: Tue, 13 Jul 2021 19:06:45 GMT  
		Size: 5.6 KB (5595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96a3a3d50a9a9b8b6e2c370b7a0248cb4796da01e3cfdf8cb4a9dcaa61dfb22`  
		Last Modified: Tue, 13 Jul 2021 19:06:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:cfd44aa0f5a2c5ca1994718a53725120cc1ac71dc756a56ce5a9e6b55495021a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:b82e26d51d8060dd543e6e1a0fedd89bd31bde8ca008fed908fa9e0b1e592f22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124686857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e4e07eca4619ee72a15a2d7a4ed06ad4acecd0752e3334996669f6f0fb7bd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:23:42 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:23:42 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:23:42 GMT
ARG MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:23:42 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:23:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:23:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:24:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:24:06 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:24:06 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:24:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:24:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:24:08 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:24:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5027808ca14c4ab7ea7b259dad54e835ebfeb87448764cfd410a1f1a99f68268`  
		Last Modified: Tue, 13 Jul 2021 18:28:06 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8475018f1c857c699b2f40ccddda5bf6bec7dbde72731f39fb854ff34aa242d2`  
		Last Modified: Tue, 13 Jul 2021 18:28:19 GMT  
		Size: 84.8 MB (84777335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03966f563d59b6a068cbe47e4ff88b70a200dcf9f1df80221310f598c99cb54f`  
		Last Modified: Tue, 13 Jul 2021 18:28:06 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9576039cfc818b1e53b4aea022af1c363e2cf45c220c67d8fbe26d7a2f9f4e68`  
		Last Modified: Tue, 13 Jul 2021 18:28:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:57e3590caa89ddf35f600349c697e342db3186861533037879195af23e95c071
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122212693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da19a7da07ae42245a6c192e4b824cf09269aa87c330086e388a178057361fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:42:02 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 23:42:02 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 23:42:03 GMT
ARG MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 23:42:03 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 23:42:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:42:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:42:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:42:26 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:42:26 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:42:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 23:42:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:42:28 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:42:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b16d3b824d146bc8f021562fbb7af6ec58b79c24991f5190058badc39454f5`  
		Last Modified: Tue, 13 Jul 2021 23:46:42 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd37388efb3dcb4e552624965e0fdf4161aff488db6474985830aa1f51b543fa`  
		Last Modified: Tue, 13 Jul 2021 23:46:58 GMT  
		Size: 84.0 MB (84007160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17003f507248f7de1c6c44cec099a9d9f18be52d257f56db6a9ecf3f821496f7`  
		Last Modified: Tue, 13 Jul 2021 23:46:42 GMT  
		Size: 5.6 KB (5591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134cc878d2d2d05235a40c4bb41dcfedca417ebec331118f825fdeccfdcc567c`  
		Last Modified: Tue, 13 Jul 2021 23:46:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7fd82f16093dc926c2a5f134c7ea8c11da1e88cbbc04d8bf765f20dd31c23d6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.4 MB (135427867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d7c91cccdefa1ef2eee18000ea4ae147bbd04e905ce86ad3e599d1d2f54a0c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:37:10 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:37:13 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:37:16 GMT
ARG MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:37:18 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:37:22 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:37:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:41:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:42:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:42:04 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:42:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:42:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:42:54 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:43:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdba9bdc7a685b07e118e09ef8dec601bb462e55c413f9632fd74989b08838a`  
		Last Modified: Tue, 13 Jul 2021 19:06:05 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd51d2c8a50ee959f075adb75e4bf9982ca10843df4e07b59156f7ee5f5b6b46`  
		Last Modified: Tue, 13 Jul 2021 19:06:25 GMT  
		Size: 89.2 MB (89230180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a280eae3846126956894661f132ca6dac5d1e8c57736a5e77a13b05399de9fa`  
		Last Modified: Tue, 13 Jul 2021 19:06:05 GMT  
		Size: 5.6 KB (5594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2e7e9297225091bf214d4aefb57f3a2f8005d779ae3434fb3667efee518b7f`  
		Last Modified: Tue, 13 Jul 2021 19:06:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:cfd44aa0f5a2c5ca1994718a53725120cc1ac71dc756a56ce5a9e6b55495021a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:b82e26d51d8060dd543e6e1a0fedd89bd31bde8ca008fed908fa9e0b1e592f22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124686857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e4e07eca4619ee72a15a2d7a4ed06ad4acecd0752e3334996669f6f0fb7bd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:23:42 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:23:42 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:23:42 GMT
ARG MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:23:42 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:23:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:23:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:24:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:24:06 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:24:06 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:24:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:24:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:24:08 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:24:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5027808ca14c4ab7ea7b259dad54e835ebfeb87448764cfd410a1f1a99f68268`  
		Last Modified: Tue, 13 Jul 2021 18:28:06 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8475018f1c857c699b2f40ccddda5bf6bec7dbde72731f39fb854ff34aa242d2`  
		Last Modified: Tue, 13 Jul 2021 18:28:19 GMT  
		Size: 84.8 MB (84777335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03966f563d59b6a068cbe47e4ff88b70a200dcf9f1df80221310f598c99cb54f`  
		Last Modified: Tue, 13 Jul 2021 18:28:06 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9576039cfc818b1e53b4aea022af1c363e2cf45c220c67d8fbe26d7a2f9f4e68`  
		Last Modified: Tue, 13 Jul 2021 18:28:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:57e3590caa89ddf35f600349c697e342db3186861533037879195af23e95c071
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122212693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da19a7da07ae42245a6c192e4b824cf09269aa87c330086e388a178057361fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:42:02 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 23:42:02 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 23:42:03 GMT
ARG MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 23:42:03 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 23:42:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:42:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:42:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:42:26 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:42:26 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:42:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 23:42:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:42:28 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:42:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b16d3b824d146bc8f021562fbb7af6ec58b79c24991f5190058badc39454f5`  
		Last Modified: Tue, 13 Jul 2021 23:46:42 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd37388efb3dcb4e552624965e0fdf4161aff488db6474985830aa1f51b543fa`  
		Last Modified: Tue, 13 Jul 2021 23:46:58 GMT  
		Size: 84.0 MB (84007160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17003f507248f7de1c6c44cec099a9d9f18be52d257f56db6a9ecf3f821496f7`  
		Last Modified: Tue, 13 Jul 2021 23:46:42 GMT  
		Size: 5.6 KB (5591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134cc878d2d2d05235a40c4bb41dcfedca417ebec331118f825fdeccfdcc567c`  
		Last Modified: Tue, 13 Jul 2021 23:46:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7fd82f16093dc926c2a5f134c7ea8c11da1e88cbbc04d8bf765f20dd31c23d6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.4 MB (135427867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d7c91cccdefa1ef2eee18000ea4ae147bbd04e905ce86ad3e599d1d2f54a0c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:37:10 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:37:13 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:37:16 GMT
ARG MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:37:18 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:37:22 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:37:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:41:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:42:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:42:04 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:42:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:42:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:42:54 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:43:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdba9bdc7a685b07e118e09ef8dec601bb462e55c413f9632fd74989b08838a`  
		Last Modified: Tue, 13 Jul 2021 19:06:05 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd51d2c8a50ee959f075adb75e4bf9982ca10843df4e07b59156f7ee5f5b6b46`  
		Last Modified: Tue, 13 Jul 2021 19:06:25 GMT  
		Size: 89.2 MB (89230180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a280eae3846126956894661f132ca6dac5d1e8c57736a5e77a13b05399de9fa`  
		Last Modified: Tue, 13 Jul 2021 19:06:05 GMT  
		Size: 5.6 KB (5594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2e7e9297225091bf214d4aefb57f3a2f8005d779ae3434fb3667efee518b7f`  
		Last Modified: Tue, 13 Jul 2021 19:06:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.20`

```console
$ docker pull mariadb@sha256:cfd44aa0f5a2c5ca1994718a53725120cc1ac71dc756a56ce5a9e6b55495021a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.20` - linux; amd64

```console
$ docker pull mariadb@sha256:b82e26d51d8060dd543e6e1a0fedd89bd31bde8ca008fed908fa9e0b1e592f22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124686857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e4e07eca4619ee72a15a2d7a4ed06ad4acecd0752e3334996669f6f0fb7bd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:23:42 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:23:42 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:23:42 GMT
ARG MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:23:42 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:23:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:23:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:24:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:24:06 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:24:06 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:24:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:24:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:24:08 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:24:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5027808ca14c4ab7ea7b259dad54e835ebfeb87448764cfd410a1f1a99f68268`  
		Last Modified: Tue, 13 Jul 2021 18:28:06 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8475018f1c857c699b2f40ccddda5bf6bec7dbde72731f39fb854ff34aa242d2`  
		Last Modified: Tue, 13 Jul 2021 18:28:19 GMT  
		Size: 84.8 MB (84777335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03966f563d59b6a068cbe47e4ff88b70a200dcf9f1df80221310f598c99cb54f`  
		Last Modified: Tue, 13 Jul 2021 18:28:06 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9576039cfc818b1e53b4aea022af1c363e2cf45c220c67d8fbe26d7a2f9f4e68`  
		Last Modified: Tue, 13 Jul 2021 18:28:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.20` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:57e3590caa89ddf35f600349c697e342db3186861533037879195af23e95c071
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122212693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da19a7da07ae42245a6c192e4b824cf09269aa87c330086e388a178057361fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:42:02 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 23:42:02 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 23:42:03 GMT
ARG MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 23:42:03 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 23:42:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:42:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:42:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:42:26 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:42:26 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:42:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 23:42:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:42:28 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:42:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b16d3b824d146bc8f021562fbb7af6ec58b79c24991f5190058badc39454f5`  
		Last Modified: Tue, 13 Jul 2021 23:46:42 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd37388efb3dcb4e552624965e0fdf4161aff488db6474985830aa1f51b543fa`  
		Last Modified: Tue, 13 Jul 2021 23:46:58 GMT  
		Size: 84.0 MB (84007160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17003f507248f7de1c6c44cec099a9d9f18be52d257f56db6a9ecf3f821496f7`  
		Last Modified: Tue, 13 Jul 2021 23:46:42 GMT  
		Size: 5.6 KB (5591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134cc878d2d2d05235a40c4bb41dcfedca417ebec331118f825fdeccfdcc567c`  
		Last Modified: Tue, 13 Jul 2021 23:46:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.20` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7fd82f16093dc926c2a5f134c7ea8c11da1e88cbbc04d8bf765f20dd31c23d6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.4 MB (135427867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d7c91cccdefa1ef2eee18000ea4ae147bbd04e905ce86ad3e599d1d2f54a0c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:37:10 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:37:13 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:37:16 GMT
ARG MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:37:18 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:37:22 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:37:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:41:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:42:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:42:04 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:42:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:42:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:42:54 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:43:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdba9bdc7a685b07e118e09ef8dec601bb462e55c413f9632fd74989b08838a`  
		Last Modified: Tue, 13 Jul 2021 19:06:05 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd51d2c8a50ee959f075adb75e4bf9982ca10843df4e07b59156f7ee5f5b6b46`  
		Last Modified: Tue, 13 Jul 2021 19:06:25 GMT  
		Size: 89.2 MB (89230180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a280eae3846126956894661f132ca6dac5d1e8c57736a5e77a13b05399de9fa`  
		Last Modified: Tue, 13 Jul 2021 19:06:05 GMT  
		Size: 5.6 KB (5594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2e7e9297225091bf214d4aefb57f3a2f8005d779ae3434fb3667efee518b7f`  
		Last Modified: Tue, 13 Jul 2021 19:06:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.20-focal`

```console
$ docker pull mariadb@sha256:cfd44aa0f5a2c5ca1994718a53725120cc1ac71dc756a56ce5a9e6b55495021a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.20-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:b82e26d51d8060dd543e6e1a0fedd89bd31bde8ca008fed908fa9e0b1e592f22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124686857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e4e07eca4619ee72a15a2d7a4ed06ad4acecd0752e3334996669f6f0fb7bd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:23:42 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:23:42 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:23:42 GMT
ARG MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:23:42 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:23:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:23:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:24:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:24:06 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:24:06 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:24:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:24:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:24:08 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:24:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5027808ca14c4ab7ea7b259dad54e835ebfeb87448764cfd410a1f1a99f68268`  
		Last Modified: Tue, 13 Jul 2021 18:28:06 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8475018f1c857c699b2f40ccddda5bf6bec7dbde72731f39fb854ff34aa242d2`  
		Last Modified: Tue, 13 Jul 2021 18:28:19 GMT  
		Size: 84.8 MB (84777335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03966f563d59b6a068cbe47e4ff88b70a200dcf9f1df80221310f598c99cb54f`  
		Last Modified: Tue, 13 Jul 2021 18:28:06 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9576039cfc818b1e53b4aea022af1c363e2cf45c220c67d8fbe26d7a2f9f4e68`  
		Last Modified: Tue, 13 Jul 2021 18:28:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.20-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:57e3590caa89ddf35f600349c697e342db3186861533037879195af23e95c071
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122212693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da19a7da07ae42245a6c192e4b824cf09269aa87c330086e388a178057361fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:42:02 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 23:42:02 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 23:42:03 GMT
ARG MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 23:42:03 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 23:42:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:42:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:42:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:42:26 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:42:26 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:42:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 23:42:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:42:28 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:42:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b16d3b824d146bc8f021562fbb7af6ec58b79c24991f5190058badc39454f5`  
		Last Modified: Tue, 13 Jul 2021 23:46:42 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd37388efb3dcb4e552624965e0fdf4161aff488db6474985830aa1f51b543fa`  
		Last Modified: Tue, 13 Jul 2021 23:46:58 GMT  
		Size: 84.0 MB (84007160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17003f507248f7de1c6c44cec099a9d9f18be52d257f56db6a9ecf3f821496f7`  
		Last Modified: Tue, 13 Jul 2021 23:46:42 GMT  
		Size: 5.6 KB (5591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134cc878d2d2d05235a40c4bb41dcfedca417ebec331118f825fdeccfdcc567c`  
		Last Modified: Tue, 13 Jul 2021 23:46:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.20-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7fd82f16093dc926c2a5f134c7ea8c11da1e88cbbc04d8bf765f20dd31c23d6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.4 MB (135427867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d7c91cccdefa1ef2eee18000ea4ae147bbd04e905ce86ad3e599d1d2f54a0c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:37:10 GMT
ARG MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:37:13 GMT
ENV MARIADB_MAJOR=10.4
# Tue, 13 Jul 2021 18:37:16 GMT
ARG MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:37:18 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Tue, 13 Jul 2021 18:37:22 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:37:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:41:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:42:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:42:04 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:42:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.20/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 18:42:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:42:54 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:43:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdba9bdc7a685b07e118e09ef8dec601bb462e55c413f9632fd74989b08838a`  
		Last Modified: Tue, 13 Jul 2021 19:06:05 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd51d2c8a50ee959f075adb75e4bf9982ca10843df4e07b59156f7ee5f5b6b46`  
		Last Modified: Tue, 13 Jul 2021 19:06:25 GMT  
		Size: 89.2 MB (89230180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a280eae3846126956894661f132ca6dac5d1e8c57736a5e77a13b05399de9fa`  
		Last Modified: Tue, 13 Jul 2021 19:06:05 GMT  
		Size: 5.6 KB (5594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2e7e9297225091bf214d4aefb57f3a2f8005d779ae3434fb3667efee518b7f`  
		Last Modified: Tue, 13 Jul 2021 19:06:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:0ac450cda7586cf0912d3acde1b71c92cfc44948f879b2332103aa5a6010f9c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:031bcc4661624b44ff4ab675d6f9eb215397d39248f7af208022fee41e1d618e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126852824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1cf62797a61beefde0c29c3e6aa4517bfd9afe316408c3d47aff47afa664dc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:23:11 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:23:12 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:23:12 GMT
ARG MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:23:12 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:23:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:23:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:23:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:23:35 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:23:35 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:23:35 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:23:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a548bce829ef69186261860c3f924739cb63625dc663d55eb4e27307f71da9`  
		Last Modified: Tue, 13 Jul 2021 18:27:35 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989a7c4201b5b576faec6495ebc26622858fd63130c544aa374497c08b6d208`  
		Last Modified: Tue, 13 Jul 2021 18:27:50 GMT  
		Size: 86.9 MB (86943420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf64005eb8b39b92c43a96f7c5e73b5c0ef90cdc55abd15fe624a75d85269e`  
		Last Modified: Tue, 13 Jul 2021 18:27:35 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8ef684c95a2e940fe537ef9a73d7580e30a07de334d6e60c21b34607bfbdbe38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124297465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f5a3a576ce7e6b353fd132f872360a916b8e68231f967ce5a41685d1b60c7e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:41:31 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 23:41:31 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 23:41:31 GMT
ARG MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 23:41:32 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 23:41:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:41:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:41:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:41:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:41:54 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:41:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:41:54 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:41:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d599f73b8461eca5b74755637bd0bee655873ecd8a60e9f2685136b3c95d18f6`  
		Last Modified: Tue, 13 Jul 2021 23:46:06 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31862b9eb243c3e684b4ee6de425d39982bb69bf124d58030470691681dec156`  
		Last Modified: Tue, 13 Jul 2021 23:46:22 GMT  
		Size: 86.1 MB (86092056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3628e06e034599173349c2993e2f60aa39b38f88a714ab813b9cfc0866abdde3`  
		Last Modified: Tue, 13 Jul 2021 23:46:06 GMT  
		Size: 5.6 KB (5590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:9cf78d86507c53c26cc476d52cd5538e69d29be9543f947365459857bce04240
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137538955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec132bda7b0a57f17df73d85683d5185bab64c2afd2ec123e4225815451d959c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:32:57 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:33:01 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:33:06 GMT
ARG MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:33:14 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:33:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:33:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:36:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:36:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:36:41 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:36:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:36:50 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:36:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79d7181537052b57e8f56d1b03c9081a56b1f468194318b6112c5d669d3f8f4`  
		Last Modified: Tue, 13 Jul 2021 19:05:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13154635bf5454dfc1d3473e53786ccc2123877921618ffda6adea0defe03a1`  
		Last Modified: Tue, 13 Jul 2021 19:05:46 GMT  
		Size: 91.3 MB (91341389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7ecd187b32672194646c1fafac119499c8acbddd0b81e53859cccf7badfde8`  
		Last Modified: Tue, 13 Jul 2021 19:05:27 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:0ac450cda7586cf0912d3acde1b71c92cfc44948f879b2332103aa5a6010f9c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:031bcc4661624b44ff4ab675d6f9eb215397d39248f7af208022fee41e1d618e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126852824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1cf62797a61beefde0c29c3e6aa4517bfd9afe316408c3d47aff47afa664dc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:23:11 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:23:12 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:23:12 GMT
ARG MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:23:12 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:23:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:23:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:23:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:23:35 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:23:35 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:23:35 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:23:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a548bce829ef69186261860c3f924739cb63625dc663d55eb4e27307f71da9`  
		Last Modified: Tue, 13 Jul 2021 18:27:35 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989a7c4201b5b576faec6495ebc26622858fd63130c544aa374497c08b6d208`  
		Last Modified: Tue, 13 Jul 2021 18:27:50 GMT  
		Size: 86.9 MB (86943420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf64005eb8b39b92c43a96f7c5e73b5c0ef90cdc55abd15fe624a75d85269e`  
		Last Modified: Tue, 13 Jul 2021 18:27:35 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8ef684c95a2e940fe537ef9a73d7580e30a07de334d6e60c21b34607bfbdbe38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124297465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f5a3a576ce7e6b353fd132f872360a916b8e68231f967ce5a41685d1b60c7e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:41:31 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 23:41:31 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 23:41:31 GMT
ARG MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 23:41:32 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 23:41:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:41:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:41:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:41:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:41:54 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:41:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:41:54 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:41:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d599f73b8461eca5b74755637bd0bee655873ecd8a60e9f2685136b3c95d18f6`  
		Last Modified: Tue, 13 Jul 2021 23:46:06 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31862b9eb243c3e684b4ee6de425d39982bb69bf124d58030470691681dec156`  
		Last Modified: Tue, 13 Jul 2021 23:46:22 GMT  
		Size: 86.1 MB (86092056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3628e06e034599173349c2993e2f60aa39b38f88a714ab813b9cfc0866abdde3`  
		Last Modified: Tue, 13 Jul 2021 23:46:06 GMT  
		Size: 5.6 KB (5590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:9cf78d86507c53c26cc476d52cd5538e69d29be9543f947365459857bce04240
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137538955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec132bda7b0a57f17df73d85683d5185bab64c2afd2ec123e4225815451d959c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:32:57 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:33:01 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:33:06 GMT
ARG MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:33:14 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:33:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:33:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:36:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:36:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:36:41 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:36:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:36:50 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:36:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79d7181537052b57e8f56d1b03c9081a56b1f468194318b6112c5d669d3f8f4`  
		Last Modified: Tue, 13 Jul 2021 19:05:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13154635bf5454dfc1d3473e53786ccc2123877921618ffda6adea0defe03a1`  
		Last Modified: Tue, 13 Jul 2021 19:05:46 GMT  
		Size: 91.3 MB (91341389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7ecd187b32672194646c1fafac119499c8acbddd0b81e53859cccf7badfde8`  
		Last Modified: Tue, 13 Jul 2021 19:05:27 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.11`

```console
$ docker pull mariadb@sha256:0ac450cda7586cf0912d3acde1b71c92cfc44948f879b2332103aa5a6010f9c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.11` - linux; amd64

```console
$ docker pull mariadb@sha256:031bcc4661624b44ff4ab675d6f9eb215397d39248f7af208022fee41e1d618e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126852824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1cf62797a61beefde0c29c3e6aa4517bfd9afe316408c3d47aff47afa664dc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:23:11 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:23:12 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:23:12 GMT
ARG MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:23:12 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:23:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:23:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:23:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:23:35 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:23:35 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:23:35 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:23:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a548bce829ef69186261860c3f924739cb63625dc663d55eb4e27307f71da9`  
		Last Modified: Tue, 13 Jul 2021 18:27:35 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989a7c4201b5b576faec6495ebc26622858fd63130c544aa374497c08b6d208`  
		Last Modified: Tue, 13 Jul 2021 18:27:50 GMT  
		Size: 86.9 MB (86943420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf64005eb8b39b92c43a96f7c5e73b5c0ef90cdc55abd15fe624a75d85269e`  
		Last Modified: Tue, 13 Jul 2021 18:27:35 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.11` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8ef684c95a2e940fe537ef9a73d7580e30a07de334d6e60c21b34607bfbdbe38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124297465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f5a3a576ce7e6b353fd132f872360a916b8e68231f967ce5a41685d1b60c7e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:41:31 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 23:41:31 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 23:41:31 GMT
ARG MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 23:41:32 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 23:41:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:41:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:41:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:41:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:41:54 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:41:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:41:54 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:41:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d599f73b8461eca5b74755637bd0bee655873ecd8a60e9f2685136b3c95d18f6`  
		Last Modified: Tue, 13 Jul 2021 23:46:06 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31862b9eb243c3e684b4ee6de425d39982bb69bf124d58030470691681dec156`  
		Last Modified: Tue, 13 Jul 2021 23:46:22 GMT  
		Size: 86.1 MB (86092056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3628e06e034599173349c2993e2f60aa39b38f88a714ab813b9cfc0866abdde3`  
		Last Modified: Tue, 13 Jul 2021 23:46:06 GMT  
		Size: 5.6 KB (5590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.11` - linux; ppc64le

```console
$ docker pull mariadb@sha256:9cf78d86507c53c26cc476d52cd5538e69d29be9543f947365459857bce04240
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137538955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec132bda7b0a57f17df73d85683d5185bab64c2afd2ec123e4225815451d959c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:32:57 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:33:01 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:33:06 GMT
ARG MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:33:14 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:33:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:33:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:36:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:36:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:36:41 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:36:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:36:50 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:36:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79d7181537052b57e8f56d1b03c9081a56b1f468194318b6112c5d669d3f8f4`  
		Last Modified: Tue, 13 Jul 2021 19:05:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13154635bf5454dfc1d3473e53786ccc2123877921618ffda6adea0defe03a1`  
		Last Modified: Tue, 13 Jul 2021 19:05:46 GMT  
		Size: 91.3 MB (91341389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7ecd187b32672194646c1fafac119499c8acbddd0b81e53859cccf7badfde8`  
		Last Modified: Tue, 13 Jul 2021 19:05:27 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.11-focal`

```console
$ docker pull mariadb@sha256:0ac450cda7586cf0912d3acde1b71c92cfc44948f879b2332103aa5a6010f9c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.11-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:031bcc4661624b44ff4ab675d6f9eb215397d39248f7af208022fee41e1d618e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126852824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1cf62797a61beefde0c29c3e6aa4517bfd9afe316408c3d47aff47afa664dc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:23:11 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:23:12 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:23:12 GMT
ARG MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:23:12 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:23:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:23:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:23:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:23:35 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:23:35 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:23:35 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:23:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a548bce829ef69186261860c3f924739cb63625dc663d55eb4e27307f71da9`  
		Last Modified: Tue, 13 Jul 2021 18:27:35 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989a7c4201b5b576faec6495ebc26622858fd63130c544aa374497c08b6d208`  
		Last Modified: Tue, 13 Jul 2021 18:27:50 GMT  
		Size: 86.9 MB (86943420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf64005eb8b39b92c43a96f7c5e73b5c0ef90cdc55abd15fe624a75d85269e`  
		Last Modified: Tue, 13 Jul 2021 18:27:35 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.11-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8ef684c95a2e940fe537ef9a73d7580e30a07de334d6e60c21b34607bfbdbe38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124297465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f5a3a576ce7e6b353fd132f872360a916b8e68231f967ce5a41685d1b60c7e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:41:31 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 23:41:31 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 23:41:31 GMT
ARG MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 23:41:32 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 23:41:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:41:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:41:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:41:53 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:41:54 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:41:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:41:54 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:41:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d599f73b8461eca5b74755637bd0bee655873ecd8a60e9f2685136b3c95d18f6`  
		Last Modified: Tue, 13 Jul 2021 23:46:06 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31862b9eb243c3e684b4ee6de425d39982bb69bf124d58030470691681dec156`  
		Last Modified: Tue, 13 Jul 2021 23:46:22 GMT  
		Size: 86.1 MB (86092056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3628e06e034599173349c2993e2f60aa39b38f88a714ab813b9cfc0866abdde3`  
		Last Modified: Tue, 13 Jul 2021 23:46:06 GMT  
		Size: 5.6 KB (5590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.11-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:9cf78d86507c53c26cc476d52cd5538e69d29be9543f947365459857bce04240
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137538955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec132bda7b0a57f17df73d85683d5185bab64c2afd2ec123e4225815451d959c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:32:57 GMT
ARG MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:33:01 GMT
ENV MARIADB_MAJOR=10.5
# Tue, 13 Jul 2021 18:33:06 GMT
ARG MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:33:14 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Tue, 13 Jul 2021 18:33:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:33:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:36:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.11/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:36:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:36:41 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:36:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:36:50 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:36:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79d7181537052b57e8f56d1b03c9081a56b1f468194318b6112c5d669d3f8f4`  
		Last Modified: Tue, 13 Jul 2021 19:05:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13154635bf5454dfc1d3473e53786ccc2123877921618ffda6adea0defe03a1`  
		Last Modified: Tue, 13 Jul 2021 19:05:46 GMT  
		Size: 91.3 MB (91341389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7ecd187b32672194646c1fafac119499c8acbddd0b81e53859cccf7badfde8`  
		Last Modified: Tue, 13 Jul 2021 19:05:27 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:d91a1a362a01a4f26c5ed3b34a861f6c1f22a20176ff4a464902adfe8382bafd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:cc58d2e89470cd6dc792be7eef70f7cf8f5e9da89c00ed01b3a7f41dc31f6297
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127011672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24439278c77038c5acc032f1e40e737db054bd1e36551108b657a31ea9233860`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:22:13 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:22:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:22:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:22:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:22:57 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:22:58 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:22:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bab4b089ce1a692b2cd7379f70920f9bab6969ea344af112a507fa96b17dd7`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992059611ea5389c3a532956c7dccc37c13d8450c6fdb79b3d65f295bdf19c51`  
		Last Modified: Tue, 13 Jul 2021 18:27:08 GMT  
		Size: 87.1 MB (87102268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba030b7d27eab09343a23988d5e00d3bf1880edfb9962197a9c9fbfd89806ffe`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:239e4679d65d9a44c983072b52312f8cbfaf505a805090aa97d1a65266c82669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124305174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5769943918c67f6492a009979e758470c83b2de2a83d1716402f1d4009b78479`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:40:54 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:40:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:41:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:41:17 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:41:17 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:41:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:41:18 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:41:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a44c338f719da6a7548fc4e647b9bd52225c5df3e2302badd4a3636d4ada6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0477462ca83c7a80d659335ac0c0d7eadd33db5bf3497027907f7c417dd036c5`  
		Last Modified: Tue, 13 Jul 2021 23:45:32 GMT  
		Size: 86.1 MB (86099760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85af6cce3f74250abc9bdff500887dc7967e9af3afde38f6d863fde77572ed62`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e83376a3a79780723ee2f77623bca0817d59cac7d5edd216700e596ab9344b2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137504069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d483574e8cdb21e02f00261a7f79687f57f662824805f3a9b2c2d43e35ebf08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:26:26 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:32 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:36 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:41 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:26:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:31:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:32:08 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:32:16 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:32:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:32:27 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:32:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fef03d4d8ec5fdbff5a48b3b0bd2e4b89871abaea39af1025a6c3c13bc5a05`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99414d7cf31143b328d34986107ab9144e1e311e6bae8d5686c17b2a8faa43`  
		Last Modified: Tue, 13 Jul 2021 19:04:55 GMT  
		Size: 91.3 MB (91306505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704b6e12ccce455e8980f637eee2cc9c2dc93e364a9dc504ed7d1073f107f7d2`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:d91a1a362a01a4f26c5ed3b34a861f6c1f22a20176ff4a464902adfe8382bafd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:cc58d2e89470cd6dc792be7eef70f7cf8f5e9da89c00ed01b3a7f41dc31f6297
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127011672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24439278c77038c5acc032f1e40e737db054bd1e36551108b657a31ea9233860`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:22:13 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:22:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:22:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:22:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:22:57 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:22:58 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:22:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bab4b089ce1a692b2cd7379f70920f9bab6969ea344af112a507fa96b17dd7`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992059611ea5389c3a532956c7dccc37c13d8450c6fdb79b3d65f295bdf19c51`  
		Last Modified: Tue, 13 Jul 2021 18:27:08 GMT  
		Size: 87.1 MB (87102268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba030b7d27eab09343a23988d5e00d3bf1880edfb9962197a9c9fbfd89806ffe`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:239e4679d65d9a44c983072b52312f8cbfaf505a805090aa97d1a65266c82669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124305174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5769943918c67f6492a009979e758470c83b2de2a83d1716402f1d4009b78479`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:40:54 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:40:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:41:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:41:17 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:41:17 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:41:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:41:18 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:41:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a44c338f719da6a7548fc4e647b9bd52225c5df3e2302badd4a3636d4ada6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0477462ca83c7a80d659335ac0c0d7eadd33db5bf3497027907f7c417dd036c5`  
		Last Modified: Tue, 13 Jul 2021 23:45:32 GMT  
		Size: 86.1 MB (86099760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85af6cce3f74250abc9bdff500887dc7967e9af3afde38f6d863fde77572ed62`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e83376a3a79780723ee2f77623bca0817d59cac7d5edd216700e596ab9344b2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137504069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d483574e8cdb21e02f00261a7f79687f57f662824805f3a9b2c2d43e35ebf08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:26:26 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:32 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:36 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:41 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:26:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:31:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:32:08 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:32:16 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:32:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:32:27 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:32:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fef03d4d8ec5fdbff5a48b3b0bd2e4b89871abaea39af1025a6c3c13bc5a05`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99414d7cf31143b328d34986107ab9144e1e311e6bae8d5686c17b2a8faa43`  
		Last Modified: Tue, 13 Jul 2021 19:04:55 GMT  
		Size: 91.3 MB (91306505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704b6e12ccce455e8980f637eee2cc9c2dc93e364a9dc504ed7d1073f107f7d2`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.3`

```console
$ docker pull mariadb@sha256:d91a1a362a01a4f26c5ed3b34a861f6c1f22a20176ff4a464902adfe8382bafd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.6.3` - linux; amd64

```console
$ docker pull mariadb@sha256:cc58d2e89470cd6dc792be7eef70f7cf8f5e9da89c00ed01b3a7f41dc31f6297
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127011672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24439278c77038c5acc032f1e40e737db054bd1e36551108b657a31ea9233860`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:22:13 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:22:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:22:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:22:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:22:57 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:22:58 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:22:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bab4b089ce1a692b2cd7379f70920f9bab6969ea344af112a507fa96b17dd7`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992059611ea5389c3a532956c7dccc37c13d8450c6fdb79b3d65f295bdf19c51`  
		Last Modified: Tue, 13 Jul 2021 18:27:08 GMT  
		Size: 87.1 MB (87102268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba030b7d27eab09343a23988d5e00d3bf1880edfb9962197a9c9fbfd89806ffe`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:239e4679d65d9a44c983072b52312f8cbfaf505a805090aa97d1a65266c82669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124305174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5769943918c67f6492a009979e758470c83b2de2a83d1716402f1d4009b78479`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:40:54 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:40:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:41:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:41:17 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:41:17 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:41:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:41:18 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:41:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a44c338f719da6a7548fc4e647b9bd52225c5df3e2302badd4a3636d4ada6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0477462ca83c7a80d659335ac0c0d7eadd33db5bf3497027907f7c417dd036c5`  
		Last Modified: Tue, 13 Jul 2021 23:45:32 GMT  
		Size: 86.1 MB (86099760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85af6cce3f74250abc9bdff500887dc7967e9af3afde38f6d863fde77572ed62`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e83376a3a79780723ee2f77623bca0817d59cac7d5edd216700e596ab9344b2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137504069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d483574e8cdb21e02f00261a7f79687f57f662824805f3a9b2c2d43e35ebf08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:26:26 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:32 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:36 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:41 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:26:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:31:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:32:08 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:32:16 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:32:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:32:27 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:32:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fef03d4d8ec5fdbff5a48b3b0bd2e4b89871abaea39af1025a6c3c13bc5a05`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99414d7cf31143b328d34986107ab9144e1e311e6bae8d5686c17b2a8faa43`  
		Last Modified: Tue, 13 Jul 2021 19:04:55 GMT  
		Size: 91.3 MB (91306505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704b6e12ccce455e8980f637eee2cc9c2dc93e364a9dc504ed7d1073f107f7d2`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.3-focal`

```console
$ docker pull mariadb@sha256:d91a1a362a01a4f26c5ed3b34a861f6c1f22a20176ff4a464902adfe8382bafd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.6.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:cc58d2e89470cd6dc792be7eef70f7cf8f5e9da89c00ed01b3a7f41dc31f6297
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127011672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24439278c77038c5acc032f1e40e737db054bd1e36551108b657a31ea9233860`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:22:13 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:22:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:22:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:22:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:22:57 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:22:58 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:22:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bab4b089ce1a692b2cd7379f70920f9bab6969ea344af112a507fa96b17dd7`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992059611ea5389c3a532956c7dccc37c13d8450c6fdb79b3d65f295bdf19c51`  
		Last Modified: Tue, 13 Jul 2021 18:27:08 GMT  
		Size: 87.1 MB (87102268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba030b7d27eab09343a23988d5e00d3bf1880edfb9962197a9c9fbfd89806ffe`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:239e4679d65d9a44c983072b52312f8cbfaf505a805090aa97d1a65266c82669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124305174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5769943918c67f6492a009979e758470c83b2de2a83d1716402f1d4009b78479`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:40:54 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:40:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:41:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:41:17 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:41:17 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:41:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:41:18 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:41:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a44c338f719da6a7548fc4e647b9bd52225c5df3e2302badd4a3636d4ada6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0477462ca83c7a80d659335ac0c0d7eadd33db5bf3497027907f7c417dd036c5`  
		Last Modified: Tue, 13 Jul 2021 23:45:32 GMT  
		Size: 86.1 MB (86099760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85af6cce3f74250abc9bdff500887dc7967e9af3afde38f6d863fde77572ed62`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e83376a3a79780723ee2f77623bca0817d59cac7d5edd216700e596ab9344b2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137504069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d483574e8cdb21e02f00261a7f79687f57f662824805f3a9b2c2d43e35ebf08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:26:26 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:32 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:36 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:41 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:26:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:31:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:32:08 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:32:16 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:32:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:32:27 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:32:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fef03d4d8ec5fdbff5a48b3b0bd2e4b89871abaea39af1025a6c3c13bc5a05`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99414d7cf31143b328d34986107ab9144e1e311e6bae8d5686c17b2a8faa43`  
		Last Modified: Tue, 13 Jul 2021 19:04:55 GMT  
		Size: 91.3 MB (91306505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704b6e12ccce455e8980f637eee2cc9c2dc93e364a9dc504ed7d1073f107f7d2`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:d91a1a362a01a4f26c5ed3b34a861f6c1f22a20176ff4a464902adfe8382bafd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:cc58d2e89470cd6dc792be7eef70f7cf8f5e9da89c00ed01b3a7f41dc31f6297
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127011672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24439278c77038c5acc032f1e40e737db054bd1e36551108b657a31ea9233860`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:22:13 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:22:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:22:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:22:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:22:57 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:22:58 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:22:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bab4b089ce1a692b2cd7379f70920f9bab6969ea344af112a507fa96b17dd7`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992059611ea5389c3a532956c7dccc37c13d8450c6fdb79b3d65f295bdf19c51`  
		Last Modified: Tue, 13 Jul 2021 18:27:08 GMT  
		Size: 87.1 MB (87102268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba030b7d27eab09343a23988d5e00d3bf1880edfb9962197a9c9fbfd89806ffe`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:239e4679d65d9a44c983072b52312f8cbfaf505a805090aa97d1a65266c82669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124305174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5769943918c67f6492a009979e758470c83b2de2a83d1716402f1d4009b78479`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:40:54 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:40:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:41:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:41:17 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:41:17 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:41:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:41:18 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:41:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a44c338f719da6a7548fc4e647b9bd52225c5df3e2302badd4a3636d4ada6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0477462ca83c7a80d659335ac0c0d7eadd33db5bf3497027907f7c417dd036c5`  
		Last Modified: Tue, 13 Jul 2021 23:45:32 GMT  
		Size: 86.1 MB (86099760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85af6cce3f74250abc9bdff500887dc7967e9af3afde38f6d863fde77572ed62`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e83376a3a79780723ee2f77623bca0817d59cac7d5edd216700e596ab9344b2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137504069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d483574e8cdb21e02f00261a7f79687f57f662824805f3a9b2c2d43e35ebf08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:26:26 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:32 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:36 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:41 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:26:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:31:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:32:08 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:32:16 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:32:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:32:27 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:32:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fef03d4d8ec5fdbff5a48b3b0bd2e4b89871abaea39af1025a6c3c13bc5a05`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99414d7cf31143b328d34986107ab9144e1e311e6bae8d5686c17b2a8faa43`  
		Last Modified: Tue, 13 Jul 2021 19:04:55 GMT  
		Size: 91.3 MB (91306505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704b6e12ccce455e8980f637eee2cc9c2dc93e364a9dc504ed7d1073f107f7d2`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:d91a1a362a01a4f26c5ed3b34a861f6c1f22a20176ff4a464902adfe8382bafd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:cc58d2e89470cd6dc792be7eef70f7cf8f5e9da89c00ed01b3a7f41dc31f6297
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127011672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24439278c77038c5acc032f1e40e737db054bd1e36551108b657a31ea9233860`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:21:46 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:22:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:22:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:22:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:22:11 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:22:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:22:13 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:22:14 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:22:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:22:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:22:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:22:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:22:57 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:22:58 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:22:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6532733f97ed67dc953298929836928f042e67d93ffd811a15c4bc06e479b`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 3.6 MB (3582410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8e85a9bd5d53305cbbfbb73c1c6b03e90a2eee824b414c20e78e0a0889436`  
		Last Modified: Tue, 13 Jul 2021 18:26:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b186e1fcc1a267eac35dce20a1dfff37f5dc4e2c2017060c1e0953fe8bd47`  
		Last Modified: Tue, 13 Jul 2021 18:26:55 GMT  
		Size: 2.3 MB (2274215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff18fad55beb0c16e4c1f59a80c03df27a404c4b56de13cb0f9a9bba5cb3b029`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bab4b089ce1a692b2cd7379f70920f9bab6969ea344af112a507fa96b17dd7`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992059611ea5389c3a532956c7dccc37c13d8450c6fdb79b3d65f295bdf19c51`  
		Last Modified: Tue, 13 Jul 2021 18:27:08 GMT  
		Size: 87.1 MB (87102268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba030b7d27eab09343a23988d5e00d3bf1880edfb9962197a9c9fbfd89806ffe`  
		Last Modified: Tue, 13 Jul 2021 18:26:54 GMT  
		Size: 5.6 KB (5593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:239e4679d65d9a44c983072b52312f8cbfaf505a805090aa97d1a65266c82669
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124305174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5769943918c67f6492a009979e758470c83b2de2a83d1716402f1d4009b78479`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:40:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 23:40:28 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:29 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 23:40:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 23:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 23:40:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:40:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 23:40:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 23:40:54 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 23:40:55 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 23:40:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 23:40:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 23:41:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 23:41:17 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 23:41:17 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 23:41:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 23:41:18 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 23:41:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866247a8c244dc65add23238c2be8aa4860fb8463050c215ed786bb4a39b29c`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d83b1c8ef82d33928af5183a83be2534a72522727ed2de9041c24b82b3c16`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 5.5 MB (5455146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a77417ecdb153ca7a104f3a35e99fe0c9ffbc8fb2ce8ce543cc95c108db6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:20 GMT  
		Size: 3.4 MB (3367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451fd044ee319a728a9c2e769b5a430ae91313fe520417d7a885d86f8b8a435f`  
		Last Modified: Tue, 13 Jul 2021 23:45:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb10aa0678e7db1d957917646d80aa856048258f79128ad45b59741de94b0`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.2 MB (2203601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b43a94638739874436239325e26cbdf7cbbe69cc50ca4f1b3e25066281b23f`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a44c338f719da6a7548fc4e647b9bd52225c5df3e2302badd4a3636d4ada6ee`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0477462ca83c7a80d659335ac0c0d7eadd33db5bf3497027907f7c417dd036c5`  
		Last Modified: Tue, 13 Jul 2021 23:45:32 GMT  
		Size: 86.1 MB (86099760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85af6cce3f74250abc9bdff500887dc7967e9af3afde38f6d863fde77572ed62`  
		Last Modified: Tue, 13 Jul 2021 23:45:17 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e83376a3a79780723ee2f77623bca0817d59cac7d5edd216700e596ab9344b2d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137504069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d483574e8cdb21e02f00261a7f79687f57f662824805f3a9b2c2d43e35ebf08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 18:21:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jul 2021 18:23:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:23:28 GMT
ENV GOSU_VERSION=1.13
# Tue, 13 Jul 2021 18:24:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jul 2021 18:24:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jul 2021 18:25:55 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 18:26:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 13 Jul 2021 18:26:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 13 Jul 2021 18:26:26 GMT
ARG MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:32 GMT
ENV MARIADB_MAJOR=10.6
# Tue, 13 Jul 2021 18:26:36 GMT
ARG MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:41 GMT
ENV MARIADB_VERSION=1:10.6.3+maria~focal
# Tue, 13 Jul 2021 18:26:47 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
# Tue, 13 Jul 2021 18:26:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 13 Jul 2021 18:31:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 13 Jul 2021 18:32:08 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jul 2021 18:32:16 GMT
COPY file:b3c92236ffa4530a3affc90901b4ff364200997f53728db206774632c54ed4bb in /usr/local/bin/ 
# Tue, 13 Jul 2021 18:32:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 18:32:27 GMT
EXPOSE 3306
# Tue, 13 Jul 2021 18:32:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabec7e267782eb04117e151b4ae19dbd31828ac2327aa93ceb2e762f739708`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957801e75b45ced792206a25e9311ed87151bf7d982ccf96992cce8b662053cd`  
		Last Modified: Tue, 13 Jul 2021 19:04:41 GMT  
		Size: 6.7 MB (6668034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de8978e5ad4aae012ca56e61e9ed998a3174b826149ab640e7be855f155a590`  
		Last Modified: Tue, 13 Jul 2021 19:04:40 GMT  
		Size: 3.7 MB (3670940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac67211566b51edb92685cb1614825334340a130bee9ab9e779b7f59b12cff4`  
		Last Modified: Tue, 13 Jul 2021 19:04:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eef40a00322a6a1bd02a11873d77eed0ffc51bce8069d4a33c1e4cb19b25b1`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.6 MB (2570014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe88f0e23af781797ca57a993657d37f40c970b0f1c34648b770da1c3b60f99`  
		Last Modified: Tue, 13 Jul 2021 19:04:36 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fef03d4d8ec5fdbff5a48b3b0bd2e4b89871abaea39af1025a6c3c13bc5a05`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99414d7cf31143b328d34986107ab9144e1e311e6bae8d5686c17b2a8faa43`  
		Last Modified: Tue, 13 Jul 2021 19:04:55 GMT  
		Size: 91.3 MB (91306505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704b6e12ccce455e8980f637eee2cc9c2dc93e364a9dc504ed7d1073f107f7d2`  
		Last Modified: Tue, 13 Jul 2021 19:04:35 GMT  
		Size: 5.6 KB (5592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
