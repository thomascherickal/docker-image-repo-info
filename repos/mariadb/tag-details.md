<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10-focal`](#mariadb10-focal)
-	[`mariadb:10.2`](#mariadb102)
-	[`mariadb:10.2-bionic`](#mariadb102-bionic)
-	[`mariadb:10.2.43`](#mariadb10243)
-	[`mariadb:10.2.43-bionic`](#mariadb10243-bionic)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.3.34`](#mariadb10334)
-	[`mariadb:10.3.34-focal`](#mariadb10334-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.4.24`](#mariadb10424)
-	[`mariadb:10.4.24-focal`](#mariadb10424-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10.5.15`](#mariadb10515)
-	[`mariadb:10.5.15-focal`](#mariadb10515-focal)
-	[`mariadb:10.6`](#mariadb106)
-	[`mariadb:10.6-focal`](#mariadb106-focal)
-	[`mariadb:10.6.7`](#mariadb1067)
-	[`mariadb:10.6.7-focal`](#mariadb1067-focal)
-	[`mariadb:10.7`](#mariadb107)
-	[`mariadb:10.7-focal`](#mariadb107-focal)
-	[`mariadb:10.7.3`](#mariadb1073)
-	[`mariadb:10.7.3-focal`](#mariadb1073-focal)
-	[`mariadb:10.8-rc`](#mariadb108-rc)
-	[`mariadb:10.8-rc-focal`](#mariadb108-rc-focal)
-	[`mariadb:10.8.2-rc`](#mariadb1082-rc)
-	[`mariadb:10.8.2-rc-focal`](#mariadb1082-rc-focal)
-	[`mariadb:focal`](#mariadbfocal)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:d28e381c205c895eb44e7e1843884bf31018a94e18a39fb6f37c769c045a4e8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:04a2c991ca9282b610ca4a5271ffc617e52d5d9c9cbe324771f827474e4d1dfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f545466a3bd9ba56de74c6aff0b326bfd31b45b23aea7982a3fe54e94c6783bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:59 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:00 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:01 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:02 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:05:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:05:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:05:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:05:29 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:05:30 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:05:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8552be18be3da4845285400b3cc0ef56395f23252feec66ec1b7d9c839caf6f3`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838f8e410529d235d60451deb629c2ad0048c54b691c81f8485e1cca8eec4846`  
		Last Modified: Sat, 30 Apr 2022 00:11:44 GMT  
		Size: 87.6 MB (87644865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6eca4b9a032371bbf080c453df543d01bdfce97ea7c11583ea86854f79dd92`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f2797f4c63be734eab71b5da1025d334620dd0a6978f80cb11022c88ccfcec`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; s390x

```console
$ docker pull mariadb@sha256:834212faeb75a2a43648a37982041f285f537b5cb1e3b0d4698a8df3732007cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127701635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5e6a0fd99b6b261fb89f90ebda2e325da3051f0d56a4895f553c69af9c69686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:45:41 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:41 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:42 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:45:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:46:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:46:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:46:15 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:46:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70732cc91f318d007de766e94265f7a0539440482fedce98b4ed140173b77f1c`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44483aab52b201a5daba428dbb324742d6ece06777315a61021f24fc22a740cd`  
		Last Modified: Fri, 29 Apr 2022 23:49:09 GMT  
		Size: 89.8 MB (89815369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d5f62ecf4e209a33d158a01c03b82ad089be13910b212570c95d41706666df`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d60e7434e17b71d925c7fe28efc5dfee00d94111b7a8225788104b4c04262ec`  
		Last Modified: Fri, 29 Apr 2022 23:48:57 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:d28e381c205c895eb44e7e1843884bf31018a94e18a39fb6f37c769c045a4e8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:04a2c991ca9282b610ca4a5271ffc617e52d5d9c9cbe324771f827474e4d1dfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f545466a3bd9ba56de74c6aff0b326bfd31b45b23aea7982a3fe54e94c6783bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:59 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:00 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:01 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:02 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:05:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:05:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:05:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:05:29 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:05:30 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:05:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8552be18be3da4845285400b3cc0ef56395f23252feec66ec1b7d9c839caf6f3`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838f8e410529d235d60451deb629c2ad0048c54b691c81f8485e1cca8eec4846`  
		Last Modified: Sat, 30 Apr 2022 00:11:44 GMT  
		Size: 87.6 MB (87644865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6eca4b9a032371bbf080c453df543d01bdfce97ea7c11583ea86854f79dd92`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f2797f4c63be734eab71b5da1025d334620dd0a6978f80cb11022c88ccfcec`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:834212faeb75a2a43648a37982041f285f537b5cb1e3b0d4698a8df3732007cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127701635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5e6a0fd99b6b261fb89f90ebda2e325da3051f0d56a4895f553c69af9c69686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:45:41 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:41 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:42 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:45:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:46:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:46:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:46:15 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:46:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70732cc91f318d007de766e94265f7a0539440482fedce98b4ed140173b77f1c`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44483aab52b201a5daba428dbb324742d6ece06777315a61021f24fc22a740cd`  
		Last Modified: Fri, 29 Apr 2022 23:49:09 GMT  
		Size: 89.8 MB (89815369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d5f62ecf4e209a33d158a01c03b82ad089be13910b212570c95d41706666df`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d60e7434e17b71d925c7fe28efc5dfee00d94111b7a8225788104b4c04262ec`  
		Last Modified: Fri, 29 Apr 2022 23:48:57 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:f28c3f215c0786c06f9057a6c4638a9ce2af4ff1e6f7be51645f94e0b37f0def
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:8fcefbc6900276beaf7355e091c097ef57d2016e710fd202d325caeaae76d0a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109317051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e64d2ba5ee25d4a070b1d24ef9e9ff239efce9a68854eef75e6bad1bd14d115`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:53:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:53:40 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:53:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:53:53 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:53:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:54:01 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:54:01 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:54:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 02:54:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:54:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:54:37 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:54:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:54:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:54:38 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:54:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2b6021c87a182e98ffd2863b419bb79abb17cbe79278678bd9fe625af2fdf0`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765f601f0e14bf00b76a7c869dda18bb82726fb91ec363e01da58c1c7b443a3c`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 4.8 MB (4813346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01afffc2780257e621ca877a11e714b4a7c5c410f53d54498085dc40d6bfbc5`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 3.6 MB (3553293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3da9b715df5cce68601eb2b10a167f2a0fce8580873de81baa04625b3630777`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a2f060b97f61c909fac29a13ed6566d3582398b8aad97229e9cc5e8ff1b932`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 1.6 MB (1583545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd15d91ff5e8df79d2baef2f494b7a3630ab71ff3873ffa33312779f13c2221`  
		Last Modified: Fri, 22 Apr 2022 02:58:22 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbe407eaad30abd7fa7ea03f254a904ee2124fc3f320b3847677be56343ffb4`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866119df23a1053b37cbcf551ce1817f59f56a5201e1cefe3af83ac98b4fccfd`  
		Last Modified: Fri, 22 Apr 2022 02:58:31 GMT  
		Size: 72.6 MB (72639071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f565937cba773bda59caa0bfc5797250dedf1cbf2794053575300e6c8a306ffd`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d560a16832325d66ddca5bcd9b1e7d6026434f572a5965d8f6ff235e17bcdc`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e6b018aab576555b6e0bfd1b1b382e6ef1eed43e7c6956456e42bf5acf235c`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:83dec39d49c17442fafdc25e6f5d1bdc4d003e6fa19426a8120ef2a0dffb9169
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104258162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1ecb118afcb05518118a6c6c361190da87c708e8f13a79da8c86b5518219e8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:26 GMT
ADD file:78300bda9e889eaa778190cac0e569ff379d5e533e86b086248476e6ba9b4b2d in / 
# Fri, 29 Apr 2022 22:49:26 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:08:34 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:08:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:08:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:09:03 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:09:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:09:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:09:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:09:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:09:16 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 00:09:17 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 00:09:18 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 00:09:19 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 00:09:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Sat, 30 Apr 2022 00:09:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:09:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:09:48 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:09:50 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:09:51 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:09:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 00:09:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:09:53 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:09:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e196da37f904f62d236ea302bf13ba07711cc62b35774f86ecda18bcc9ed57c6`  
		Last Modified: Fri, 29 Apr 2022 22:51:14 GMT  
		Size: 23.7 MB (23735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddffcde8b39b72c10cbcd5d96f2307b6d6857369d4a57beb67277bd9f18aedc`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 1.9 KB (1854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed99cb2e83bbae3472b1b2ab68249e1c7dec481cc489c7d69b2627706d3058e7`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 4.3 MB (4261792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745c5d6a542769b03497a41228d4f31506c746d9f5ec5bf393f426c2a27c815b`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 3.2 MB (3207565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8e8f86c5634b4f012cd1f27e537c696a24e4c684810681da4d92d4f232d43a`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2279bacf1382c4ea4fafacc8f579b65d5e2c3949c934e3d1c3efe6fab90ec2cf`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 1.5 MB (1530621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e032a6d669d1fd06479b50389ac1237c010ebdc2fe3008e47c9c210355e610`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca03d365d608581c1ec95c9598c731f7ad23a5aada3e6cf3f922dd5b2f06aefe`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd652c8e3ea310658ef47c6b04dd8b10abbfdfa65f045b815927eefc3c11159`  
		Last Modified: Sat, 30 Apr 2022 00:14:38 GMT  
		Size: 71.5 MB (71505266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8582ce62371798e566652db61f61f6b3ac140e399d53b6bcada44b529bedd042`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71d811b1286367aff356ca96336aac53fee0fead10ee696d36e58a6482a9d7`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be419480cdcf62f9cee9f539c942f5b06825adb72c0410187c9a9c7e8fdc1dd`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:dbc2601a0da428fc25e3d403550a438bfcc8fd9cfd1a781a09cd93a184437f38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117723741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ea9e8a354784e1f553b08a6a4844b6ea7270601ceac2d5d2612d78f261b2bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:07:45 GMT
ADD file:d5447cb8fcc4a12030e43cda74f87e1bec09c6d1093307e25164127500f5e0d9 in / 
# Fri, 22 Apr 2022 08:07:52 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:46:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:47:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:47:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:48:02 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:48:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:48:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:48:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:48:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:48:44 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:46 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:48 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:53 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 10:49:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:50:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:50:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:50:33 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:50:35 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:50:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:50:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:50:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00422cde8b22ee0ff419263739625132280d08ffe78075ad3fb44dd003fab8e2`  
		Last Modified: Tue, 19 Apr 2022 13:12:05 GMT  
		Size: 30.4 MB (30442273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73a75b263aa5a8efa4063fe2cb0f0d32acae619cdc553734e3417e30d6b27bd`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e177e7220472e4fb95ebe55fc7c4df30f6f8e906eedcf2b2de96ee46427ddb27`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 5.6 MB (5630370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f94b997942bb04b6262987f676f71c4fcb3405275aaffa1d93cb2761cd992`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 3.5 MB (3533576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaaa83e354a55bc8695e97ccbe18ad1983635ddffc077397d9dcab59232a6ca`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0acb42415ce918b2ef55aa6ca28ff68811a35afd6397ddfad2745e9304fd51`  
		Last Modified: Fri, 22 Apr 2022 10:56:14 GMT  
		Size: 1.9 MB (1940450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37da9d58fff4c88201a1f7e6ca49ee9196e8ca997be6fe3f1fd8746e5c86e555`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d52f49a6d22ef0cdb764bed90008e3bb404704dd3a9d79bfb8553294c037909`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e181baf563e9972873f24b1166c5a0da1afe97ef128d2bab41ef59b7443f9cf0`  
		Last Modified: Fri, 22 Apr 2022 10:56:25 GMT  
		Size: 76.2 MB (76159138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11feb102b797ccfad139daa6fb6e80ad9b042348e827b5f259bd2a9c0e25fe3`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 3.5 KB (3499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a56146d487a5b8c4b9b6e79fdf91674d8c023a9bef40ff2639db425f8000ac0`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2563b23b40b5850bb08c2404b1e6ec15774ac8815fbba0b60d731bd0597820`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:f28c3f215c0786c06f9057a6c4638a9ce2af4ff1e6f7be51645f94e0b37f0def
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:8fcefbc6900276beaf7355e091c097ef57d2016e710fd202d325caeaae76d0a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109317051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e64d2ba5ee25d4a070b1d24ef9e9ff239efce9a68854eef75e6bad1bd14d115`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:53:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:53:40 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:53:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:53:53 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:53:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:54:01 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:54:01 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:54:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 02:54:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:54:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:54:37 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:54:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:54:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:54:38 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:54:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2b6021c87a182e98ffd2863b419bb79abb17cbe79278678bd9fe625af2fdf0`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765f601f0e14bf00b76a7c869dda18bb82726fb91ec363e01da58c1c7b443a3c`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 4.8 MB (4813346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01afffc2780257e621ca877a11e714b4a7c5c410f53d54498085dc40d6bfbc5`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 3.6 MB (3553293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3da9b715df5cce68601eb2b10a167f2a0fce8580873de81baa04625b3630777`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a2f060b97f61c909fac29a13ed6566d3582398b8aad97229e9cc5e8ff1b932`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 1.6 MB (1583545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd15d91ff5e8df79d2baef2f494b7a3630ab71ff3873ffa33312779f13c2221`  
		Last Modified: Fri, 22 Apr 2022 02:58:22 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbe407eaad30abd7fa7ea03f254a904ee2124fc3f320b3847677be56343ffb4`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866119df23a1053b37cbcf551ce1817f59f56a5201e1cefe3af83ac98b4fccfd`  
		Last Modified: Fri, 22 Apr 2022 02:58:31 GMT  
		Size: 72.6 MB (72639071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f565937cba773bda59caa0bfc5797250dedf1cbf2794053575300e6c8a306ffd`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d560a16832325d66ddca5bcd9b1e7d6026434f572a5965d8f6ff235e17bcdc`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e6b018aab576555b6e0bfd1b1b382e6ef1eed43e7c6956456e42bf5acf235c`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:83dec39d49c17442fafdc25e6f5d1bdc4d003e6fa19426a8120ef2a0dffb9169
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104258162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1ecb118afcb05518118a6c6c361190da87c708e8f13a79da8c86b5518219e8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:26 GMT
ADD file:78300bda9e889eaa778190cac0e569ff379d5e533e86b086248476e6ba9b4b2d in / 
# Fri, 29 Apr 2022 22:49:26 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:08:34 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:08:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:08:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:09:03 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:09:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:09:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:09:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:09:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:09:16 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 00:09:17 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 00:09:18 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 00:09:19 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 00:09:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Sat, 30 Apr 2022 00:09:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:09:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:09:48 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:09:50 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:09:51 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:09:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 00:09:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:09:53 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:09:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e196da37f904f62d236ea302bf13ba07711cc62b35774f86ecda18bcc9ed57c6`  
		Last Modified: Fri, 29 Apr 2022 22:51:14 GMT  
		Size: 23.7 MB (23735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddffcde8b39b72c10cbcd5d96f2307b6d6857369d4a57beb67277bd9f18aedc`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 1.9 KB (1854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed99cb2e83bbae3472b1b2ab68249e1c7dec481cc489c7d69b2627706d3058e7`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 4.3 MB (4261792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745c5d6a542769b03497a41228d4f31506c746d9f5ec5bf393f426c2a27c815b`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 3.2 MB (3207565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8e8f86c5634b4f012cd1f27e537c696a24e4c684810681da4d92d4f232d43a`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2279bacf1382c4ea4fafacc8f579b65d5e2c3949c934e3d1c3efe6fab90ec2cf`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 1.5 MB (1530621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e032a6d669d1fd06479b50389ac1237c010ebdc2fe3008e47c9c210355e610`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca03d365d608581c1ec95c9598c731f7ad23a5aada3e6cf3f922dd5b2f06aefe`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd652c8e3ea310658ef47c6b04dd8b10abbfdfa65f045b815927eefc3c11159`  
		Last Modified: Sat, 30 Apr 2022 00:14:38 GMT  
		Size: 71.5 MB (71505266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8582ce62371798e566652db61f61f6b3ac140e399d53b6bcada44b529bedd042`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71d811b1286367aff356ca96336aac53fee0fead10ee696d36e58a6482a9d7`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be419480cdcf62f9cee9f539c942f5b06825adb72c0410187c9a9c7e8fdc1dd`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:dbc2601a0da428fc25e3d403550a438bfcc8fd9cfd1a781a09cd93a184437f38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117723741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ea9e8a354784e1f553b08a6a4844b6ea7270601ceac2d5d2612d78f261b2bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:07:45 GMT
ADD file:d5447cb8fcc4a12030e43cda74f87e1bec09c6d1093307e25164127500f5e0d9 in / 
# Fri, 22 Apr 2022 08:07:52 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:46:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:47:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:47:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:48:02 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:48:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:48:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:48:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:48:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:48:44 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:46 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:48 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:53 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 10:49:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:50:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:50:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:50:33 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:50:35 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:50:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:50:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:50:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00422cde8b22ee0ff419263739625132280d08ffe78075ad3fb44dd003fab8e2`  
		Last Modified: Tue, 19 Apr 2022 13:12:05 GMT  
		Size: 30.4 MB (30442273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73a75b263aa5a8efa4063fe2cb0f0d32acae619cdc553734e3417e30d6b27bd`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e177e7220472e4fb95ebe55fc7c4df30f6f8e906eedcf2b2de96ee46427ddb27`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 5.6 MB (5630370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f94b997942bb04b6262987f676f71c4fcb3405275aaffa1d93cb2761cd992`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 3.5 MB (3533576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaaa83e354a55bc8695e97ccbe18ad1983635ddffc077397d9dcab59232a6ca`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0acb42415ce918b2ef55aa6ca28ff68811a35afd6397ddfad2745e9304fd51`  
		Last Modified: Fri, 22 Apr 2022 10:56:14 GMT  
		Size: 1.9 MB (1940450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37da9d58fff4c88201a1f7e6ca49ee9196e8ca997be6fe3f1fd8746e5c86e555`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d52f49a6d22ef0cdb764bed90008e3bb404704dd3a9d79bfb8553294c037909`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e181baf563e9972873f24b1166c5a0da1afe97ef128d2bab41ef59b7443f9cf0`  
		Last Modified: Fri, 22 Apr 2022 10:56:25 GMT  
		Size: 76.2 MB (76159138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11feb102b797ccfad139daa6fb6e80ad9b042348e827b5f259bd2a9c0e25fe3`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 3.5 KB (3499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a56146d487a5b8c4b9b6e79fdf91674d8c023a9bef40ff2639db425f8000ac0`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2563b23b40b5850bb08c2404b1e6ec15774ac8815fbba0b60d731bd0597820`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.43`

```console
$ docker pull mariadb@sha256:f28c3f215c0786c06f9057a6c4638a9ce2af4ff1e6f7be51645f94e0b37f0def
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.43` - linux; amd64

```console
$ docker pull mariadb@sha256:8fcefbc6900276beaf7355e091c097ef57d2016e710fd202d325caeaae76d0a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109317051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e64d2ba5ee25d4a070b1d24ef9e9ff239efce9a68854eef75e6bad1bd14d115`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:53:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:53:40 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:53:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:53:53 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:53:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:54:01 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:54:01 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:54:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 02:54:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:54:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:54:37 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:54:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:54:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:54:38 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:54:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2b6021c87a182e98ffd2863b419bb79abb17cbe79278678bd9fe625af2fdf0`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765f601f0e14bf00b76a7c869dda18bb82726fb91ec363e01da58c1c7b443a3c`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 4.8 MB (4813346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01afffc2780257e621ca877a11e714b4a7c5c410f53d54498085dc40d6bfbc5`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 3.6 MB (3553293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3da9b715df5cce68601eb2b10a167f2a0fce8580873de81baa04625b3630777`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a2f060b97f61c909fac29a13ed6566d3582398b8aad97229e9cc5e8ff1b932`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 1.6 MB (1583545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd15d91ff5e8df79d2baef2f494b7a3630ab71ff3873ffa33312779f13c2221`  
		Last Modified: Fri, 22 Apr 2022 02:58:22 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbe407eaad30abd7fa7ea03f254a904ee2124fc3f320b3847677be56343ffb4`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866119df23a1053b37cbcf551ce1817f59f56a5201e1cefe3af83ac98b4fccfd`  
		Last Modified: Fri, 22 Apr 2022 02:58:31 GMT  
		Size: 72.6 MB (72639071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f565937cba773bda59caa0bfc5797250dedf1cbf2794053575300e6c8a306ffd`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d560a16832325d66ddca5bcd9b1e7d6026434f572a5965d8f6ff235e17bcdc`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e6b018aab576555b6e0bfd1b1b382e6ef1eed43e7c6956456e42bf5acf235c`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:83dec39d49c17442fafdc25e6f5d1bdc4d003e6fa19426a8120ef2a0dffb9169
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104258162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1ecb118afcb05518118a6c6c361190da87c708e8f13a79da8c86b5518219e8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:26 GMT
ADD file:78300bda9e889eaa778190cac0e569ff379d5e533e86b086248476e6ba9b4b2d in / 
# Fri, 29 Apr 2022 22:49:26 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:08:34 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:08:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:08:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:09:03 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:09:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:09:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:09:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:09:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:09:16 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 00:09:17 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 00:09:18 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 00:09:19 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 00:09:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Sat, 30 Apr 2022 00:09:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:09:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:09:48 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:09:50 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:09:51 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:09:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 00:09:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:09:53 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:09:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e196da37f904f62d236ea302bf13ba07711cc62b35774f86ecda18bcc9ed57c6`  
		Last Modified: Fri, 29 Apr 2022 22:51:14 GMT  
		Size: 23.7 MB (23735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddffcde8b39b72c10cbcd5d96f2307b6d6857369d4a57beb67277bd9f18aedc`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 1.9 KB (1854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed99cb2e83bbae3472b1b2ab68249e1c7dec481cc489c7d69b2627706d3058e7`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 4.3 MB (4261792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745c5d6a542769b03497a41228d4f31506c746d9f5ec5bf393f426c2a27c815b`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 3.2 MB (3207565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8e8f86c5634b4f012cd1f27e537c696a24e4c684810681da4d92d4f232d43a`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2279bacf1382c4ea4fafacc8f579b65d5e2c3949c934e3d1c3efe6fab90ec2cf`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 1.5 MB (1530621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e032a6d669d1fd06479b50389ac1237c010ebdc2fe3008e47c9c210355e610`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca03d365d608581c1ec95c9598c731f7ad23a5aada3e6cf3f922dd5b2f06aefe`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd652c8e3ea310658ef47c6b04dd8b10abbfdfa65f045b815927eefc3c11159`  
		Last Modified: Sat, 30 Apr 2022 00:14:38 GMT  
		Size: 71.5 MB (71505266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8582ce62371798e566652db61f61f6b3ac140e399d53b6bcada44b529bedd042`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71d811b1286367aff356ca96336aac53fee0fead10ee696d36e58a6482a9d7`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be419480cdcf62f9cee9f539c942f5b06825adb72c0410187c9a9c7e8fdc1dd`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43` - linux; ppc64le

```console
$ docker pull mariadb@sha256:dbc2601a0da428fc25e3d403550a438bfcc8fd9cfd1a781a09cd93a184437f38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117723741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ea9e8a354784e1f553b08a6a4844b6ea7270601ceac2d5d2612d78f261b2bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:07:45 GMT
ADD file:d5447cb8fcc4a12030e43cda74f87e1bec09c6d1093307e25164127500f5e0d9 in / 
# Fri, 22 Apr 2022 08:07:52 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:46:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:47:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:47:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:48:02 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:48:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:48:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:48:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:48:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:48:44 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:46 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:48 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:53 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 10:49:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:50:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:50:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:50:33 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:50:35 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:50:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:50:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:50:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00422cde8b22ee0ff419263739625132280d08ffe78075ad3fb44dd003fab8e2`  
		Last Modified: Tue, 19 Apr 2022 13:12:05 GMT  
		Size: 30.4 MB (30442273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73a75b263aa5a8efa4063fe2cb0f0d32acae619cdc553734e3417e30d6b27bd`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e177e7220472e4fb95ebe55fc7c4df30f6f8e906eedcf2b2de96ee46427ddb27`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 5.6 MB (5630370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f94b997942bb04b6262987f676f71c4fcb3405275aaffa1d93cb2761cd992`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 3.5 MB (3533576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaaa83e354a55bc8695e97ccbe18ad1983635ddffc077397d9dcab59232a6ca`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0acb42415ce918b2ef55aa6ca28ff68811a35afd6397ddfad2745e9304fd51`  
		Last Modified: Fri, 22 Apr 2022 10:56:14 GMT  
		Size: 1.9 MB (1940450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37da9d58fff4c88201a1f7e6ca49ee9196e8ca997be6fe3f1fd8746e5c86e555`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d52f49a6d22ef0cdb764bed90008e3bb404704dd3a9d79bfb8553294c037909`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e181baf563e9972873f24b1166c5a0da1afe97ef128d2bab41ef59b7443f9cf0`  
		Last Modified: Fri, 22 Apr 2022 10:56:25 GMT  
		Size: 76.2 MB (76159138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11feb102b797ccfad139daa6fb6e80ad9b042348e827b5f259bd2a9c0e25fe3`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 3.5 KB (3499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a56146d487a5b8c4b9b6e79fdf91674d8c023a9bef40ff2639db425f8000ac0`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2563b23b40b5850bb08c2404b1e6ec15774ac8815fbba0b60d731bd0597820`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.43-bionic`

```console
$ docker pull mariadb@sha256:f28c3f215c0786c06f9057a6c4638a9ce2af4ff1e6f7be51645f94e0b37f0def
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.43-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:8fcefbc6900276beaf7355e091c097ef57d2016e710fd202d325caeaae76d0a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109317051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e64d2ba5ee25d4a070b1d24ef9e9ff239efce9a68854eef75e6bad1bd14d115`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:53:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:53:40 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:53:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:53:53 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:53:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:54:01 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:54:01 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:54:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 02:54:02 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 02:54:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 02:54:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:54:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:54:37 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:54:38 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:54:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:54:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:54:38 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:54:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2b6021c87a182e98ffd2863b419bb79abb17cbe79278678bd9fe625af2fdf0`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765f601f0e14bf00b76a7c869dda18bb82726fb91ec363e01da58c1c7b443a3c`  
		Last Modified: Fri, 22 Apr 2022 02:58:25 GMT  
		Size: 4.8 MB (4813346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01afffc2780257e621ca877a11e714b4a7c5c410f53d54498085dc40d6bfbc5`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 3.6 MB (3553293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3da9b715df5cce68601eb2b10a167f2a0fce8580873de81baa04625b3630777`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a2f060b97f61c909fac29a13ed6566d3582398b8aad97229e9cc5e8ff1b932`  
		Last Modified: Fri, 22 Apr 2022 02:58:23 GMT  
		Size: 1.6 MB (1583545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd15d91ff5e8df79d2baef2f494b7a3630ab71ff3873ffa33312779f13c2221`  
		Last Modified: Fri, 22 Apr 2022 02:58:22 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbe407eaad30abd7fa7ea03f254a904ee2124fc3f320b3847677be56343ffb4`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866119df23a1053b37cbcf551ce1817f59f56a5201e1cefe3af83ac98b4fccfd`  
		Last Modified: Fri, 22 Apr 2022 02:58:31 GMT  
		Size: 72.6 MB (72639071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f565937cba773bda59caa0bfc5797250dedf1cbf2794053575300e6c8a306ffd`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d560a16832325d66ddca5bcd9b1e7d6026434f572a5965d8f6ff235e17bcdc`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e6b018aab576555b6e0bfd1b1b382e6ef1eed43e7c6956456e42bf5acf235c`  
		Last Modified: Fri, 22 Apr 2022 02:58:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:83dec39d49c17442fafdc25e6f5d1bdc4d003e6fa19426a8120ef2a0dffb9169
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104258162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1ecb118afcb05518118a6c6c361190da87c708e8f13a79da8c86b5518219e8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:26 GMT
ADD file:78300bda9e889eaa778190cac0e569ff379d5e533e86b086248476e6ba9b4b2d in / 
# Fri, 29 Apr 2022 22:49:26 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:08:34 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:08:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:08:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:09:03 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:09:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:09:12 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:09:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:09:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:09:16 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 00:09:17 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 00:09:18 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 00:09:19 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 00:09:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Sat, 30 Apr 2022 00:09:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:09:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:09:48 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:09:50 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:09:51 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:09:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 00:09:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:09:53 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:09:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e196da37f904f62d236ea302bf13ba07711cc62b35774f86ecda18bcc9ed57c6`  
		Last Modified: Fri, 29 Apr 2022 22:51:14 GMT  
		Size: 23.7 MB (23735089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddffcde8b39b72c10cbcd5d96f2307b6d6857369d4a57beb67277bd9f18aedc`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 1.9 KB (1854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed99cb2e83bbae3472b1b2ab68249e1c7dec481cc489c7d69b2627706d3058e7`  
		Last Modified: Sat, 30 Apr 2022 00:14:32 GMT  
		Size: 4.3 MB (4261792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745c5d6a542769b03497a41228d4f31506c746d9f5ec5bf393f426c2a27c815b`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 3.2 MB (3207565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8e8f86c5634b4f012cd1f27e537c696a24e4c684810681da4d92d4f232d43a`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2279bacf1382c4ea4fafacc8f579b65d5e2c3949c934e3d1c3efe6fab90ec2cf`  
		Last Modified: Sat, 30 Apr 2022 00:14:30 GMT  
		Size: 1.5 MB (1530621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e032a6d669d1fd06479b50389ac1237c010ebdc2fe3008e47c9c210355e610`  
		Last Modified: Sat, 30 Apr 2022 00:14:29 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca03d365d608581c1ec95c9598c731f7ad23a5aada3e6cf3f922dd5b2f06aefe`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd652c8e3ea310658ef47c6b04dd8b10abbfdfa65f045b815927eefc3c11159`  
		Last Modified: Sat, 30 Apr 2022 00:14:38 GMT  
		Size: 71.5 MB (71505266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8582ce62371798e566652db61f61f6b3ac140e399d53b6bcada44b529bedd042`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71d811b1286367aff356ca96336aac53fee0fead10ee696d36e58a6482a9d7`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be419480cdcf62f9cee9f539c942f5b06825adb72c0410187c9a9c7e8fdc1dd`  
		Last Modified: Sat, 30 Apr 2022 00:14:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:dbc2601a0da428fc25e3d403550a438bfcc8fd9cfd1a781a09cd93a184437f38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117723741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ea9e8a354784e1f553b08a6a4844b6ea7270601ceac2d5d2612d78f261b2bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:07:45 GMT
ADD file:d5447cb8fcc4a12030e43cda74f87e1bec09c6d1093307e25164127500f5e0d9 in / 
# Fri, 22 Apr 2022 08:07:52 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:46:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:47:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:47:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:48:02 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:48:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:48:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:48:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:48:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:48:44 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:46 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 22 Apr 2022 10:48:48 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:53 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 22 Apr 2022 10:48:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 22 Apr 2022 10:49:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:50:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:50:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:50:33 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:50:35 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:50:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:50:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:50:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:50:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00422cde8b22ee0ff419263739625132280d08ffe78075ad3fb44dd003fab8e2`  
		Last Modified: Tue, 19 Apr 2022 13:12:05 GMT  
		Size: 30.4 MB (30442273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73a75b263aa5a8efa4063fe2cb0f0d32acae619cdc553734e3417e30d6b27bd`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e177e7220472e4fb95ebe55fc7c4df30f6f8e906eedcf2b2de96ee46427ddb27`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 5.6 MB (5630370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f94b997942bb04b6262987f676f71c4fcb3405275aaffa1d93cb2761cd992`  
		Last Modified: Fri, 22 Apr 2022 10:56:17 GMT  
		Size: 3.5 MB (3533576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaaa83e354a55bc8695e97ccbe18ad1983635ddffc077397d9dcab59232a6ca`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0acb42415ce918b2ef55aa6ca28ff68811a35afd6397ddfad2745e9304fd51`  
		Last Modified: Fri, 22 Apr 2022 10:56:14 GMT  
		Size: 1.9 MB (1940450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37da9d58fff4c88201a1f7e6ca49ee9196e8ca997be6fe3f1fd8746e5c86e555`  
		Last Modified: Fri, 22 Apr 2022 10:56:13 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d52f49a6d22ef0cdb764bed90008e3bb404704dd3a9d79bfb8553294c037909`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e181baf563e9972873f24b1166c5a0da1afe97ef128d2bab41ef59b7443f9cf0`  
		Last Modified: Fri, 22 Apr 2022 10:56:25 GMT  
		Size: 76.2 MB (76159138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11feb102b797ccfad139daa6fb6e80ad9b042348e827b5f259bd2a9c0e25fe3`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 3.5 KB (3499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a56146d487a5b8c4b9b6e79fdf91674d8c023a9bef40ff2639db425f8000ac0`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2563b23b40b5850bb08c2404b1e6ec15774ac8815fbba0b60d731bd0597820`  
		Last Modified: Fri, 22 Apr 2022 10:56:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:f6dfc11df1b13547001aa1aa6253d1bfdbc53efea01e742dc1fbf14bc437d6d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:3fadf7ebd60b5b879e6f9e2cd46c782e18c64ec78a5e1ddd5e587a779364933d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120117709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82643bd90d5e12d8dcc3923c5037bace1b14063504a971ec0498cf5e162bf61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:58 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:58 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:59 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:53:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:53:26 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:53:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:53:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:53:27 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:53:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7801d5a27d87a0a14725087a02be10adf3637adbacf9636d809795ed70a34ce`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7f812281a340552e5374feef34fd9a2563c703d0193aad89c90cf3fe9fe39a`  
		Last Modified: Fri, 22 Apr 2022 02:58:04 GMT  
		Size: 80.2 MB (80191115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b0502732e9ee8013217b08ed97cb6199c16b413212459861470162d7a1ea6d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fba0e3193601cd73bca932f9f778413d041e214ebad8a4a0b24f5ce35ec76d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2c705d6abdc6c36ec9ad28a43a47c9d00d5c2aa196ceee150b34001faaad4`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c7e75fdf4c42861ad3c3308ecb27884d1f5a1ad9456ee8340ffefaadf64a3647
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117607637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04e1678b50f5522c2bb9d42788974746509daa03b41b5a25c7824df65fda867b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:50 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 00:07:51 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 00:07:52 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 00:07:53 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 00:07:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:07:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:08:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:08:22 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:08:23 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:08:24 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:08:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 00:08:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:08:26 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:08:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827639ffd0f6973506d2471dc8f02b5a518193f49551d0557592bf7042952520`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cefc5946682e5ee04e15ca043c4a3f923a13a118a0e7180ff82527ea1efb2d`  
		Last Modified: Sat, 30 Apr 2022 00:14:08 GMT  
		Size: 79.5 MB (79530756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871eee533a53c8bb4d0151ee816fab7e5991ad89392849a15a169bb7424e73e0`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8898159042295570916d79f108aca4b2def594ba24a5f0bcf00f5532c612ebb`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa876d92dfdee70f9ec9d549c75cf0ea28d71e7c95d867b42fec0a5ca24c47ce`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:87b61f8379eb65a704fd612759413f1078a26d40e8d2bea31075c10e8e5c64c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131005136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d224c4121a61e5b5ed36485d24161c66509f7d3e5726444beca6059032c3a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:43:50 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:52 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:55 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:43:58 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:44:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:44:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:45:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:45:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:45:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:45:56 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:46:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:46:18 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e69825db8399a8e8531089312f836140b3c2e202cd9e9f8d3e33f2862140bf7`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f3a5eacd4b3852d2a6df25f3dcdbe1a2350a97ac7a75e7f6fef19cc6ce125d`  
		Last Modified: Fri, 22 Apr 2022 10:55:50 GMT  
		Size: 84.8 MB (84791769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127a0e21401b0104caee55b024a479dcacb37031f547853f5f157d65bb3afe1`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a468c88d3fc33c46a0b0bfc86b2251de989fffa4efb7f03fddd35192bd88acd`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413ee9ba3b320da907982067cc2460e9ae78998da3271ca620f0e122a465d7c5`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:f6dfc11df1b13547001aa1aa6253d1bfdbc53efea01e742dc1fbf14bc437d6d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:3fadf7ebd60b5b879e6f9e2cd46c782e18c64ec78a5e1ddd5e587a779364933d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120117709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82643bd90d5e12d8dcc3923c5037bace1b14063504a971ec0498cf5e162bf61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:58 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:58 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:59 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:53:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:53:26 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:53:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:53:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:53:27 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:53:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7801d5a27d87a0a14725087a02be10adf3637adbacf9636d809795ed70a34ce`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7f812281a340552e5374feef34fd9a2563c703d0193aad89c90cf3fe9fe39a`  
		Last Modified: Fri, 22 Apr 2022 02:58:04 GMT  
		Size: 80.2 MB (80191115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b0502732e9ee8013217b08ed97cb6199c16b413212459861470162d7a1ea6d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fba0e3193601cd73bca932f9f778413d041e214ebad8a4a0b24f5ce35ec76d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2c705d6abdc6c36ec9ad28a43a47c9d00d5c2aa196ceee150b34001faaad4`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c7e75fdf4c42861ad3c3308ecb27884d1f5a1ad9456ee8340ffefaadf64a3647
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117607637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04e1678b50f5522c2bb9d42788974746509daa03b41b5a25c7824df65fda867b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:50 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 00:07:51 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 00:07:52 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 00:07:53 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 00:07:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:07:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:08:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:08:22 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:08:23 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:08:24 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:08:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 00:08:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:08:26 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:08:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827639ffd0f6973506d2471dc8f02b5a518193f49551d0557592bf7042952520`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cefc5946682e5ee04e15ca043c4a3f923a13a118a0e7180ff82527ea1efb2d`  
		Last Modified: Sat, 30 Apr 2022 00:14:08 GMT  
		Size: 79.5 MB (79530756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871eee533a53c8bb4d0151ee816fab7e5991ad89392849a15a169bb7424e73e0`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8898159042295570916d79f108aca4b2def594ba24a5f0bcf00f5532c612ebb`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa876d92dfdee70f9ec9d549c75cf0ea28d71e7c95d867b42fec0a5ca24c47ce`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:87b61f8379eb65a704fd612759413f1078a26d40e8d2bea31075c10e8e5c64c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131005136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d224c4121a61e5b5ed36485d24161c66509f7d3e5726444beca6059032c3a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:43:50 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:52 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:55 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:43:58 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:44:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:44:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:45:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:45:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:45:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:45:56 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:46:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:46:18 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e69825db8399a8e8531089312f836140b3c2e202cd9e9f8d3e33f2862140bf7`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f3a5eacd4b3852d2a6df25f3dcdbe1a2350a97ac7a75e7f6fef19cc6ce125d`  
		Last Modified: Fri, 22 Apr 2022 10:55:50 GMT  
		Size: 84.8 MB (84791769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127a0e21401b0104caee55b024a479dcacb37031f547853f5f157d65bb3afe1`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a468c88d3fc33c46a0b0bfc86b2251de989fffa4efb7f03fddd35192bd88acd`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413ee9ba3b320da907982067cc2460e9ae78998da3271ca620f0e122a465d7c5`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.34`

```console
$ docker pull mariadb@sha256:f6dfc11df1b13547001aa1aa6253d1bfdbc53efea01e742dc1fbf14bc437d6d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.34` - linux; amd64

```console
$ docker pull mariadb@sha256:3fadf7ebd60b5b879e6f9e2cd46c782e18c64ec78a5e1ddd5e587a779364933d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120117709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82643bd90d5e12d8dcc3923c5037bace1b14063504a971ec0498cf5e162bf61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:58 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:58 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:59 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:53:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:53:26 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:53:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:53:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:53:27 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:53:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7801d5a27d87a0a14725087a02be10adf3637adbacf9636d809795ed70a34ce`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7f812281a340552e5374feef34fd9a2563c703d0193aad89c90cf3fe9fe39a`  
		Last Modified: Fri, 22 Apr 2022 02:58:04 GMT  
		Size: 80.2 MB (80191115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b0502732e9ee8013217b08ed97cb6199c16b413212459861470162d7a1ea6d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fba0e3193601cd73bca932f9f778413d041e214ebad8a4a0b24f5ce35ec76d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2c705d6abdc6c36ec9ad28a43a47c9d00d5c2aa196ceee150b34001faaad4`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c7e75fdf4c42861ad3c3308ecb27884d1f5a1ad9456ee8340ffefaadf64a3647
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117607637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04e1678b50f5522c2bb9d42788974746509daa03b41b5a25c7824df65fda867b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:50 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 00:07:51 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 00:07:52 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 00:07:53 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 00:07:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:07:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:08:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:08:22 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:08:23 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:08:24 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:08:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 00:08:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:08:26 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:08:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827639ffd0f6973506d2471dc8f02b5a518193f49551d0557592bf7042952520`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cefc5946682e5ee04e15ca043c4a3f923a13a118a0e7180ff82527ea1efb2d`  
		Last Modified: Sat, 30 Apr 2022 00:14:08 GMT  
		Size: 79.5 MB (79530756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871eee533a53c8bb4d0151ee816fab7e5991ad89392849a15a169bb7424e73e0`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8898159042295570916d79f108aca4b2def594ba24a5f0bcf00f5532c612ebb`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa876d92dfdee70f9ec9d549c75cf0ea28d71e7c95d867b42fec0a5ca24c47ce`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34` - linux; ppc64le

```console
$ docker pull mariadb@sha256:87b61f8379eb65a704fd612759413f1078a26d40e8d2bea31075c10e8e5c64c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131005136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d224c4121a61e5b5ed36485d24161c66509f7d3e5726444beca6059032c3a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:43:50 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:52 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:55 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:43:58 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:44:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:44:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:45:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:45:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:45:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:45:56 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:46:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:46:18 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e69825db8399a8e8531089312f836140b3c2e202cd9e9f8d3e33f2862140bf7`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f3a5eacd4b3852d2a6df25f3dcdbe1a2350a97ac7a75e7f6fef19cc6ce125d`  
		Last Modified: Fri, 22 Apr 2022 10:55:50 GMT  
		Size: 84.8 MB (84791769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127a0e21401b0104caee55b024a479dcacb37031f547853f5f157d65bb3afe1`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a468c88d3fc33c46a0b0bfc86b2251de989fffa4efb7f03fddd35192bd88acd`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413ee9ba3b320da907982067cc2460e9ae78998da3271ca620f0e122a465d7c5`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.34-focal`

```console
$ docker pull mariadb@sha256:f6dfc11df1b13547001aa1aa6253d1bfdbc53efea01e742dc1fbf14bc437d6d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.34-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:3fadf7ebd60b5b879e6f9e2cd46c782e18c64ec78a5e1ddd5e587a779364933d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120117709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82643bd90d5e12d8dcc3923c5037bace1b14063504a971ec0498cf5e162bf61f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:58 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:58 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 02:52:59 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 02:52:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:53:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:53:26 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:53:26 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:53:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:53:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:53:27 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:53:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7801d5a27d87a0a14725087a02be10adf3637adbacf9636d809795ed70a34ce`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7f812281a340552e5374feef34fd9a2563c703d0193aad89c90cf3fe9fe39a`  
		Last Modified: Fri, 22 Apr 2022 02:58:04 GMT  
		Size: 80.2 MB (80191115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b0502732e9ee8013217b08ed97cb6199c16b413212459861470162d7a1ea6d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fba0e3193601cd73bca932f9f778413d041e214ebad8a4a0b24f5ce35ec76d`  
		Last Modified: Fri, 22 Apr 2022 02:57:53 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c2c705d6abdc6c36ec9ad28a43a47c9d00d5c2aa196ceee150b34001faaad4`  
		Last Modified: Fri, 22 Apr 2022 02:57:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c7e75fdf4c42861ad3c3308ecb27884d1f5a1ad9456ee8340ffefaadf64a3647
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117607637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04e1678b50f5522c2bb9d42788974746509daa03b41b5a25c7824df65fda867b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:50 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 00:07:51 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 00:07:52 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 00:07:53 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 00:07:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:07:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:08:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:08:22 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:08:23 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:08:24 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:08:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 00:08:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:08:26 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:08:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827639ffd0f6973506d2471dc8f02b5a518193f49551d0557592bf7042952520`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cefc5946682e5ee04e15ca043c4a3f923a13a118a0e7180ff82527ea1efb2d`  
		Last Modified: Sat, 30 Apr 2022 00:14:08 GMT  
		Size: 79.5 MB (79530756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871eee533a53c8bb4d0151ee816fab7e5991ad89392849a15a169bb7424e73e0`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8898159042295570916d79f108aca4b2def594ba24a5f0bcf00f5532c612ebb`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa876d92dfdee70f9ec9d549c75cf0ea28d71e7c95d867b42fec0a5ca24c47ce`  
		Last Modified: Sat, 30 Apr 2022 00:13:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:87b61f8379eb65a704fd612759413f1078a26d40e8d2bea31075c10e8e5c64c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131005136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d224c4121a61e5b5ed36485d24161c66509f7d3e5726444beca6059032c3a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:43:50 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:52 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 22 Apr 2022 10:43:55 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:43:58 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 22 Apr 2022 10:44:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:44:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:45:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:45:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:45:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:45:56 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:46:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:46:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:46:18 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e69825db8399a8e8531089312f836140b3c2e202cd9e9f8d3e33f2862140bf7`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f3a5eacd4b3852d2a6df25f3dcdbe1a2350a97ac7a75e7f6fef19cc6ce125d`  
		Last Modified: Fri, 22 Apr 2022 10:55:50 GMT  
		Size: 84.8 MB (84791769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3127a0e21401b0104caee55b024a479dcacb37031f547853f5f157d65bb3afe1`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a468c88d3fc33c46a0b0bfc86b2251de989fffa4efb7f03fddd35192bd88acd`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413ee9ba3b320da907982067cc2460e9ae78998da3271ca620f0e122a465d7c5`  
		Last Modified: Fri, 22 Apr 2022 10:55:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:003b0917c376a4d15014f8941327f3f7d5f3cd214d34dc939e5ec1d7d29734c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:819963937619a1891b4e1f4c6125d4ea4f3bb6195d72042307ae2cd68071b1ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad3c8256a516f93654aed599432527de806b5da9c2088233c692591c291a9a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:55 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b744c9184d699263c8a3ef44c0767a0429db8c6892701eef91c0237b61421e5`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d15a78b4ec63a31d0349185788c72af768e99002fcbb2a6a46c3a8a6fd263eb`  
		Last Modified: Fri, 22 Apr 2022 02:57:36 GMT  
		Size: 85.8 MB (85753125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76088cf45319c739b3d59169b2c599481218be04824f4aadb20657eb83c43f1b`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4519dcc8d4be31b8246d8f666c1db6c7eab0ff35ade6ece88c6b7f39a784d29`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f902b376b26e5290db3e69f9cfadc24be1001705c68c97205619cd98b2a00d`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8bfb170f85dabe8990a7f8c617ed3e166268e3551e7c833a4fdae67f80bb8d2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123003140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c8ce1f7ba4010e4154d4dd2c21c60dcd436a8bc46f37e14267a510356f6e9eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:07 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 00:07:07 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 00:07:08 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 00:07:09 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 00:07:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:07:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:07:35 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:07:36 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:07:37 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:07:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 00:07:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:07:39 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:07:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2370afa0cb3644b2d9be6e26d9f9b610d0295bff4feb0d2bcdaf56b85e187c1e`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5728e1dcaaddd66fbda9f16cd0772c895a00a5d8c15918137a9836fce7d946b1`  
		Last Modified: Sat, 30 Apr 2022 00:13:37 GMT  
		Size: 84.9 MB (84926260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5b639137cad7da2c5b759893b3e2db6c6a44fd7595c455c94db6d6ea6ab296`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2a7a95b3d3793d60733ed2e6a2d3d33157f28f10e04e9da497dc61c62918cb`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bc2c849485f68cc5dcb289be30577925d4c7ce0864c28354c461c2843fff2f`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2a66bce22b31b71f3e4c5ca55d1344053c2405d40cbd5cd2d6db8583f8b498d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136559157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e3ed094c127c558d29be417acf0ef28f516f3c6ce0059d914ad23b1dd1e0abc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:41:09 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:11 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:13 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:15 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:41:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:43:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:43:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:43:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:43:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:43:29 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:43:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7f41e21911d9adde7defbce93577afcf701ee7053f4465df314a9652f54872`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e15a11cf0a1e0548f3cca3664f091c4b1b78d83e51c62656c5e57113914280b`  
		Last Modified: Fri, 22 Apr 2022 10:55:12 GMT  
		Size: 90.3 MB (90345786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9773723ca77bed5f552c2e35fb43ee9cc4c3c575340c8d985ae91428a19f15a0`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6560ee8fe30273309437e97324852b4d11e1d5d9190e485cf4f44ac6d50320b3`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7263353b18e3000afe4ce89fc5a3eb2462783f322c68298b0c7a90fc76acc8`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:003b0917c376a4d15014f8941327f3f7d5f3cd214d34dc939e5ec1d7d29734c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:819963937619a1891b4e1f4c6125d4ea4f3bb6195d72042307ae2cd68071b1ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad3c8256a516f93654aed599432527de806b5da9c2088233c692591c291a9a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:55 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b744c9184d699263c8a3ef44c0767a0429db8c6892701eef91c0237b61421e5`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d15a78b4ec63a31d0349185788c72af768e99002fcbb2a6a46c3a8a6fd263eb`  
		Last Modified: Fri, 22 Apr 2022 02:57:36 GMT  
		Size: 85.8 MB (85753125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76088cf45319c739b3d59169b2c599481218be04824f4aadb20657eb83c43f1b`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4519dcc8d4be31b8246d8f666c1db6c7eab0ff35ade6ece88c6b7f39a784d29`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f902b376b26e5290db3e69f9cfadc24be1001705c68c97205619cd98b2a00d`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8bfb170f85dabe8990a7f8c617ed3e166268e3551e7c833a4fdae67f80bb8d2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123003140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c8ce1f7ba4010e4154d4dd2c21c60dcd436a8bc46f37e14267a510356f6e9eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:07 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 00:07:07 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 00:07:08 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 00:07:09 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 00:07:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:07:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:07:35 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:07:36 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:07:37 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:07:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 00:07:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:07:39 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:07:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2370afa0cb3644b2d9be6e26d9f9b610d0295bff4feb0d2bcdaf56b85e187c1e`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5728e1dcaaddd66fbda9f16cd0772c895a00a5d8c15918137a9836fce7d946b1`  
		Last Modified: Sat, 30 Apr 2022 00:13:37 GMT  
		Size: 84.9 MB (84926260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5b639137cad7da2c5b759893b3e2db6c6a44fd7595c455c94db6d6ea6ab296`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2a7a95b3d3793d60733ed2e6a2d3d33157f28f10e04e9da497dc61c62918cb`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bc2c849485f68cc5dcb289be30577925d4c7ce0864c28354c461c2843fff2f`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2a66bce22b31b71f3e4c5ca55d1344053c2405d40cbd5cd2d6db8583f8b498d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136559157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e3ed094c127c558d29be417acf0ef28f516f3c6ce0059d914ad23b1dd1e0abc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:41:09 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:11 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:13 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:15 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:41:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:43:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:43:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:43:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:43:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:43:29 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:43:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7f41e21911d9adde7defbce93577afcf701ee7053f4465df314a9652f54872`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e15a11cf0a1e0548f3cca3664f091c4b1b78d83e51c62656c5e57113914280b`  
		Last Modified: Fri, 22 Apr 2022 10:55:12 GMT  
		Size: 90.3 MB (90345786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9773723ca77bed5f552c2e35fb43ee9cc4c3c575340c8d985ae91428a19f15a0`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6560ee8fe30273309437e97324852b4d11e1d5d9190e485cf4f44ac6d50320b3`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7263353b18e3000afe4ce89fc5a3eb2462783f322c68298b0c7a90fc76acc8`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.24`

```console
$ docker pull mariadb@sha256:003b0917c376a4d15014f8941327f3f7d5f3cd214d34dc939e5ec1d7d29734c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.24` - linux; amd64

```console
$ docker pull mariadb@sha256:819963937619a1891b4e1f4c6125d4ea4f3bb6195d72042307ae2cd68071b1ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad3c8256a516f93654aed599432527de806b5da9c2088233c692591c291a9a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:55 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b744c9184d699263c8a3ef44c0767a0429db8c6892701eef91c0237b61421e5`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d15a78b4ec63a31d0349185788c72af768e99002fcbb2a6a46c3a8a6fd263eb`  
		Last Modified: Fri, 22 Apr 2022 02:57:36 GMT  
		Size: 85.8 MB (85753125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76088cf45319c739b3d59169b2c599481218be04824f4aadb20657eb83c43f1b`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4519dcc8d4be31b8246d8f666c1db6c7eab0ff35ade6ece88c6b7f39a784d29`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f902b376b26e5290db3e69f9cfadc24be1001705c68c97205619cd98b2a00d`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8bfb170f85dabe8990a7f8c617ed3e166268e3551e7c833a4fdae67f80bb8d2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123003140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c8ce1f7ba4010e4154d4dd2c21c60dcd436a8bc46f37e14267a510356f6e9eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:07 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 00:07:07 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 00:07:08 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 00:07:09 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 00:07:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:07:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:07:35 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:07:36 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:07:37 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:07:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 00:07:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:07:39 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:07:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2370afa0cb3644b2d9be6e26d9f9b610d0295bff4feb0d2bcdaf56b85e187c1e`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5728e1dcaaddd66fbda9f16cd0772c895a00a5d8c15918137a9836fce7d946b1`  
		Last Modified: Sat, 30 Apr 2022 00:13:37 GMT  
		Size: 84.9 MB (84926260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5b639137cad7da2c5b759893b3e2db6c6a44fd7595c455c94db6d6ea6ab296`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2a7a95b3d3793d60733ed2e6a2d3d33157f28f10e04e9da497dc61c62918cb`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bc2c849485f68cc5dcb289be30577925d4c7ce0864c28354c461c2843fff2f`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2a66bce22b31b71f3e4c5ca55d1344053c2405d40cbd5cd2d6db8583f8b498d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136559157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e3ed094c127c558d29be417acf0ef28f516f3c6ce0059d914ad23b1dd1e0abc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:41:09 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:11 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:13 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:15 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:41:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:43:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:43:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:43:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:43:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:43:29 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:43:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7f41e21911d9adde7defbce93577afcf701ee7053f4465df314a9652f54872`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e15a11cf0a1e0548f3cca3664f091c4b1b78d83e51c62656c5e57113914280b`  
		Last Modified: Fri, 22 Apr 2022 10:55:12 GMT  
		Size: 90.3 MB (90345786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9773723ca77bed5f552c2e35fb43ee9cc4c3c575340c8d985ae91428a19f15a0`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6560ee8fe30273309437e97324852b4d11e1d5d9190e485cf4f44ac6d50320b3`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7263353b18e3000afe4ce89fc5a3eb2462783f322c68298b0c7a90fc76acc8`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.24-focal`

```console
$ docker pull mariadb@sha256:003b0917c376a4d15014f8941327f3f7d5f3cd214d34dc939e5ec1d7d29734c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.24-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:819963937619a1891b4e1f4c6125d4ea4f3bb6195d72042307ae2cd68071b1ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad3c8256a516f93654aed599432527de806b5da9c2088233c692591c291a9a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 02:52:31 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 02:52:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:54 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 02:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:55 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b744c9184d699263c8a3ef44c0767a0429db8c6892701eef91c0237b61421e5`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d15a78b4ec63a31d0349185788c72af768e99002fcbb2a6a46c3a8a6fd263eb`  
		Last Modified: Fri, 22 Apr 2022 02:57:36 GMT  
		Size: 85.8 MB (85753125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76088cf45319c739b3d59169b2c599481218be04824f4aadb20657eb83c43f1b`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4519dcc8d4be31b8246d8f666c1db6c7eab0ff35ade6ece88c6b7f39a784d29`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f902b376b26e5290db3e69f9cfadc24be1001705c68c97205619cd98b2a00d`  
		Last Modified: Fri, 22 Apr 2022 02:57:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8bfb170f85dabe8990a7f8c617ed3e166268e3551e7c833a4fdae67f80bb8d2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123003140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c8ce1f7ba4010e4154d4dd2c21c60dcd436a8bc46f37e14267a510356f6e9eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:07:07 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 00:07:07 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 00:07:08 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 00:07:09 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 00:07:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:07:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:07:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:07:35 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:07:36 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:07:37 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:07:37 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 00:07:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:07:39 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:07:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2370afa0cb3644b2d9be6e26d9f9b610d0295bff4feb0d2bcdaf56b85e187c1e`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5728e1dcaaddd66fbda9f16cd0772c895a00a5d8c15918137a9836fce7d946b1`  
		Last Modified: Sat, 30 Apr 2022 00:13:37 GMT  
		Size: 84.9 MB (84926260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5b639137cad7da2c5b759893b3e2db6c6a44fd7595c455c94db6d6ea6ab296`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2a7a95b3d3793d60733ed2e6a2d3d33157f28f10e04e9da497dc61c62918cb`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bc2c849485f68cc5dcb289be30577925d4c7ce0864c28354c461c2843fff2f`  
		Last Modified: Sat, 30 Apr 2022 00:13:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:2a66bce22b31b71f3e4c5ca55d1344053c2405d40cbd5cd2d6db8583f8b498d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136559157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e3ed094c127c558d29be417acf0ef28f516f3c6ce0059d914ad23b1dd1e0abc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:41:09 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:11 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 22 Apr 2022 10:41:13 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:15 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 22 Apr 2022 10:41:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:41:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:43:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:43:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:43:18 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:43:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 22 Apr 2022 10:43:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:43:29 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:43:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7f41e21911d9adde7defbce93577afcf701ee7053f4465df314a9652f54872`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e15a11cf0a1e0548f3cca3664f091c4b1b78d83e51c62656c5e57113914280b`  
		Last Modified: Fri, 22 Apr 2022 10:55:12 GMT  
		Size: 90.3 MB (90345786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9773723ca77bed5f552c2e35fb43ee9cc4c3c575340c8d985ae91428a19f15a0`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6560ee8fe30273309437e97324852b4d11e1d5d9190e485cf4f44ac6d50320b3`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7263353b18e3000afe4ce89fc5a3eb2462783f322c68298b0c7a90fc76acc8`  
		Last Modified: Fri, 22 Apr 2022 10:54:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:05cb37411dcd35206d03d2f2ea409f40bc6a6b6585b4085b025a2c868f505a1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:5d5daf7e35f3b1e8dc54b7f279bf8d0fabdc5489f329b9e4af289e92c692abd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127923752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8247f649c1ad0ed98bded330f521a2114583f7d253dcb91228d0f865e76ac90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:25 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490dd7915b8002205becea23f1301b54b93df661098f49fb349100eace3c473d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0791622d551403008eaaa8a55b8c2ce888d9cf059518ffec3789cef789c4c987`  
		Last Modified: Fri, 22 Apr 2022 02:57:07 GMT  
		Size: 88.0 MB (87997283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43c35539e9763ffe7ff15d83e7fe71d078c83207758e1114050595ca29ecfc9`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42c10e4d1ed516fbfdc6e0848f37064f65ff78b2638f1c30002dbd8850e140d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ec36f331246daf3dc3028e12eda26f596b77d4a15287b24f73fa1fb46f16a3fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125185435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb7ed9035465fdb35e183d804c6fa5af0d792feb30fc46c09158d87debbad8a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:06:23 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 00:06:24 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 00:06:25 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 00:06:26 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 00:06:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:06:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:06:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:06:51 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:06:53 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:06:54 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:06:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:06:55 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:06:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ec2c785fac5ffcee396e609a7abadf074df38ac9625705b0723ae245864028`  
		Last Modified: Sat, 30 Apr 2022 00:12:51 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b9f507571abbf14efa935e4102855354c36573d6d0e0987c74d40b5085409e`  
		Last Modified: Sat, 30 Apr 2022 00:13:04 GMT  
		Size: 87.1 MB (87108678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b714e50265e492fa21c91d4b927d5fcafa6d9ce6b64bb51a89f69c63688c298`  
		Last Modified: Sat, 30 Apr 2022 00:12:51 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71962414ed60d8a6fec935ad5e7b8b6982d7c41382f74e52a30b110f90f57b63`  
		Last Modified: Sat, 30 Apr 2022 00:12:51 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7253c8bbce09ad62f4aedb92fb4ece6de9a8a6b9389b70fd915a2630bc910810
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138780434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b5ae0af269fec9ab843a97f38af5e144f1d13e845da7729991e23afb6c4820`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:38:45 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:48 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:50 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:53 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:39:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:40:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:40:39 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:40:41 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:40:42 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:40:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:40:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:40:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8585fdfb939ad59fe43800e8258791cae1a48fe19fc82bc5b28ee7cea88e25a6`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55c8c0f19134ea3f4e78d7db234e964e8f9b8a28d596ebe4a625594319f9159`  
		Last Modified: Fri, 22 Apr 2022 10:54:35 GMT  
		Size: 92.6 MB (92567188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd4f314b64534547b791600e31d8158b548b2fe4e79ecc4da4285aea8a8741`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47740fd99121c3a1f7c4c4125a8beb046167869d84ae7ed84c2f6ea1ae329ee8`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; s390x

```console
$ docker pull mariadb@sha256:c5787d0833702e64bbf45c367044853ba5758d107d383b1b6b7ea848d621a038
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127176421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f9a36fde17b045be592b43bab340b70a084c0974ae644be98e846bbd0c0e1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:47:08 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 29 Apr 2022 23:47:08 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 29 Apr 2022 23:47:08 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 29 Apr 2022 23:47:08 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 29 Apr 2022 23:47:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:47:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:47:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:47:43 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:47:43 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:47:44 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:47:44 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:47:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e342171dfa0498624df901d3be0c1f25da8848b11c6e600397573b26af1dba63`  
		Last Modified: Fri, 29 Apr 2022 23:49:51 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef89698870d6a80a263874ac4e55383d084b81c60e0f13a55ac4525da23f171`  
		Last Modified: Fri, 29 Apr 2022 23:50:04 GMT  
		Size: 89.3 MB (89290156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e7960c465106f14ae6c5868a026fe66b071bb347e80c15b341a1e6ecd1d1da`  
		Last Modified: Fri, 29 Apr 2022 23:49:51 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e880dc457b58bf0de1aa5d2e9ac2d4275ae61a6c9e078e8f73c8be19c971d2d`  
		Last Modified: Fri, 29 Apr 2022 23:49:51 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:05cb37411dcd35206d03d2f2ea409f40bc6a6b6585b4085b025a2c868f505a1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:5d5daf7e35f3b1e8dc54b7f279bf8d0fabdc5489f329b9e4af289e92c692abd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127923752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8247f649c1ad0ed98bded330f521a2114583f7d253dcb91228d0f865e76ac90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:25 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490dd7915b8002205becea23f1301b54b93df661098f49fb349100eace3c473d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0791622d551403008eaaa8a55b8c2ce888d9cf059518ffec3789cef789c4c987`  
		Last Modified: Fri, 22 Apr 2022 02:57:07 GMT  
		Size: 88.0 MB (87997283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43c35539e9763ffe7ff15d83e7fe71d078c83207758e1114050595ca29ecfc9`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42c10e4d1ed516fbfdc6e0848f37064f65ff78b2638f1c30002dbd8850e140d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ec36f331246daf3dc3028e12eda26f596b77d4a15287b24f73fa1fb46f16a3fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125185435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb7ed9035465fdb35e183d804c6fa5af0d792feb30fc46c09158d87debbad8a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:06:23 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 00:06:24 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 00:06:25 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 00:06:26 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 00:06:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:06:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:06:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:06:51 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:06:53 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:06:54 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:06:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:06:55 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:06:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ec2c785fac5ffcee396e609a7abadf074df38ac9625705b0723ae245864028`  
		Last Modified: Sat, 30 Apr 2022 00:12:51 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b9f507571abbf14efa935e4102855354c36573d6d0e0987c74d40b5085409e`  
		Last Modified: Sat, 30 Apr 2022 00:13:04 GMT  
		Size: 87.1 MB (87108678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b714e50265e492fa21c91d4b927d5fcafa6d9ce6b64bb51a89f69c63688c298`  
		Last Modified: Sat, 30 Apr 2022 00:12:51 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71962414ed60d8a6fec935ad5e7b8b6982d7c41382f74e52a30b110f90f57b63`  
		Last Modified: Sat, 30 Apr 2022 00:12:51 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7253c8bbce09ad62f4aedb92fb4ece6de9a8a6b9389b70fd915a2630bc910810
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138780434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b5ae0af269fec9ab843a97f38af5e144f1d13e845da7729991e23afb6c4820`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:38:45 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:48 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:50 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:53 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:39:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:40:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:40:39 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:40:41 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:40:42 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:40:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:40:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:40:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8585fdfb939ad59fe43800e8258791cae1a48fe19fc82bc5b28ee7cea88e25a6`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55c8c0f19134ea3f4e78d7db234e964e8f9b8a28d596ebe4a625594319f9159`  
		Last Modified: Fri, 22 Apr 2022 10:54:35 GMT  
		Size: 92.6 MB (92567188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd4f314b64534547b791600e31d8158b548b2fe4e79ecc4da4285aea8a8741`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47740fd99121c3a1f7c4c4125a8beb046167869d84ae7ed84c2f6ea1ae329ee8`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:c5787d0833702e64bbf45c367044853ba5758d107d383b1b6b7ea848d621a038
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127176421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f9a36fde17b045be592b43bab340b70a084c0974ae644be98e846bbd0c0e1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:47:08 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 29 Apr 2022 23:47:08 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 29 Apr 2022 23:47:08 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 29 Apr 2022 23:47:08 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 29 Apr 2022 23:47:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:47:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:47:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:47:43 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:47:43 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:47:44 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:47:44 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:47:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e342171dfa0498624df901d3be0c1f25da8848b11c6e600397573b26af1dba63`  
		Last Modified: Fri, 29 Apr 2022 23:49:51 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef89698870d6a80a263874ac4e55383d084b81c60e0f13a55ac4525da23f171`  
		Last Modified: Fri, 29 Apr 2022 23:50:04 GMT  
		Size: 89.3 MB (89290156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e7960c465106f14ae6c5868a026fe66b071bb347e80c15b341a1e6ecd1d1da`  
		Last Modified: Fri, 29 Apr 2022 23:49:51 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e880dc457b58bf0de1aa5d2e9ac2d4275ae61a6c9e078e8f73c8be19c971d2d`  
		Last Modified: Fri, 29 Apr 2022 23:49:51 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.15`

```console
$ docker pull mariadb@sha256:05cb37411dcd35206d03d2f2ea409f40bc6a6b6585b4085b025a2c868f505a1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.15` - linux; amd64

```console
$ docker pull mariadb@sha256:5d5daf7e35f3b1e8dc54b7f279bf8d0fabdc5489f329b9e4af289e92c692abd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127923752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8247f649c1ad0ed98bded330f521a2114583f7d253dcb91228d0f865e76ac90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:25 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490dd7915b8002205becea23f1301b54b93df661098f49fb349100eace3c473d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0791622d551403008eaaa8a55b8c2ce888d9cf059518ffec3789cef789c4c987`  
		Last Modified: Fri, 22 Apr 2022 02:57:07 GMT  
		Size: 88.0 MB (87997283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43c35539e9763ffe7ff15d83e7fe71d078c83207758e1114050595ca29ecfc9`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42c10e4d1ed516fbfdc6e0848f37064f65ff78b2638f1c30002dbd8850e140d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ec36f331246daf3dc3028e12eda26f596b77d4a15287b24f73fa1fb46f16a3fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125185435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb7ed9035465fdb35e183d804c6fa5af0d792feb30fc46c09158d87debbad8a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:06:23 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 00:06:24 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 00:06:25 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 00:06:26 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 00:06:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:06:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:06:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:06:51 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:06:53 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:06:54 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:06:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:06:55 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:06:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ec2c785fac5ffcee396e609a7abadf074df38ac9625705b0723ae245864028`  
		Last Modified: Sat, 30 Apr 2022 00:12:51 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b9f507571abbf14efa935e4102855354c36573d6d0e0987c74d40b5085409e`  
		Last Modified: Sat, 30 Apr 2022 00:13:04 GMT  
		Size: 87.1 MB (87108678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b714e50265e492fa21c91d4b927d5fcafa6d9ce6b64bb51a89f69c63688c298`  
		Last Modified: Sat, 30 Apr 2022 00:12:51 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71962414ed60d8a6fec935ad5e7b8b6982d7c41382f74e52a30b110f90f57b63`  
		Last Modified: Sat, 30 Apr 2022 00:12:51 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7253c8bbce09ad62f4aedb92fb4ece6de9a8a6b9389b70fd915a2630bc910810
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138780434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b5ae0af269fec9ab843a97f38af5e144f1d13e845da7729991e23afb6c4820`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:38:45 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:48 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:50 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:53 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:39:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:40:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:40:39 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:40:41 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:40:42 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:40:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:40:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:40:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8585fdfb939ad59fe43800e8258791cae1a48fe19fc82bc5b28ee7cea88e25a6`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55c8c0f19134ea3f4e78d7db234e964e8f9b8a28d596ebe4a625594319f9159`  
		Last Modified: Fri, 22 Apr 2022 10:54:35 GMT  
		Size: 92.6 MB (92567188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd4f314b64534547b791600e31d8158b548b2fe4e79ecc4da4285aea8a8741`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47740fd99121c3a1f7c4c4125a8beb046167869d84ae7ed84c2f6ea1ae329ee8`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; s390x

```console
$ docker pull mariadb@sha256:c5787d0833702e64bbf45c367044853ba5758d107d383b1b6b7ea848d621a038
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127176421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f9a36fde17b045be592b43bab340b70a084c0974ae644be98e846bbd0c0e1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:47:08 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 29 Apr 2022 23:47:08 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 29 Apr 2022 23:47:08 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 29 Apr 2022 23:47:08 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 29 Apr 2022 23:47:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:47:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:47:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:47:43 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:47:43 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:47:44 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:47:44 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:47:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e342171dfa0498624df901d3be0c1f25da8848b11c6e600397573b26af1dba63`  
		Last Modified: Fri, 29 Apr 2022 23:49:51 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef89698870d6a80a263874ac4e55383d084b81c60e0f13a55ac4525da23f171`  
		Last Modified: Fri, 29 Apr 2022 23:50:04 GMT  
		Size: 89.3 MB (89290156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e7960c465106f14ae6c5868a026fe66b071bb347e80c15b341a1e6ecd1d1da`  
		Last Modified: Fri, 29 Apr 2022 23:49:51 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e880dc457b58bf0de1aa5d2e9ac2d4275ae61a6c9e078e8f73c8be19c971d2d`  
		Last Modified: Fri, 29 Apr 2022 23:49:51 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.15-focal`

```console
$ docker pull mariadb@sha256:05cb37411dcd35206d03d2f2ea409f40bc6a6b6585b4085b025a2c868f505a1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.15-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:5d5daf7e35f3b1e8dc54b7f279bf8d0fabdc5489f329b9e4af289e92c692abd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127923752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8247f649c1ad0ed98bded330f521a2114583f7d253dcb91228d0f865e76ac90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 02:52:03 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 02:52:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:52:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:52:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:52:25 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:52:25 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:52:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:52:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490dd7915b8002205becea23f1301b54b93df661098f49fb349100eace3c473d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0791622d551403008eaaa8a55b8c2ce888d9cf059518ffec3789cef789c4c987`  
		Last Modified: Fri, 22 Apr 2022 02:57:07 GMT  
		Size: 88.0 MB (87997283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43c35539e9763ffe7ff15d83e7fe71d078c83207758e1114050595ca29ecfc9`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42c10e4d1ed516fbfdc6e0848f37064f65ff78b2638f1c30002dbd8850e140d`  
		Last Modified: Fri, 22 Apr 2022 02:56:54 GMT  
		Size: 6.8 KB (6769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ec36f331246daf3dc3028e12eda26f596b77d4a15287b24f73fa1fb46f16a3fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125185435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb7ed9035465fdb35e183d804c6fa5af0d792feb30fc46c09158d87debbad8a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:06:23 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 00:06:24 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 00:06:25 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 00:06:26 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 00:06:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:06:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:06:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:06:51 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:06:53 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:06:54 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:06:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:06:55 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:06:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ec2c785fac5ffcee396e609a7abadf074df38ac9625705b0723ae245864028`  
		Last Modified: Sat, 30 Apr 2022 00:12:51 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b9f507571abbf14efa935e4102855354c36573d6d0e0987c74d40b5085409e`  
		Last Modified: Sat, 30 Apr 2022 00:13:04 GMT  
		Size: 87.1 MB (87108678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b714e50265e492fa21c91d4b927d5fcafa6d9ce6b64bb51a89f69c63688c298`  
		Last Modified: Sat, 30 Apr 2022 00:12:51 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71962414ed60d8a6fec935ad5e7b8b6982d7c41382f74e52a30b110f90f57b63`  
		Last Modified: Sat, 30 Apr 2022 00:12:51 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7253c8bbce09ad62f4aedb92fb4ece6de9a8a6b9389b70fd915a2630bc910810
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138780434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b5ae0af269fec9ab843a97f38af5e144f1d13e845da7729991e23afb6c4820`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:38:45 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:48 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 22 Apr 2022 10:38:50 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:53 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 22 Apr 2022 10:38:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:39:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:40:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:40:39 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:40:41 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:40:42 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:40:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:40:47 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:40:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8585fdfb939ad59fe43800e8258791cae1a48fe19fc82bc5b28ee7cea88e25a6`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55c8c0f19134ea3f4e78d7db234e964e8f9b8a28d596ebe4a625594319f9159`  
		Last Modified: Fri, 22 Apr 2022 10:54:35 GMT  
		Size: 92.6 MB (92567188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd4f314b64534547b791600e31d8158b548b2fe4e79ecc4da4285aea8a8741`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47740fd99121c3a1f7c4c4125a8beb046167869d84ae7ed84c2f6ea1ae329ee8`  
		Last Modified: Fri, 22 Apr 2022 10:54:17 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:c5787d0833702e64bbf45c367044853ba5758d107d383b1b6b7ea848d621a038
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127176421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f9a36fde17b045be592b43bab340b70a084c0974ae644be98e846bbd0c0e1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:47:08 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 29 Apr 2022 23:47:08 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 29 Apr 2022 23:47:08 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 29 Apr 2022 23:47:08 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 29 Apr 2022 23:47:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:47:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:47:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:47:43 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:47:43 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:47:44 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:47:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:47:44 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:47:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e342171dfa0498624df901d3be0c1f25da8848b11c6e600397573b26af1dba63`  
		Last Modified: Fri, 29 Apr 2022 23:49:51 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef89698870d6a80a263874ac4e55383d084b81c60e0f13a55ac4525da23f171`  
		Last Modified: Fri, 29 Apr 2022 23:50:04 GMT  
		Size: 89.3 MB (89290156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e7960c465106f14ae6c5868a026fe66b071bb347e80c15b341a1e6ecd1d1da`  
		Last Modified: Fri, 29 Apr 2022 23:49:51 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e880dc457b58bf0de1aa5d2e9ac2d4275ae61a6c9e078e8f73c8be19c971d2d`  
		Last Modified: Fri, 29 Apr 2022 23:49:51 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:60511c90bbb80c49cd53fe1474c06383ecc44336623abb5a7f6deb503f5c1f5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:50f7f199fb81c7cc4a3b367ee8a25f18ce83439a565d094d1d55d25924b195a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128169667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00b1a894e91d2f10ceabfce4375d818c5ca907add9dfbaf8d5954c717baa1d5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:58 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585fa6ed9f9263b79c20959c2e25d32d6523ac4267f3f4b450311c77bbfc30ff`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c4c29c67dbd6b0c81f43ef62d78d3a581ab7f158f68716c49129209ce26140`  
		Last Modified: Fri, 22 Apr 2022 02:56:37 GMT  
		Size: 88.2 MB (88243195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e60110958fb03947e33902acb382866ef3dc70a9dd00ec275c738ccf39c525`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505d73d050133db6e682e04624cbd8a35f21434a6abfe41a42acf3d86f2a8be2`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:77020582792a621d15ffc371263018a82c0b91cd30648890b0d80419cde70788
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125269693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:925020e4d537fc3c6e96410564c712f81a727071d9ba3f8ec15aad8c16b3a86c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:05:39 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 00:05:40 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 00:05:41 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 00:05:42 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 00:05:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:05:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:06:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:06:11 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:06:13 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:06:14 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:06:15 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:06:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8bd198ebd889272c17b8569e98b7355086b25b92a6a0ac147f90847ec6e059`  
		Last Modified: Sat, 30 Apr 2022 00:12:18 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7699d685826cf5dffdf20f2fc57c0a166579bec3cdd437629e016327b23e59f0`  
		Last Modified: Sat, 30 Apr 2022 00:12:31 GMT  
		Size: 87.2 MB (87192939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50b6cf6c6145fd9000b0e2b16648496bce674be857315f0f687487ff42fbf62`  
		Last Modified: Sat, 30 Apr 2022 00:12:18 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6add2ec5f8f0e06b3dc2feeff88c21d87b765df433c9aeb043163bfd6a28cba5`  
		Last Modified: Sat, 30 Apr 2022 00:12:18 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a39a7f33def5844756a0716e2080b6541f8d3be2fb462c15b689cda1bc4e516c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138840617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a07018cb70d1cbe1cfba60fa5297c5e412d15a54ecd11ab0f4b9888774bf1f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:36:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:37 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:39 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:41 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:36:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:38:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:38:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:38:18 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:38:20 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:38:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:38:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:38:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f321db739686e112b38409c1a2f57546c06f622fde87d19ca5f556414f96c55e`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587f01c1085fb65e86c6b1592a8d8fe53e2e5abc56f331aa8d55c6be5756deb4`  
		Last Modified: Fri, 22 Apr 2022 10:53:56 GMT  
		Size: 92.6 MB (92627369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02d948139d8d0e091f50c2b98b6fafa25be9aaf1088eeabb89fa1b80bcaed34`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259eabdc6f306e8fc1339696c7d86f65dfae8a68f5bf05b76f16ceba8f12b2c1`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; s390x

```console
$ docker pull mariadb@sha256:a7a462df82eaa6b734d752d93b54c274114ae6fa8ce9663a21fdbbb52c56e46c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127202634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f512cdfe00a0838da732d7fad44d849905a1fadce49fee63789b9503369ea00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:46:24 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 29 Apr 2022 23:46:24 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 29 Apr 2022 23:46:24 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 29 Apr 2022 23:46:24 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 29 Apr 2022 23:46:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:46:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:46:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:47:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:47:01 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:47:01 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:47:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:47:01 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:47:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a33c0272f0f9687d8e6de127fdd2602c7fc049edf8ec78132a804314c67c83`  
		Last Modified: Fri, 29 Apr 2022 23:49:28 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7311e4fd14e28ed72aab284032ae0fada5fcd8b1d20cd74327710ccd816e3ddf`  
		Last Modified: Fri, 29 Apr 2022 23:49:41 GMT  
		Size: 89.3 MB (89316370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02243ac7ffc45fe985d5d330064524d9513ae889edaf53582204a91f59cd59f8`  
		Last Modified: Fri, 29 Apr 2022 23:49:28 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b820eb4b0315473ae086503e86cd021aa70a4371b7950b1fc1f0e453f06d97`  
		Last Modified: Fri, 29 Apr 2022 23:49:28 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:60511c90bbb80c49cd53fe1474c06383ecc44336623abb5a7f6deb503f5c1f5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:50f7f199fb81c7cc4a3b367ee8a25f18ce83439a565d094d1d55d25924b195a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128169667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00b1a894e91d2f10ceabfce4375d818c5ca907add9dfbaf8d5954c717baa1d5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:58 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585fa6ed9f9263b79c20959c2e25d32d6523ac4267f3f4b450311c77bbfc30ff`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c4c29c67dbd6b0c81f43ef62d78d3a581ab7f158f68716c49129209ce26140`  
		Last Modified: Fri, 22 Apr 2022 02:56:37 GMT  
		Size: 88.2 MB (88243195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e60110958fb03947e33902acb382866ef3dc70a9dd00ec275c738ccf39c525`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505d73d050133db6e682e04624cbd8a35f21434a6abfe41a42acf3d86f2a8be2`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:77020582792a621d15ffc371263018a82c0b91cd30648890b0d80419cde70788
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125269693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:925020e4d537fc3c6e96410564c712f81a727071d9ba3f8ec15aad8c16b3a86c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:05:39 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 00:05:40 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 00:05:41 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 00:05:42 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 00:05:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:05:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:06:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:06:11 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:06:13 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:06:14 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:06:15 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:06:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8bd198ebd889272c17b8569e98b7355086b25b92a6a0ac147f90847ec6e059`  
		Last Modified: Sat, 30 Apr 2022 00:12:18 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7699d685826cf5dffdf20f2fc57c0a166579bec3cdd437629e016327b23e59f0`  
		Last Modified: Sat, 30 Apr 2022 00:12:31 GMT  
		Size: 87.2 MB (87192939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50b6cf6c6145fd9000b0e2b16648496bce674be857315f0f687487ff42fbf62`  
		Last Modified: Sat, 30 Apr 2022 00:12:18 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6add2ec5f8f0e06b3dc2feeff88c21d87b765df433c9aeb043163bfd6a28cba5`  
		Last Modified: Sat, 30 Apr 2022 00:12:18 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a39a7f33def5844756a0716e2080b6541f8d3be2fb462c15b689cda1bc4e516c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138840617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a07018cb70d1cbe1cfba60fa5297c5e412d15a54ecd11ab0f4b9888774bf1f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:36:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:37 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:39 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:41 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:36:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:38:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:38:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:38:18 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:38:20 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:38:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:38:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:38:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f321db739686e112b38409c1a2f57546c06f622fde87d19ca5f556414f96c55e`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587f01c1085fb65e86c6b1592a8d8fe53e2e5abc56f331aa8d55c6be5756deb4`  
		Last Modified: Fri, 22 Apr 2022 10:53:56 GMT  
		Size: 92.6 MB (92627369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02d948139d8d0e091f50c2b98b6fafa25be9aaf1088eeabb89fa1b80bcaed34`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259eabdc6f306e8fc1339696c7d86f65dfae8a68f5bf05b76f16ceba8f12b2c1`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:a7a462df82eaa6b734d752d93b54c274114ae6fa8ce9663a21fdbbb52c56e46c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127202634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f512cdfe00a0838da732d7fad44d849905a1fadce49fee63789b9503369ea00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:46:24 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 29 Apr 2022 23:46:24 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 29 Apr 2022 23:46:24 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 29 Apr 2022 23:46:24 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 29 Apr 2022 23:46:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:46:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:46:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:47:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:47:01 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:47:01 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:47:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:47:01 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:47:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a33c0272f0f9687d8e6de127fdd2602c7fc049edf8ec78132a804314c67c83`  
		Last Modified: Fri, 29 Apr 2022 23:49:28 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7311e4fd14e28ed72aab284032ae0fada5fcd8b1d20cd74327710ccd816e3ddf`  
		Last Modified: Fri, 29 Apr 2022 23:49:41 GMT  
		Size: 89.3 MB (89316370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02243ac7ffc45fe985d5d330064524d9513ae889edaf53582204a91f59cd59f8`  
		Last Modified: Fri, 29 Apr 2022 23:49:28 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b820eb4b0315473ae086503e86cd021aa70a4371b7950b1fc1f0e453f06d97`  
		Last Modified: Fri, 29 Apr 2022 23:49:28 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.7`

```console
$ docker pull mariadb@sha256:60511c90bbb80c49cd53fe1474c06383ecc44336623abb5a7f6deb503f5c1f5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.7` - linux; amd64

```console
$ docker pull mariadb@sha256:50f7f199fb81c7cc4a3b367ee8a25f18ce83439a565d094d1d55d25924b195a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128169667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00b1a894e91d2f10ceabfce4375d818c5ca907add9dfbaf8d5954c717baa1d5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:58 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585fa6ed9f9263b79c20959c2e25d32d6523ac4267f3f4b450311c77bbfc30ff`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c4c29c67dbd6b0c81f43ef62d78d3a581ab7f158f68716c49129209ce26140`  
		Last Modified: Fri, 22 Apr 2022 02:56:37 GMT  
		Size: 88.2 MB (88243195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e60110958fb03947e33902acb382866ef3dc70a9dd00ec275c738ccf39c525`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505d73d050133db6e682e04624cbd8a35f21434a6abfe41a42acf3d86f2a8be2`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:77020582792a621d15ffc371263018a82c0b91cd30648890b0d80419cde70788
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125269693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:925020e4d537fc3c6e96410564c712f81a727071d9ba3f8ec15aad8c16b3a86c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:05:39 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 00:05:40 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 00:05:41 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 00:05:42 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 00:05:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:05:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:06:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:06:11 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:06:13 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:06:14 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:06:15 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:06:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8bd198ebd889272c17b8569e98b7355086b25b92a6a0ac147f90847ec6e059`  
		Last Modified: Sat, 30 Apr 2022 00:12:18 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7699d685826cf5dffdf20f2fc57c0a166579bec3cdd437629e016327b23e59f0`  
		Last Modified: Sat, 30 Apr 2022 00:12:31 GMT  
		Size: 87.2 MB (87192939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50b6cf6c6145fd9000b0e2b16648496bce674be857315f0f687487ff42fbf62`  
		Last Modified: Sat, 30 Apr 2022 00:12:18 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6add2ec5f8f0e06b3dc2feeff88c21d87b765df433c9aeb043163bfd6a28cba5`  
		Last Modified: Sat, 30 Apr 2022 00:12:18 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a39a7f33def5844756a0716e2080b6541f8d3be2fb462c15b689cda1bc4e516c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138840617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a07018cb70d1cbe1cfba60fa5297c5e412d15a54ecd11ab0f4b9888774bf1f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:36:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:37 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:39 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:41 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:36:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:38:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:38:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:38:18 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:38:20 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:38:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:38:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:38:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f321db739686e112b38409c1a2f57546c06f622fde87d19ca5f556414f96c55e`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587f01c1085fb65e86c6b1592a8d8fe53e2e5abc56f331aa8d55c6be5756deb4`  
		Last Modified: Fri, 22 Apr 2022 10:53:56 GMT  
		Size: 92.6 MB (92627369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02d948139d8d0e091f50c2b98b6fafa25be9aaf1088eeabb89fa1b80bcaed34`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259eabdc6f306e8fc1339696c7d86f65dfae8a68f5bf05b76f16ceba8f12b2c1`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; s390x

```console
$ docker pull mariadb@sha256:a7a462df82eaa6b734d752d93b54c274114ae6fa8ce9663a21fdbbb52c56e46c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127202634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f512cdfe00a0838da732d7fad44d849905a1fadce49fee63789b9503369ea00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:46:24 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 29 Apr 2022 23:46:24 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 29 Apr 2022 23:46:24 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 29 Apr 2022 23:46:24 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 29 Apr 2022 23:46:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:46:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:46:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:47:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:47:01 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:47:01 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:47:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:47:01 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:47:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a33c0272f0f9687d8e6de127fdd2602c7fc049edf8ec78132a804314c67c83`  
		Last Modified: Fri, 29 Apr 2022 23:49:28 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7311e4fd14e28ed72aab284032ae0fada5fcd8b1d20cd74327710ccd816e3ddf`  
		Last Modified: Fri, 29 Apr 2022 23:49:41 GMT  
		Size: 89.3 MB (89316370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02243ac7ffc45fe985d5d330064524d9513ae889edaf53582204a91f59cd59f8`  
		Last Modified: Fri, 29 Apr 2022 23:49:28 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b820eb4b0315473ae086503e86cd021aa70a4371b7950b1fc1f0e453f06d97`  
		Last Modified: Fri, 29 Apr 2022 23:49:28 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.7-focal`

```console
$ docker pull mariadb@sha256:60511c90bbb80c49cd53fe1474c06383ecc44336623abb5a7f6deb503f5c1f5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:50f7f199fb81c7cc4a3b367ee8a25f18ce83439a565d094d1d55d25924b195a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128169667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00b1a894e91d2f10ceabfce4375d818c5ca907add9dfbaf8d5954c717baa1d5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 02:51:35 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 02:51:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:58 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:58 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585fa6ed9f9263b79c20959c2e25d32d6523ac4267f3f4b450311c77bbfc30ff`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c4c29c67dbd6b0c81f43ef62d78d3a581ab7f158f68716c49129209ce26140`  
		Last Modified: Fri, 22 Apr 2022 02:56:37 GMT  
		Size: 88.2 MB (88243195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e60110958fb03947e33902acb382866ef3dc70a9dd00ec275c738ccf39c525`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505d73d050133db6e682e04624cbd8a35f21434a6abfe41a42acf3d86f2a8be2`  
		Last Modified: Fri, 22 Apr 2022 02:56:24 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:77020582792a621d15ffc371263018a82c0b91cd30648890b0d80419cde70788
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125269693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:925020e4d537fc3c6e96410564c712f81a727071d9ba3f8ec15aad8c16b3a86c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:05:39 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 00:05:40 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 00:05:41 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 00:05:42 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 00:05:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:05:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:06:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:06:11 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:06:13 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:06:14 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:06:15 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:06:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8bd198ebd889272c17b8569e98b7355086b25b92a6a0ac147f90847ec6e059`  
		Last Modified: Sat, 30 Apr 2022 00:12:18 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7699d685826cf5dffdf20f2fc57c0a166579bec3cdd437629e016327b23e59f0`  
		Last Modified: Sat, 30 Apr 2022 00:12:31 GMT  
		Size: 87.2 MB (87192939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50b6cf6c6145fd9000b0e2b16648496bce674be857315f0f687487ff42fbf62`  
		Last Modified: Sat, 30 Apr 2022 00:12:18 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6add2ec5f8f0e06b3dc2feeff88c21d87b765df433c9aeb043163bfd6a28cba5`  
		Last Modified: Sat, 30 Apr 2022 00:12:18 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a39a7f33def5844756a0716e2080b6541f8d3be2fb462c15b689cda1bc4e516c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138840617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a07018cb70d1cbe1cfba60fa5297c5e412d15a54ecd11ab0f4b9888774bf1f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:36:35 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:37 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 22 Apr 2022 10:36:39 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:41 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 22 Apr 2022 10:36:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:36:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:38:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:38:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:38:18 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:38:20 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:38:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:38:25 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:38:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f321db739686e112b38409c1a2f57546c06f622fde87d19ca5f556414f96c55e`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587f01c1085fb65e86c6b1592a8d8fe53e2e5abc56f331aa8d55c6be5756deb4`  
		Last Modified: Fri, 22 Apr 2022 10:53:56 GMT  
		Size: 92.6 MB (92627369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02d948139d8d0e091f50c2b98b6fafa25be9aaf1088eeabb89fa1b80bcaed34`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259eabdc6f306e8fc1339696c7d86f65dfae8a68f5bf05b76f16ceba8f12b2c1`  
		Last Modified: Fri, 22 Apr 2022 10:53:38 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:a7a462df82eaa6b734d752d93b54c274114ae6fa8ce9663a21fdbbb52c56e46c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127202634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f512cdfe00a0838da732d7fad44d849905a1fadce49fee63789b9503369ea00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:46:24 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 29 Apr 2022 23:46:24 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 29 Apr 2022 23:46:24 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 29 Apr 2022 23:46:24 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 29 Apr 2022 23:46:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:46:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:46:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:47:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:47:01 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:47:01 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:47:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:47:01 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:47:01 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a33c0272f0f9687d8e6de127fdd2602c7fc049edf8ec78132a804314c67c83`  
		Last Modified: Fri, 29 Apr 2022 23:49:28 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7311e4fd14e28ed72aab284032ae0fada5fcd8b1d20cd74327710ccd816e3ddf`  
		Last Modified: Fri, 29 Apr 2022 23:49:41 GMT  
		Size: 89.3 MB (89316370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02243ac7ffc45fe985d5d330064524d9513ae889edaf53582204a91f59cd59f8`  
		Last Modified: Fri, 29 Apr 2022 23:49:28 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b820eb4b0315473ae086503e86cd021aa70a4371b7950b1fc1f0e453f06d97`  
		Last Modified: Fri, 29 Apr 2022 23:49:28 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7`

```console
$ docker pull mariadb@sha256:d28e381c205c895eb44e7e1843884bf31018a94e18a39fb6f37c769c045a4e8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:04a2c991ca9282b610ca4a5271ffc617e52d5d9c9cbe324771f827474e4d1dfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f545466a3bd9ba56de74c6aff0b326bfd31b45b23aea7982a3fe54e94c6783bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:59 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:00 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:01 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:02 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:05:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:05:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:05:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:05:29 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:05:30 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:05:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8552be18be3da4845285400b3cc0ef56395f23252feec66ec1b7d9c839caf6f3`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838f8e410529d235d60451deb629c2ad0048c54b691c81f8485e1cca8eec4846`  
		Last Modified: Sat, 30 Apr 2022 00:11:44 GMT  
		Size: 87.6 MB (87644865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6eca4b9a032371bbf080c453df543d01bdfce97ea7c11583ea86854f79dd92`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f2797f4c63be734eab71b5da1025d334620dd0a6978f80cb11022c88ccfcec`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; s390x

```console
$ docker pull mariadb@sha256:834212faeb75a2a43648a37982041f285f537b5cb1e3b0d4698a8df3732007cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127701635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5e6a0fd99b6b261fb89f90ebda2e325da3051f0d56a4895f553c69af9c69686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:45:41 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:41 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:42 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:45:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:46:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:46:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:46:15 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:46:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70732cc91f318d007de766e94265f7a0539440482fedce98b4ed140173b77f1c`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44483aab52b201a5daba428dbb324742d6ece06777315a61021f24fc22a740cd`  
		Last Modified: Fri, 29 Apr 2022 23:49:09 GMT  
		Size: 89.8 MB (89815369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d5f62ecf4e209a33d158a01c03b82ad089be13910b212570c95d41706666df`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d60e7434e17b71d925c7fe28efc5dfee00d94111b7a8225788104b4c04262ec`  
		Last Modified: Fri, 29 Apr 2022 23:48:57 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7-focal`

```console
$ docker pull mariadb@sha256:d28e381c205c895eb44e7e1843884bf31018a94e18a39fb6f37c769c045a4e8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:04a2c991ca9282b610ca4a5271ffc617e52d5d9c9cbe324771f827474e4d1dfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f545466a3bd9ba56de74c6aff0b326bfd31b45b23aea7982a3fe54e94c6783bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:59 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:00 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:01 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:02 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:05:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:05:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:05:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:05:29 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:05:30 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:05:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8552be18be3da4845285400b3cc0ef56395f23252feec66ec1b7d9c839caf6f3`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838f8e410529d235d60451deb629c2ad0048c54b691c81f8485e1cca8eec4846`  
		Last Modified: Sat, 30 Apr 2022 00:11:44 GMT  
		Size: 87.6 MB (87644865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6eca4b9a032371bbf080c453df543d01bdfce97ea7c11583ea86854f79dd92`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f2797f4c63be734eab71b5da1025d334620dd0a6978f80cb11022c88ccfcec`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:834212faeb75a2a43648a37982041f285f537b5cb1e3b0d4698a8df3732007cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127701635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5e6a0fd99b6b261fb89f90ebda2e325da3051f0d56a4895f553c69af9c69686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:45:41 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:41 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:42 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:45:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:46:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:46:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:46:15 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:46:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70732cc91f318d007de766e94265f7a0539440482fedce98b4ed140173b77f1c`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44483aab52b201a5daba428dbb324742d6ece06777315a61021f24fc22a740cd`  
		Last Modified: Fri, 29 Apr 2022 23:49:09 GMT  
		Size: 89.8 MB (89815369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d5f62ecf4e209a33d158a01c03b82ad089be13910b212570c95d41706666df`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d60e7434e17b71d925c7fe28efc5dfee00d94111b7a8225788104b4c04262ec`  
		Last Modified: Fri, 29 Apr 2022 23:48:57 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.3`

```console
$ docker pull mariadb@sha256:d28e381c205c895eb44e7e1843884bf31018a94e18a39fb6f37c769c045a4e8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.3` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:04a2c991ca9282b610ca4a5271ffc617e52d5d9c9cbe324771f827474e4d1dfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f545466a3bd9ba56de74c6aff0b326bfd31b45b23aea7982a3fe54e94c6783bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:59 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:00 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:01 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:02 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:05:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:05:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:05:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:05:29 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:05:30 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:05:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8552be18be3da4845285400b3cc0ef56395f23252feec66ec1b7d9c839caf6f3`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838f8e410529d235d60451deb629c2ad0048c54b691c81f8485e1cca8eec4846`  
		Last Modified: Sat, 30 Apr 2022 00:11:44 GMT  
		Size: 87.6 MB (87644865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6eca4b9a032371bbf080c453df543d01bdfce97ea7c11583ea86854f79dd92`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f2797f4c63be734eab71b5da1025d334620dd0a6978f80cb11022c88ccfcec`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3` - linux; s390x

```console
$ docker pull mariadb@sha256:834212faeb75a2a43648a37982041f285f537b5cb1e3b0d4698a8df3732007cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127701635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5e6a0fd99b6b261fb89f90ebda2e325da3051f0d56a4895f553c69af9c69686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:45:41 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:41 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:42 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:45:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:46:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:46:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:46:15 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:46:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70732cc91f318d007de766e94265f7a0539440482fedce98b4ed140173b77f1c`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44483aab52b201a5daba428dbb324742d6ece06777315a61021f24fc22a740cd`  
		Last Modified: Fri, 29 Apr 2022 23:49:09 GMT  
		Size: 89.8 MB (89815369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d5f62ecf4e209a33d158a01c03b82ad089be13910b212570c95d41706666df`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d60e7434e17b71d925c7fe28efc5dfee00d94111b7a8225788104b4c04262ec`  
		Last Modified: Fri, 29 Apr 2022 23:48:57 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.3-focal`

```console
$ docker pull mariadb@sha256:d28e381c205c895eb44e7e1843884bf31018a94e18a39fb6f37c769c045a4e8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:04a2c991ca9282b610ca4a5271ffc617e52d5d9c9cbe324771f827474e4d1dfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f545466a3bd9ba56de74c6aff0b326bfd31b45b23aea7982a3fe54e94c6783bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:59 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:00 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:01 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:02 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:05:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:05:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:05:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:05:29 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:05:30 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:05:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8552be18be3da4845285400b3cc0ef56395f23252feec66ec1b7d9c839caf6f3`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838f8e410529d235d60451deb629c2ad0048c54b691c81f8485e1cca8eec4846`  
		Last Modified: Sat, 30 Apr 2022 00:11:44 GMT  
		Size: 87.6 MB (87644865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6eca4b9a032371bbf080c453df543d01bdfce97ea7c11583ea86854f79dd92`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f2797f4c63be734eab71b5da1025d334620dd0a6978f80cb11022c88ccfcec`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:834212faeb75a2a43648a37982041f285f537b5cb1e3b0d4698a8df3732007cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127701635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5e6a0fd99b6b261fb89f90ebda2e325da3051f0d56a4895f553c69af9c69686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:45:41 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:41 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:42 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:45:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:46:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:46:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:46:15 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:46:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70732cc91f318d007de766e94265f7a0539440482fedce98b4ed140173b77f1c`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44483aab52b201a5daba428dbb324742d6ece06777315a61021f24fc22a740cd`  
		Last Modified: Fri, 29 Apr 2022 23:49:09 GMT  
		Size: 89.8 MB (89815369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d5f62ecf4e209a33d158a01c03b82ad089be13910b212570c95d41706666df`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d60e7434e17b71d925c7fe28efc5dfee00d94111b7a8225788104b4c04262ec`  
		Last Modified: Fri, 29 Apr 2022 23:48:57 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8-rc`

```console
$ docker pull mariadb@sha256:f649c5ca676ac6cdefc78f2b657efd2cee83031abd0cdd896d1f7458dc35bede
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:6207f31973a665b4d1c9ba7ea7ac726adad41a661a549561fc671b44148ce330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9732c0915d292a0e4f73669df378c84618d6492d687d02bd6217d4d3dff650`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:50:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:03 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ba526ebec155d55cbb43daf63138efab1b47b098a037e64dd6acfcee49c6fd`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c3c04a1f7b4ecf07d5a5de05f17a2d0290974d190181a5f6a2533bde7931cf`  
		Last Modified: Fri, 22 Apr 2022 02:55:27 GMT  
		Size: 88.7 MB (88651923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8147174b3e651ed73d19ba9e151df9da5da3d253719e13ff39d98fb4f37b05b0`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e24d2b3f05313227b1155b461f451eac48ce5ae7c60d77d5cf22ed1c4bb2df9`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:a86c75410340ea8b97b2fd88ffce64af01629013c2a1097d32b2989e7b6dbf49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125650366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65fce899e90716f18477e435b254cb2946e575afa0f8b0226e7eec4aac5b61d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:13 GMT
ARG MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:04:14 GMT
ENV MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:04:15 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:04:16 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:04:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:04:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:04:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:04:43 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:04:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:04:46 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:04:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:04:47 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:04:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce763ae3d19421a5238af59de35db56c45d38497925298ada8ea527ce14c8b51`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d496894956c169d962cd64bea30da9bdb9fb883514a3d7876612731ffb36f24`  
		Last Modified: Sat, 30 Apr 2022 00:11:11 GMT  
		Size: 87.6 MB (87573611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ff3d92cd0ad9f07598a46b25670aa02fb6aa29c04c767621f2446783562b96`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65305c7f16fd5bc46bb41b6398226ee20a00ee96efc7e5cb6bf90cd754cf016`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:89a7053031696f7d4e7553d8cab343f90e2a53df5e60091b29ae56fbe967e17a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139619033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5e81f620d456e1b33bde7bf9cb5040219e3345e305dd9e8a0d53004c7cd5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:31:50 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:51 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:54 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:55 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:32:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:33:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:33:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:33:52 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:33:53 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:33:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:34:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad9f52d7b4e854a5040fae3388098651787b071fe78342b69192cd1686a19ef`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b681bd97d5fa7c912ef840826913da6df694154fb9147f41dd223cb415316c`  
		Last Modified: Fri, 22 Apr 2022 10:52:21 GMT  
		Size: 93.4 MB (93405782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baeda5a29e96eab044146b1ea14602da3bfcf2f2285cd12f4a43f2f6845c3d8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269ad16de2005b90fdfbaa56368cb57a565049c8b9e4980dd91fc7d52543557`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:967adf27f0817cf0b01da306254d88f2c82a365dd475bff204bf7d03ddad9bef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127666379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd11eeb57e6641f58e6801a1162b6d88e2fbb84384c7356ff867c41cc00ddbde`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:44:57 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 29 Apr 2022 23:44:57 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 29 Apr 2022 23:44:57 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 29 Apr 2022 23:44:57 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 29 Apr 2022 23:44:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:44:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:45:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:45:28 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:45:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:45:28 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:45:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:45:29 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:45:29 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb7b68a9ad671742bf83a5263aef5d9bee045aa15d8045dd5df2767a26f4b3e`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d94e61c904d2fe0a0d5beeee5a698a77e6757337449a9a6c437fb7922b81688`  
		Last Modified: Fri, 29 Apr 2022 23:48:45 GMT  
		Size: 89.8 MB (89780108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3c085a38d4321480df7612fc014d39a04af2503c4ad6370c63252200e19892`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22135004b6f478b57d495c68991e235e3cdd13193621e68775335df7034acdb0`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 6.8 KB (6776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8-rc-focal`

```console
$ docker pull mariadb@sha256:f649c5ca676ac6cdefc78f2b657efd2cee83031abd0cdd896d1f7458dc35bede
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-rc-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:6207f31973a665b4d1c9ba7ea7ac726adad41a661a549561fc671b44148ce330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9732c0915d292a0e4f73669df378c84618d6492d687d02bd6217d4d3dff650`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:50:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:03 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ba526ebec155d55cbb43daf63138efab1b47b098a037e64dd6acfcee49c6fd`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c3c04a1f7b4ecf07d5a5de05f17a2d0290974d190181a5f6a2533bde7931cf`  
		Last Modified: Fri, 22 Apr 2022 02:55:27 GMT  
		Size: 88.7 MB (88651923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8147174b3e651ed73d19ba9e151df9da5da3d253719e13ff39d98fb4f37b05b0`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e24d2b3f05313227b1155b461f451eac48ce5ae7c60d77d5cf22ed1c4bb2df9`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:a86c75410340ea8b97b2fd88ffce64af01629013c2a1097d32b2989e7b6dbf49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125650366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65fce899e90716f18477e435b254cb2946e575afa0f8b0226e7eec4aac5b61d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:13 GMT
ARG MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:04:14 GMT
ENV MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:04:15 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:04:16 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:04:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:04:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:04:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:04:43 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:04:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:04:46 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:04:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:04:47 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:04:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce763ae3d19421a5238af59de35db56c45d38497925298ada8ea527ce14c8b51`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d496894956c169d962cd64bea30da9bdb9fb883514a3d7876612731ffb36f24`  
		Last Modified: Sat, 30 Apr 2022 00:11:11 GMT  
		Size: 87.6 MB (87573611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ff3d92cd0ad9f07598a46b25670aa02fb6aa29c04c767621f2446783562b96`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65305c7f16fd5bc46bb41b6398226ee20a00ee96efc7e5cb6bf90cd754cf016`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:89a7053031696f7d4e7553d8cab343f90e2a53df5e60091b29ae56fbe967e17a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139619033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5e81f620d456e1b33bde7bf9cb5040219e3345e305dd9e8a0d53004c7cd5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:31:50 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:51 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:54 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:55 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:32:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:33:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:33:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:33:52 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:33:53 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:33:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:34:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad9f52d7b4e854a5040fae3388098651787b071fe78342b69192cd1686a19ef`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b681bd97d5fa7c912ef840826913da6df694154fb9147f41dd223cb415316c`  
		Last Modified: Fri, 22 Apr 2022 10:52:21 GMT  
		Size: 93.4 MB (93405782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baeda5a29e96eab044146b1ea14602da3bfcf2f2285cd12f4a43f2f6845c3d8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269ad16de2005b90fdfbaa56368cb57a565049c8b9e4980dd91fc7d52543557`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:967adf27f0817cf0b01da306254d88f2c82a365dd475bff204bf7d03ddad9bef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127666379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd11eeb57e6641f58e6801a1162b6d88e2fbb84384c7356ff867c41cc00ddbde`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:44:57 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 29 Apr 2022 23:44:57 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 29 Apr 2022 23:44:57 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 29 Apr 2022 23:44:57 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 29 Apr 2022 23:44:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:44:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:45:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:45:28 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:45:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:45:28 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:45:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:45:29 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:45:29 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb7b68a9ad671742bf83a5263aef5d9bee045aa15d8045dd5df2767a26f4b3e`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d94e61c904d2fe0a0d5beeee5a698a77e6757337449a9a6c437fb7922b81688`  
		Last Modified: Fri, 29 Apr 2022 23:48:45 GMT  
		Size: 89.8 MB (89780108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3c085a38d4321480df7612fc014d39a04af2503c4ad6370c63252200e19892`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22135004b6f478b57d495c68991e235e3cdd13193621e68775335df7034acdb0`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 6.8 KB (6776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.2-rc`

```console
$ docker pull mariadb@sha256:f649c5ca676ac6cdefc78f2b657efd2cee83031abd0cdd896d1f7458dc35bede
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8.2-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:6207f31973a665b4d1c9ba7ea7ac726adad41a661a549561fc671b44148ce330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9732c0915d292a0e4f73669df378c84618d6492d687d02bd6217d4d3dff650`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:50:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:03 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ba526ebec155d55cbb43daf63138efab1b47b098a037e64dd6acfcee49c6fd`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c3c04a1f7b4ecf07d5a5de05f17a2d0290974d190181a5f6a2533bde7931cf`  
		Last Modified: Fri, 22 Apr 2022 02:55:27 GMT  
		Size: 88.7 MB (88651923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8147174b3e651ed73d19ba9e151df9da5da3d253719e13ff39d98fb4f37b05b0`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e24d2b3f05313227b1155b461f451eac48ce5ae7c60d77d5cf22ed1c4bb2df9`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:a86c75410340ea8b97b2fd88ffce64af01629013c2a1097d32b2989e7b6dbf49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125650366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65fce899e90716f18477e435b254cb2946e575afa0f8b0226e7eec4aac5b61d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:13 GMT
ARG MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:04:14 GMT
ENV MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:04:15 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:04:16 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:04:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:04:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:04:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:04:43 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:04:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:04:46 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:04:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:04:47 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:04:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce763ae3d19421a5238af59de35db56c45d38497925298ada8ea527ce14c8b51`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d496894956c169d962cd64bea30da9bdb9fb883514a3d7876612731ffb36f24`  
		Last Modified: Sat, 30 Apr 2022 00:11:11 GMT  
		Size: 87.6 MB (87573611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ff3d92cd0ad9f07598a46b25670aa02fb6aa29c04c767621f2446783562b96`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65305c7f16fd5bc46bb41b6398226ee20a00ee96efc7e5cb6bf90cd754cf016`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:89a7053031696f7d4e7553d8cab343f90e2a53df5e60091b29ae56fbe967e17a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139619033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5e81f620d456e1b33bde7bf9cb5040219e3345e305dd9e8a0d53004c7cd5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:31:50 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:51 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:54 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:55 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:32:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:33:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:33:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:33:52 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:33:53 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:33:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:34:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad9f52d7b4e854a5040fae3388098651787b071fe78342b69192cd1686a19ef`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b681bd97d5fa7c912ef840826913da6df694154fb9147f41dd223cb415316c`  
		Last Modified: Fri, 22 Apr 2022 10:52:21 GMT  
		Size: 93.4 MB (93405782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baeda5a29e96eab044146b1ea14602da3bfcf2f2285cd12f4a43f2f6845c3d8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269ad16de2005b90fdfbaa56368cb57a565049c8b9e4980dd91fc7d52543557`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:967adf27f0817cf0b01da306254d88f2c82a365dd475bff204bf7d03ddad9bef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127666379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd11eeb57e6641f58e6801a1162b6d88e2fbb84384c7356ff867c41cc00ddbde`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:44:57 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 29 Apr 2022 23:44:57 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 29 Apr 2022 23:44:57 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 29 Apr 2022 23:44:57 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 29 Apr 2022 23:44:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:44:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:45:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:45:28 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:45:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:45:28 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:45:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:45:29 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:45:29 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb7b68a9ad671742bf83a5263aef5d9bee045aa15d8045dd5df2767a26f4b3e`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d94e61c904d2fe0a0d5beeee5a698a77e6757337449a9a6c437fb7922b81688`  
		Last Modified: Fri, 29 Apr 2022 23:48:45 GMT  
		Size: 89.8 MB (89780108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3c085a38d4321480df7612fc014d39a04af2503c4ad6370c63252200e19892`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22135004b6f478b57d495c68991e235e3cdd13193621e68775335df7034acdb0`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 6.8 KB (6776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.2-rc-focal`

```console
$ docker pull mariadb@sha256:f649c5ca676ac6cdefc78f2b657efd2cee83031abd0cdd896d1f7458dc35bede
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8.2-rc-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:6207f31973a665b4d1c9ba7ea7ac726adad41a661a549561fc671b44148ce330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9732c0915d292a0e4f73669df378c84618d6492d687d02bd6217d4d3dff650`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 02:50:32 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:32 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 02:50:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:50:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:03 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ba526ebec155d55cbb43daf63138efab1b47b098a037e64dd6acfcee49c6fd`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c3c04a1f7b4ecf07d5a5de05f17a2d0290974d190181a5f6a2533bde7931cf`  
		Last Modified: Fri, 22 Apr 2022 02:55:27 GMT  
		Size: 88.7 MB (88651923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8147174b3e651ed73d19ba9e151df9da5da3d253719e13ff39d98fb4f37b05b0`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e24d2b3f05313227b1155b461f451eac48ce5ae7c60d77d5cf22ed1c4bb2df9`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:a86c75410340ea8b97b2fd88ffce64af01629013c2a1097d32b2989e7b6dbf49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125650366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65fce899e90716f18477e435b254cb2946e575afa0f8b0226e7eec4aac5b61d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:13 GMT
ARG MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:04:14 GMT
ENV MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:04:15 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:04:16 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:04:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:04:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:04:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:04:43 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:04:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:04:46 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:04:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:04:47 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:04:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce763ae3d19421a5238af59de35db56c45d38497925298ada8ea527ce14c8b51`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d496894956c169d962cd64bea30da9bdb9fb883514a3d7876612731ffb36f24`  
		Last Modified: Sat, 30 Apr 2022 00:11:11 GMT  
		Size: 87.6 MB (87573611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ff3d92cd0ad9f07598a46b25670aa02fb6aa29c04c767621f2446783562b96`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65305c7f16fd5bc46bb41b6398226ee20a00ee96efc7e5cb6bf90cd754cf016`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:89a7053031696f7d4e7553d8cab343f90e2a53df5e60091b29ae56fbe967e17a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139619033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c5e81f620d456e1b33bde7bf9cb5040219e3345e305dd9e8a0d53004c7cd5bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:31:50 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:51 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 22 Apr 2022 10:31:54 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:55 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 22 Apr 2022 10:31:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:32:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:33:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:33:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:33:52 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:33:53 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:33:57 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:34:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad9f52d7b4e854a5040fae3388098651787b071fe78342b69192cd1686a19ef`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b681bd97d5fa7c912ef840826913da6df694154fb9147f41dd223cb415316c`  
		Last Modified: Fri, 22 Apr 2022 10:52:21 GMT  
		Size: 93.4 MB (93405782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baeda5a29e96eab044146b1ea14602da3bfcf2f2285cd12f4a43f2f6845c3d8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b269ad16de2005b90fdfbaa56368cb57a565049c8b9e4980dd91fc7d52543557`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:967adf27f0817cf0b01da306254d88f2c82a365dd475bff204bf7d03ddad9bef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127666379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd11eeb57e6641f58e6801a1162b6d88e2fbb84384c7356ff867c41cc00ddbde`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:44:57 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 29 Apr 2022 23:44:57 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 29 Apr 2022 23:44:57 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 29 Apr 2022 23:44:57 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 29 Apr 2022 23:44:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:44:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:45:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:45:28 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:45:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:45:28 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:45:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:45:29 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:45:29 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb7b68a9ad671742bf83a5263aef5d9bee045aa15d8045dd5df2767a26f4b3e`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d94e61c904d2fe0a0d5beeee5a698a77e6757337449a9a6c437fb7922b81688`  
		Last Modified: Fri, 29 Apr 2022 23:48:45 GMT  
		Size: 89.8 MB (89780108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3c085a38d4321480df7612fc014d39a04af2503c4ad6370c63252200e19892`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22135004b6f478b57d495c68991e235e3cdd13193621e68775335df7034acdb0`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 6.8 KB (6776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:d28e381c205c895eb44e7e1843884bf31018a94e18a39fb6f37c769c045a4e8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:04a2c991ca9282b610ca4a5271ffc617e52d5d9c9cbe324771f827474e4d1dfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f545466a3bd9ba56de74c6aff0b326bfd31b45b23aea7982a3fe54e94c6783bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:59 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:00 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:01 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:02 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:05:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:05:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:05:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:05:29 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:05:30 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:05:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8552be18be3da4845285400b3cc0ef56395f23252feec66ec1b7d9c839caf6f3`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838f8e410529d235d60451deb629c2ad0048c54b691c81f8485e1cca8eec4846`  
		Last Modified: Sat, 30 Apr 2022 00:11:44 GMT  
		Size: 87.6 MB (87644865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6eca4b9a032371bbf080c453df543d01bdfce97ea7c11583ea86854f79dd92`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f2797f4c63be734eab71b5da1025d334620dd0a6978f80cb11022c88ccfcec`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; s390x

```console
$ docker pull mariadb@sha256:834212faeb75a2a43648a37982041f285f537b5cb1e3b0d4698a8df3732007cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127701635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5e6a0fd99b6b261fb89f90ebda2e325da3051f0d56a4895f553c69af9c69686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:45:41 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:41 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:42 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:45:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:46:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:46:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:46:15 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:46:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70732cc91f318d007de766e94265f7a0539440482fedce98b4ed140173b77f1c`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44483aab52b201a5daba428dbb324742d6ece06777315a61021f24fc22a740cd`  
		Last Modified: Fri, 29 Apr 2022 23:49:09 GMT  
		Size: 89.8 MB (89815369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d5f62ecf4e209a33d158a01c03b82ad089be13910b212570c95d41706666df`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d60e7434e17b71d925c7fe28efc5dfee00d94111b7a8225788104b4c04262ec`  
		Last Modified: Fri, 29 Apr 2022 23:48:57 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:d28e381c205c895eb44e7e1843884bf31018a94e18a39fb6f37c769c045a4e8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:c5cefb5639e0f9360734406cb0f8b7a119c29083705059a1c4509cf31b6f1dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1ace59b072bf4850281c7a3262a76f762ef97d774a38f5a5cddda9514dd811`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:49:58 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 02:50:11 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 02:50:23 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 02:50:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 02:50:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:50:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 02:50:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 02:51:07 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 02:51:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 02:51:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 02:51:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 02:51:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 02:51:29 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 02:51:30 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 02:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 02:51:30 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 02:51:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c31fd2b56f53ff5ba5ad5d21b9b28fa703a2f00ba36f7eb46f2d33b5990991`  
		Last Modified: Fri, 22 Apr 2022 02:55:18 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283b74a4775214476da7b0f4c35eca591deb95c8bc63302ab6f9e683bdf27c64`  
		Last Modified: Fri, 22 Apr 2022 02:55:17 GMT  
		Size: 5.5 MB (5488530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9826fce863ca3c5d0aba036e072e4d8e223bed29a3a7c69e257e9e8041343`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 3.6 MB (3584958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c55a00590e4f6368ec1f193c5ed403478245d2a7a10d09e41ed70caee085a0`  
		Last Modified: Fri, 22 Apr 2022 02:55:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc07b7e87bb4284714b6d047b39b0b5f4e21fec8aae18c882caaf0224049425c`  
		Last Modified: Fri, 22 Apr 2022 02:55:16 GMT  
		Size: 2.3 MB (2272009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cf1a0d04d7cbb85b720ddc123637c146ca65878e7c24c71b738588d5ab9b1`  
		Last Modified: Fri, 22 Apr 2022 02:55:13 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8f6c64a8fa57732c8eb3db48d751c40e0795aa5ca42f05d27c2e9ab31075bc`  
		Last Modified: Fri, 22 Apr 2022 02:55:43 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9817bd990fc72a53340f7dfdda9343811b5a6f4cbc914369c092d3994a044a`  
		Last Modified: Fri, 22 Apr 2022 02:55:56 GMT  
		Size: 88.7 MB (88741666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14828b87067569c6589bb8a62987321b440e088af17c5e8a0163841f3bba2e26`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233be9bdce04aeae1b3a83158f299fccc9e8ef3535617d5ea40ebe5b9dcac8c6`  
		Last Modified: Fri, 22 Apr 2022 02:55:42 GMT  
		Size: 6.8 KB (6774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:04a2c991ca9282b610ca4a5271ffc617e52d5d9c9cbe324771f827474e4d1dfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125721625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f545466a3bd9ba56de74c6aff0b326bfd31b45b23aea7982a3fe54e94c6783bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:03:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:45 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:04:00 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:04:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:04:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:04:10 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:04:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:04:59 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:00 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:05:01 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:02 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 00:05:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:05:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:05:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:05:26 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:05:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:05:29 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:05:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:05:30 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:05:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d0da437931580c9d7f118c259624e1c3ec8e81acb2acf5740d945e511ba78`  
		Last Modified: Sat, 30 Apr 2022 00:11:03 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc35c765a7328bd99273ee471b6b108980755023d4bcb1927fa7717942a9d318`  
		Last Modified: Sat, 30 Apr 2022 00:11:02 GMT  
		Size: 5.3 MB (5320183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88bae007bd9c42610e465ab436d60b2457b10b735a1bc8e5daba38f548c026`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 3.4 MB (3369899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7734d2f7be989dfe94fb891565830b8101d8e9bdbcbce8e5a7e1b1932eb3ac3c`  
		Last Modified: Sat, 30 Apr 2022 00:11:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24600bac48ce2157027e68df9e26a81754edc6f7e099c33c0a89de879dba5d9`  
		Last Modified: Sat, 30 Apr 2022 00:11:01 GMT  
		Size: 2.2 MB (2202385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da05700210f681c47e021b8f3ce45f244f696854cfd656f0cd46e59cb8ca9b7d`  
		Last Modified: Sat, 30 Apr 2022 00:10:58 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8552be18be3da4845285400b3cc0ef56395f23252feec66ec1b7d9c839caf6f3`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838f8e410529d235d60451deb629c2ad0048c54b691c81f8485e1cca8eec4846`  
		Last Modified: Sat, 30 Apr 2022 00:11:44 GMT  
		Size: 87.6 MB (87644865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6eca4b9a032371bbf080c453df543d01bdfce97ea7c11583ea86854f79dd92`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f2797f4c63be734eab71b5da1025d334620dd0a6978f80cb11022c88ccfcec`  
		Last Modified: Sat, 30 Apr 2022 00:11:31 GMT  
		Size: 6.8 KB (6777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e66b201216b5bebbd358365e3b3c977f306720c2dcd66dad04da85aeeb1ac9ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139536731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff5e20d4ebd7fe8753ba3d0e7907e1a21a78868e5672e580c4951ab3f27b484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:29:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 22 Apr 2022 10:30:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:30:29 GMT
ENV GOSU_VERSION=1.14
# Fri, 22 Apr 2022 10:31:11 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 22 Apr 2022 10:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 22 Apr 2022 10:31:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:31:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 22 Apr 2022 10:31:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 22 Apr 2022 10:34:08 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:09 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 22 Apr 2022 10:34:11 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:12 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 22 Apr 2022 10:34:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 22 Apr 2022 10:34:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 22 Apr 2022 10:36:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 22 Apr 2022 10:36:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 22 Apr 2022 10:36:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 22 Apr 2022 10:36:16 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 22 Apr 2022 10:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 10:36:19 GMT
EXPOSE 3306
# Fri, 22 Apr 2022 10:36:21 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be0ad54de6069c64f7b43c074840e67d3ddd21cc2ad90b05d7d0457b4be81be`  
		Last Modified: Fri, 22 Apr 2022 10:52:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a08ff384025c85f93f2989db3024179ae496da9e36b2feec6647df6c36a0c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 6.7 MB (6667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53313c251391a9eaf379d639ea11ac4249154c5f10ee6d340d40778fbf0e9896`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 3.7 MB (3672387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eac687e1d0f9671e2102f2297b475bee41f5b5ce630b31dffb6b0a01f9710a7`  
		Last Modified: Fri, 22 Apr 2022 10:52:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0385c9ef3c7732b5c6caca569ab2d7a382520e1b9d1d3190c92c42a72985b9c`  
		Last Modified: Fri, 22 Apr 2022 10:52:08 GMT  
		Size: 2.6 MB (2568219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77d42234064d5e8b5c0451fc70a307f3dc89bb4d58b6d7df4024e5c05d54ca8`  
		Last Modified: Fri, 22 Apr 2022 10:52:03 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fdd8f2b7ed887c119c9ca942715f9f1d4e3d0704344fe671cb921c3df6e6`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc7852c7cfc5a89e8ec199e80be577caf5cb6278d52334b86888dad8b9a5d19`  
		Last Modified: Fri, 22 Apr 2022 10:53:01 GMT  
		Size: 93.3 MB (93323480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90b1dfdfe9bb649c7f4ce895a13e16f1cefed0bd1dca47c742a8dbb7f7ecd33`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf93f3686f15dba104bc6ae5f4303b33340d33a2d4244c00f76ef218d9ded2d`  
		Last Modified: Fri, 22 Apr 2022 10:52:43 GMT  
		Size: 6.8 KB (6778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:834212faeb75a2a43648a37982041f285f537b5cb1e3b0d4698a8df3732007cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127701635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5e6a0fd99b6b261fb89f90ebda2e325da3051f0d56a4895f553c69af9c69686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:44:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Apr 2022 23:44:39 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:40 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Apr 2022 23:44:50 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Apr 2022 23:44:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Apr 2022 23:44:56 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:44:56 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Apr 2022 23:44:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Apr 2022 23:45:41 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:41 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 29 Apr 2022 23:45:42 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 29 Apr 2022 23:45:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 29 Apr 2022 23:45:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Apr 2022 23:46:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Apr 2022 23:46:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Apr 2022 23:46:15 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Fri, 29 Apr 2022 23:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Apr 2022 23:46:15 GMT
EXPOSE 3306
# Fri, 29 Apr 2022 23:46:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d94a3bb2fc539579c4f036c3b3118da4202863463564d17683b22216ee287d`  
		Last Modified: Fri, 29 Apr 2022 23:48:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73adb98f19e9309bc38c5f4d51b5268c971697a3893a5785a91042a9d7ad5716`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 5.4 MB (5378443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485a2faaf09d2e03e8beb15803c8b55cb8f315f538e45f8fa80a8b3634d1271a`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 3.2 MB (3243950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecd90f1ad3ffaf9b6c65548d8a73e0c78a4850bebc2d8ab0f6eb8d9c53fc337`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d106db260d87aa469fd4081fed0423071d5e56bd09cd4313cb87944310b1dbe`  
		Last Modified: Fri, 29 Apr 2022 23:48:34 GMT  
		Size: 2.2 MB (2183475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf5cf8408ffb03733ed0acf3d4ac29524279620d7304f22a0c58a00c3c5f47`  
		Last Modified: Fri, 29 Apr 2022 23:48:32 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70732cc91f318d007de766e94265f7a0539440482fedce98b4ed140173b77f1c`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44483aab52b201a5daba428dbb324742d6ece06777315a61021f24fc22a740cd`  
		Last Modified: Fri, 29 Apr 2022 23:49:09 GMT  
		Size: 89.8 MB (89815369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d5f62ecf4e209a33d158a01c03b82ad089be13910b212570c95d41706666df`  
		Last Modified: Fri, 29 Apr 2022 23:48:56 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d60e7434e17b71d925c7fe28efc5dfee00d94111b7a8225788104b4c04262ec`  
		Last Modified: Fri, 29 Apr 2022 23:48:57 GMT  
		Size: 6.8 KB (6775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
