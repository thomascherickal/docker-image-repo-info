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
