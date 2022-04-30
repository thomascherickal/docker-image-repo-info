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
