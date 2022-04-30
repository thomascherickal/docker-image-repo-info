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
$ docker pull mariadb@sha256:07e06f2e7ae9dfc63707a83130a62e00167c827f08fcac7a9aa33f4b6dc34e0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:a252cb5322f288f0bbba2c289828db981ed4df92ecc35bce77881ec774982a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daf0f023c28d0a811ba382b5645b71cc771c49fd15d53b8075018fb15e677d05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:17:56 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:17:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:24 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:18:24 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:18:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c0075a397aba5c127769d6a6215111fd53df47f5c7b95491172709c21c210f`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a5800afaceb66771d7d7d5d6290e5dbb1cf69e96fa8cb9e218623d2d70178`  
		Last Modified: Sat, 30 Apr 2022 01:23:11 GMT  
		Size: 88.7 MB (88741718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27261e54ed45f6cf3697709e7fe0f23952ef5fd6123cefcadaf1f65296e72737`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18f8f832430d5c46086dbcd197ccdb6fe2ba4b1467e9e755ad2c6a8b205292`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
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
$ docker pull mariadb@sha256:9f0a93c25897df9a9b2ca3becf35fccdfd9531009c57b1481d8d027f8722dc49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139538393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9fdde589bdb89bddd62d2076c08de8ca866b15932b15f44b9809efd0a2c54d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:59:29 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:47 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:55 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:09 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:00:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:03:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:03:59 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:04:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:04:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:04:08 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:04:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38d1aea9df71e0e7b7a07ebbf73d3df047d6925b8517612731ce14b29d81e6f`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219c8b280b85bfcb106c1c23cb4f820d20c27c361c26bc4b7b20b972ae0e550d`  
		Last Modified: Sat, 30 Apr 2022 01:21:50 GMT  
		Size: 93.3 MB (93324167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca5c34dd9a2fb0cbcf95168f69c6aa33df79bce1e843d573af62fc0ca0bf60`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ec7c5c6f4af575453b8a299723e99a51c614cf4d411dc507c8c4970ecaf71`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 6.8 KB (6774 bytes)  
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
$ docker pull mariadb@sha256:07e06f2e7ae9dfc63707a83130a62e00167c827f08fcac7a9aa33f4b6dc34e0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:a252cb5322f288f0bbba2c289828db981ed4df92ecc35bce77881ec774982a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daf0f023c28d0a811ba382b5645b71cc771c49fd15d53b8075018fb15e677d05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:17:56 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:17:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:24 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:18:24 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:18:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c0075a397aba5c127769d6a6215111fd53df47f5c7b95491172709c21c210f`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a5800afaceb66771d7d7d5d6290e5dbb1cf69e96fa8cb9e218623d2d70178`  
		Last Modified: Sat, 30 Apr 2022 01:23:11 GMT  
		Size: 88.7 MB (88741718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27261e54ed45f6cf3697709e7fe0f23952ef5fd6123cefcadaf1f65296e72737`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18f8f832430d5c46086dbcd197ccdb6fe2ba4b1467e9e755ad2c6a8b205292`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
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
$ docker pull mariadb@sha256:9f0a93c25897df9a9b2ca3becf35fccdfd9531009c57b1481d8d027f8722dc49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139538393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9fdde589bdb89bddd62d2076c08de8ca866b15932b15f44b9809efd0a2c54d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:59:29 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:47 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:55 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:09 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:00:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:03:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:03:59 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:04:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:04:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:04:08 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:04:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38d1aea9df71e0e7b7a07ebbf73d3df047d6925b8517612731ce14b29d81e6f`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219c8b280b85bfcb106c1c23cb4f820d20c27c361c26bc4b7b20b972ae0e550d`  
		Last Modified: Sat, 30 Apr 2022 01:21:50 GMT  
		Size: 93.3 MB (93324167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca5c34dd9a2fb0cbcf95168f69c6aa33df79bce1e843d573af62fc0ca0bf60`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ec7c5c6f4af575453b8a299723e99a51c614cf4d411dc507c8c4970ecaf71`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 6.8 KB (6774 bytes)  
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
$ docker pull mariadb@sha256:b7192a8f1e3597e41b17a81e33b13e94cdfd92e9461d1e2f5a743f7ca6d0f2aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:dddbb9e57adcf4daa11c3d2a42c0815361d862b433f87823db677a991acef01f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109316379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005e450d582e0a55c2a96bf986588481d2e413a401f36a1a135c598075f809e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:20:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:20:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:20:54 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:21:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:21:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:21:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:21:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:21:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:21:17 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:21:17 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:21:17 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:21:17 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:21:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Sat, 30 Apr 2022 01:21:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:21:51 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:21:51 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:21:51 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:21:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:21:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:21:52 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:21:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190b8c80b7103756fd9375f1cb894bfd4c3af205728f36d6eec4794d23d98ffd`  
		Last Modified: Sat, 30 Apr 2022 01:25:41 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f755b4f7a5e833d6cea1644bc8d71f3a552c592f26010ddab15026b55916c228`  
		Last Modified: Sat, 30 Apr 2022 01:25:42 GMT  
		Size: 4.8 MB (4813356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0b5b9b99ce0fb23a23284f700464a2a19d791fa7a6965c5e1e104460836dfe`  
		Last Modified: Sat, 30 Apr 2022 01:25:40 GMT  
		Size: 3.6 MB (3553311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f35866a1805c7af691937e6f62f09aa1603e0b84587ea01d78068d5a17973a`  
		Last Modified: Sat, 30 Apr 2022 01:25:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54ee4cc8b0844161ce39e700e1e3452dcd6fd5b8afb000296af8c3c19bdc916`  
		Last Modified: Sat, 30 Apr 2022 01:25:39 GMT  
		Size: 1.6 MB (1583543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317f7603ac96b53ec5aaccaeaaa0935832dd58778caab2a13c6d7e048329264c`  
		Last Modified: Sat, 30 Apr 2022 01:25:39 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b95497aa877ed66a64b16f85d0579999b233599ae75e717e3d4413218534a`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e1f698d414e2f673124db02942f60eef713ab28f5ff611a7dec1c48cc92120`  
		Last Modified: Sat, 30 Apr 2022 01:25:48 GMT  
		Size: 72.6 MB (72639162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39129eee82af59d4c3bd139157767aa7de2c29c5fbd96a920bccbbf752b6c82d`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dd6df4730a4744a4780e0878f1d2ad35753365414d5802c85b91d36ace7590`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea33a9dc9b049082ee64b1ca85fcdb39edb0f2bd9a7cd15f165c96e77cd96e`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
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
$ docker pull mariadb@sha256:53dcf3ff44311ef8aab2de165d72af2bc480aad91556893e12d4585f7eb32163
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117724105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:004bd7db539770985ea0d8caa061eed86b79cbe895140bd9b02c2a3c5beb5256`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:00 GMT
ADD file:2d91cfcbab5facf9c027064efd477cfde81eca0c1a62c6611ac694bafb94d817 in / 
# Fri, 29 Apr 2022 23:22:04 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:14:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:15:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:15:24 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:16:01 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:16:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:16:32 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:16:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:16:49 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:16:52 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:16:55 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:16:57 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:17:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Sat, 30 Apr 2022 01:17:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:57 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:58 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:19:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:19:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:19:11 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:19:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c70b79613e1f9e69f0d6473fa0b3f8b10d376e24350617c381ed64978f4bae97`  
		Last Modified: Fri, 29 Apr 2022 23:24:58 GMT  
		Size: 30.4 MB (30443183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448ae79bf43f8c59af197df2aff3d1e4134ffec92a9689023e25f1cf20665c5a`  
		Last Modified: Sat, 30 Apr 2022 01:25:18 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f1abd7822aced7810b1eeed5428599e37ce652171494a0d37f7af1a9032509`  
		Last Modified: Sat, 30 Apr 2022 01:25:18 GMT  
		Size: 5.6 MB (5630459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799d2b082938ff06ee285f7c5558acfdbc4c0ef8a76dcd7659a81e7aa2a3689`  
		Last Modified: Sat, 30 Apr 2022 01:25:15 GMT  
		Size: 3.5 MB (3533678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8b00fbe9c59d34bef9471c373fcf3be53dac2b02ea93292a91001250c83d77`  
		Last Modified: Sat, 30 Apr 2022 01:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed0a19fddbe862f31d5f1b6ed06e2adf508d897fde6cc9bef3854ab642f895c`  
		Last Modified: Sat, 30 Apr 2022 01:25:14 GMT  
		Size: 1.9 MB (1940585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0658ae05e18419daff1f358fb666932ae8e20f8ce1065899ddfb3596900618`  
		Last Modified: Sat, 30 Apr 2022 01:25:13 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1066f1d5876bbe7075a484a0a3c0a066d4a6b2f5de631cf46bd9244007346a0`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d7dc4893fd0dedcf3080a69baa1fa3b50ef081ab072b4f03d052185cc8f6e`  
		Last Modified: Sat, 30 Apr 2022 01:25:25 GMT  
		Size: 76.2 MB (76158287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4795e9c47ca3398d9964c8067fe3e87b8c740875b7c4a3dec9b8a7e61a27c740`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b643d8715e8490c7c0ae64dbf90b2f9fb03b20bc45ea4ae0a8d9bc26b992bd`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17376a0aa9f49f43012e17503df54fc2b8a3d59654138af6a5f0c76f9b9294c`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:b7192a8f1e3597e41b17a81e33b13e94cdfd92e9461d1e2f5a743f7ca6d0f2aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:dddbb9e57adcf4daa11c3d2a42c0815361d862b433f87823db677a991acef01f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109316379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005e450d582e0a55c2a96bf986588481d2e413a401f36a1a135c598075f809e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:20:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:20:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:20:54 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:21:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:21:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:21:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:21:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:21:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:21:17 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:21:17 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:21:17 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:21:17 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:21:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Sat, 30 Apr 2022 01:21:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:21:51 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:21:51 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:21:51 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:21:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:21:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:21:52 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:21:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190b8c80b7103756fd9375f1cb894bfd4c3af205728f36d6eec4794d23d98ffd`  
		Last Modified: Sat, 30 Apr 2022 01:25:41 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f755b4f7a5e833d6cea1644bc8d71f3a552c592f26010ddab15026b55916c228`  
		Last Modified: Sat, 30 Apr 2022 01:25:42 GMT  
		Size: 4.8 MB (4813356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0b5b9b99ce0fb23a23284f700464a2a19d791fa7a6965c5e1e104460836dfe`  
		Last Modified: Sat, 30 Apr 2022 01:25:40 GMT  
		Size: 3.6 MB (3553311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f35866a1805c7af691937e6f62f09aa1603e0b84587ea01d78068d5a17973a`  
		Last Modified: Sat, 30 Apr 2022 01:25:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54ee4cc8b0844161ce39e700e1e3452dcd6fd5b8afb000296af8c3c19bdc916`  
		Last Modified: Sat, 30 Apr 2022 01:25:39 GMT  
		Size: 1.6 MB (1583543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317f7603ac96b53ec5aaccaeaaa0935832dd58778caab2a13c6d7e048329264c`  
		Last Modified: Sat, 30 Apr 2022 01:25:39 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b95497aa877ed66a64b16f85d0579999b233599ae75e717e3d4413218534a`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e1f698d414e2f673124db02942f60eef713ab28f5ff611a7dec1c48cc92120`  
		Last Modified: Sat, 30 Apr 2022 01:25:48 GMT  
		Size: 72.6 MB (72639162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39129eee82af59d4c3bd139157767aa7de2c29c5fbd96a920bccbbf752b6c82d`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dd6df4730a4744a4780e0878f1d2ad35753365414d5802c85b91d36ace7590`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea33a9dc9b049082ee64b1ca85fcdb39edb0f2bd9a7cd15f165c96e77cd96e`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
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
$ docker pull mariadb@sha256:53dcf3ff44311ef8aab2de165d72af2bc480aad91556893e12d4585f7eb32163
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117724105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:004bd7db539770985ea0d8caa061eed86b79cbe895140bd9b02c2a3c5beb5256`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:00 GMT
ADD file:2d91cfcbab5facf9c027064efd477cfde81eca0c1a62c6611ac694bafb94d817 in / 
# Fri, 29 Apr 2022 23:22:04 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:14:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:15:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:15:24 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:16:01 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:16:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:16:32 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:16:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:16:49 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:16:52 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:16:55 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:16:57 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:17:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Sat, 30 Apr 2022 01:17:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:57 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:58 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:19:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:19:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:19:11 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:19:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c70b79613e1f9e69f0d6473fa0b3f8b10d376e24350617c381ed64978f4bae97`  
		Last Modified: Fri, 29 Apr 2022 23:24:58 GMT  
		Size: 30.4 MB (30443183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448ae79bf43f8c59af197df2aff3d1e4134ffec92a9689023e25f1cf20665c5a`  
		Last Modified: Sat, 30 Apr 2022 01:25:18 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f1abd7822aced7810b1eeed5428599e37ce652171494a0d37f7af1a9032509`  
		Last Modified: Sat, 30 Apr 2022 01:25:18 GMT  
		Size: 5.6 MB (5630459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799d2b082938ff06ee285f7c5558acfdbc4c0ef8a76dcd7659a81e7aa2a3689`  
		Last Modified: Sat, 30 Apr 2022 01:25:15 GMT  
		Size: 3.5 MB (3533678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8b00fbe9c59d34bef9471c373fcf3be53dac2b02ea93292a91001250c83d77`  
		Last Modified: Sat, 30 Apr 2022 01:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed0a19fddbe862f31d5f1b6ed06e2adf508d897fde6cc9bef3854ab642f895c`  
		Last Modified: Sat, 30 Apr 2022 01:25:14 GMT  
		Size: 1.9 MB (1940585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0658ae05e18419daff1f358fb666932ae8e20f8ce1065899ddfb3596900618`  
		Last Modified: Sat, 30 Apr 2022 01:25:13 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1066f1d5876bbe7075a484a0a3c0a066d4a6b2f5de631cf46bd9244007346a0`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d7dc4893fd0dedcf3080a69baa1fa3b50ef081ab072b4f03d052185cc8f6e`  
		Last Modified: Sat, 30 Apr 2022 01:25:25 GMT  
		Size: 76.2 MB (76158287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4795e9c47ca3398d9964c8067fe3e87b8c740875b7c4a3dec9b8a7e61a27c740`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b643d8715e8490c7c0ae64dbf90b2f9fb03b20bc45ea4ae0a8d9bc26b992bd`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17376a0aa9f49f43012e17503df54fc2b8a3d59654138af6a5f0c76f9b9294c`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.43`

```console
$ docker pull mariadb@sha256:b7192a8f1e3597e41b17a81e33b13e94cdfd92e9461d1e2f5a743f7ca6d0f2aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.43` - linux; amd64

```console
$ docker pull mariadb@sha256:dddbb9e57adcf4daa11c3d2a42c0815361d862b433f87823db677a991acef01f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109316379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005e450d582e0a55c2a96bf986588481d2e413a401f36a1a135c598075f809e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:20:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:20:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:20:54 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:21:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:21:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:21:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:21:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:21:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:21:17 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:21:17 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:21:17 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:21:17 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:21:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Sat, 30 Apr 2022 01:21:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:21:51 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:21:51 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:21:51 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:21:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:21:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:21:52 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:21:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190b8c80b7103756fd9375f1cb894bfd4c3af205728f36d6eec4794d23d98ffd`  
		Last Modified: Sat, 30 Apr 2022 01:25:41 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f755b4f7a5e833d6cea1644bc8d71f3a552c592f26010ddab15026b55916c228`  
		Last Modified: Sat, 30 Apr 2022 01:25:42 GMT  
		Size: 4.8 MB (4813356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0b5b9b99ce0fb23a23284f700464a2a19d791fa7a6965c5e1e104460836dfe`  
		Last Modified: Sat, 30 Apr 2022 01:25:40 GMT  
		Size: 3.6 MB (3553311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f35866a1805c7af691937e6f62f09aa1603e0b84587ea01d78068d5a17973a`  
		Last Modified: Sat, 30 Apr 2022 01:25:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54ee4cc8b0844161ce39e700e1e3452dcd6fd5b8afb000296af8c3c19bdc916`  
		Last Modified: Sat, 30 Apr 2022 01:25:39 GMT  
		Size: 1.6 MB (1583543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317f7603ac96b53ec5aaccaeaaa0935832dd58778caab2a13c6d7e048329264c`  
		Last Modified: Sat, 30 Apr 2022 01:25:39 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b95497aa877ed66a64b16f85d0579999b233599ae75e717e3d4413218534a`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e1f698d414e2f673124db02942f60eef713ab28f5ff611a7dec1c48cc92120`  
		Last Modified: Sat, 30 Apr 2022 01:25:48 GMT  
		Size: 72.6 MB (72639162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39129eee82af59d4c3bd139157767aa7de2c29c5fbd96a920bccbbf752b6c82d`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dd6df4730a4744a4780e0878f1d2ad35753365414d5802c85b91d36ace7590`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea33a9dc9b049082ee64b1ca85fcdb39edb0f2bd9a7cd15f165c96e77cd96e`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
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
$ docker pull mariadb@sha256:53dcf3ff44311ef8aab2de165d72af2bc480aad91556893e12d4585f7eb32163
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117724105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:004bd7db539770985ea0d8caa061eed86b79cbe895140bd9b02c2a3c5beb5256`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:00 GMT
ADD file:2d91cfcbab5facf9c027064efd477cfde81eca0c1a62c6611ac694bafb94d817 in / 
# Fri, 29 Apr 2022 23:22:04 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:14:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:15:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:15:24 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:16:01 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:16:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:16:32 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:16:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:16:49 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:16:52 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:16:55 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:16:57 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:17:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Sat, 30 Apr 2022 01:17:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:57 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:58 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:19:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:19:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:19:11 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:19:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c70b79613e1f9e69f0d6473fa0b3f8b10d376e24350617c381ed64978f4bae97`  
		Last Modified: Fri, 29 Apr 2022 23:24:58 GMT  
		Size: 30.4 MB (30443183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448ae79bf43f8c59af197df2aff3d1e4134ffec92a9689023e25f1cf20665c5a`  
		Last Modified: Sat, 30 Apr 2022 01:25:18 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f1abd7822aced7810b1eeed5428599e37ce652171494a0d37f7af1a9032509`  
		Last Modified: Sat, 30 Apr 2022 01:25:18 GMT  
		Size: 5.6 MB (5630459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799d2b082938ff06ee285f7c5558acfdbc4c0ef8a76dcd7659a81e7aa2a3689`  
		Last Modified: Sat, 30 Apr 2022 01:25:15 GMT  
		Size: 3.5 MB (3533678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8b00fbe9c59d34bef9471c373fcf3be53dac2b02ea93292a91001250c83d77`  
		Last Modified: Sat, 30 Apr 2022 01:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed0a19fddbe862f31d5f1b6ed06e2adf508d897fde6cc9bef3854ab642f895c`  
		Last Modified: Sat, 30 Apr 2022 01:25:14 GMT  
		Size: 1.9 MB (1940585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0658ae05e18419daff1f358fb666932ae8e20f8ce1065899ddfb3596900618`  
		Last Modified: Sat, 30 Apr 2022 01:25:13 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1066f1d5876bbe7075a484a0a3c0a066d4a6b2f5de631cf46bd9244007346a0`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d7dc4893fd0dedcf3080a69baa1fa3b50ef081ab072b4f03d052185cc8f6e`  
		Last Modified: Sat, 30 Apr 2022 01:25:25 GMT  
		Size: 76.2 MB (76158287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4795e9c47ca3398d9964c8067fe3e87b8c740875b7c4a3dec9b8a7e61a27c740`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b643d8715e8490c7c0ae64dbf90b2f9fb03b20bc45ea4ae0a8d9bc26b992bd`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17376a0aa9f49f43012e17503df54fc2b8a3d59654138af6a5f0c76f9b9294c`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.43-bionic`

```console
$ docker pull mariadb@sha256:b7192a8f1e3597e41b17a81e33b13e94cdfd92e9461d1e2f5a743f7ca6d0f2aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.43-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:dddbb9e57adcf4daa11c3d2a42c0815361d862b433f87823db677a991acef01f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109316379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005e450d582e0a55c2a96bf986588481d2e413a401f36a1a135c598075f809e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:20:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:20:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:20:54 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:21:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:21:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:21:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:21:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:21:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:21:17 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:21:17 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:21:17 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:21:17 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:21:17 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Sat, 30 Apr 2022 01:21:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:21:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:21:51 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:21:51 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:21:51 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:21:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:21:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:21:52 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:21:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190b8c80b7103756fd9375f1cb894bfd4c3af205728f36d6eec4794d23d98ffd`  
		Last Modified: Sat, 30 Apr 2022 01:25:41 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f755b4f7a5e833d6cea1644bc8d71f3a552c592f26010ddab15026b55916c228`  
		Last Modified: Sat, 30 Apr 2022 01:25:42 GMT  
		Size: 4.8 MB (4813356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0b5b9b99ce0fb23a23284f700464a2a19d791fa7a6965c5e1e104460836dfe`  
		Last Modified: Sat, 30 Apr 2022 01:25:40 GMT  
		Size: 3.6 MB (3553311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f35866a1805c7af691937e6f62f09aa1603e0b84587ea01d78068d5a17973a`  
		Last Modified: Sat, 30 Apr 2022 01:25:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54ee4cc8b0844161ce39e700e1e3452dcd6fd5b8afb000296af8c3c19bdc916`  
		Last Modified: Sat, 30 Apr 2022 01:25:39 GMT  
		Size: 1.6 MB (1583543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317f7603ac96b53ec5aaccaeaaa0935832dd58778caab2a13c6d7e048329264c`  
		Last Modified: Sat, 30 Apr 2022 01:25:39 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b95497aa877ed66a64b16f85d0579999b233599ae75e717e3d4413218534a`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e1f698d414e2f673124db02942f60eef713ab28f5ff611a7dec1c48cc92120`  
		Last Modified: Sat, 30 Apr 2022 01:25:48 GMT  
		Size: 72.6 MB (72639162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39129eee82af59d4c3bd139157767aa7de2c29c5fbd96a920bccbbf752b6c82d`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dd6df4730a4744a4780e0878f1d2ad35753365414d5802c85b91d36ace7590`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bea33a9dc9b049082ee64b1ca85fcdb39edb0f2bd9a7cd15f165c96e77cd96e`  
		Last Modified: Sat, 30 Apr 2022 01:25:37 GMT  
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
$ docker pull mariadb@sha256:53dcf3ff44311ef8aab2de165d72af2bc480aad91556893e12d4585f7eb32163
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117724105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:004bd7db539770985ea0d8caa061eed86b79cbe895140bd9b02c2a3c5beb5256`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:00 GMT
ADD file:2d91cfcbab5facf9c027064efd477cfde81eca0c1a62c6611ac694bafb94d817 in / 
# Fri, 29 Apr 2022 23:22:04 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:14:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:15:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:15:24 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:16:01 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:16:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:16:32 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:36 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:16:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:16:49 GMT
ARG MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:16:52 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 30 Apr 2022 01:16:55 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:16:57 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Sat, 30 Apr 2022 01:17:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Sat, 30 Apr 2022 01:17:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:57 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:58 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:19:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:19:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:19:11 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:19:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c70b79613e1f9e69f0d6473fa0b3f8b10d376e24350617c381ed64978f4bae97`  
		Last Modified: Fri, 29 Apr 2022 23:24:58 GMT  
		Size: 30.4 MB (30443183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448ae79bf43f8c59af197df2aff3d1e4134ffec92a9689023e25f1cf20665c5a`  
		Last Modified: Sat, 30 Apr 2022 01:25:18 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f1abd7822aced7810b1eeed5428599e37ce652171494a0d37f7af1a9032509`  
		Last Modified: Sat, 30 Apr 2022 01:25:18 GMT  
		Size: 5.6 MB (5630459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e799d2b082938ff06ee285f7c5558acfdbc4c0ef8a76dcd7659a81e7aa2a3689`  
		Last Modified: Sat, 30 Apr 2022 01:25:15 GMT  
		Size: 3.5 MB (3533678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8b00fbe9c59d34bef9471c373fcf3be53dac2b02ea93292a91001250c83d77`  
		Last Modified: Sat, 30 Apr 2022 01:25:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed0a19fddbe862f31d5f1b6ed06e2adf508d897fde6cc9bef3854ab642f895c`  
		Last Modified: Sat, 30 Apr 2022 01:25:14 GMT  
		Size: 1.9 MB (1940585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0658ae05e18419daff1f358fb666932ae8e20f8ce1065899ddfb3596900618`  
		Last Modified: Sat, 30 Apr 2022 01:25:13 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1066f1d5876bbe7075a484a0a3c0a066d4a6b2f5de631cf46bd9244007346a0`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d7dc4893fd0dedcf3080a69baa1fa3b50ef081ab072b4f03d052185cc8f6e`  
		Last Modified: Sat, 30 Apr 2022 01:25:25 GMT  
		Size: 76.2 MB (76158287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4795e9c47ca3398d9964c8067fe3e87b8c740875b7c4a3dec9b8a7e61a27c740`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b643d8715e8490c7c0ae64dbf90b2f9fb03b20bc45ea4ae0a8d9bc26b992bd`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 6.8 KB (6770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17376a0aa9f49f43012e17503df54fc2b8a3d59654138af6a5f0c76f9b9294c`  
		Last Modified: Sat, 30 Apr 2022 01:25:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:4e69699f60f4c9558ad2b647bce4d34282878341a7a614c5f247999bb6e7ee94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:50b2b331cac391840255a45a7db888a05cd3aae3ca3c4f8aa15f7ae720820908
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120118308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b4bd92cc2beffd7bc338a0d0ec06338dbb6b08c6da93a8629f09eb8240afdd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:20:05 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:20:05 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:20:05 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:20:05 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:20:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:20:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:20:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:20:37 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:20:37 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:20:37 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:20:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:20:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:20:38 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:20:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb73d705ad0a2c75a41410e21328b0bd34968d48a054220e0b5333e70846e713`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e77e97d6950896df936a43926061f2a62ffffa0d05007f4367ab46de4e4b794`  
		Last Modified: Sat, 30 Apr 2022 01:25:20 GMT  
		Size: 80.2 MB (80191360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c54b35786ca8151a16f0b7f17a7c79fb3b6fa1327e7921e5f64fc35a5b1112a`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ccdc7b428b8a56574c890ab374664f2c6d7cd8d5348430c06652b948db4f96`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10815100c7b7f595c7c7eaef8115720341e35a3f9f35fec046a27c4afe92ec61`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
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
$ docker pull mariadb@sha256:e7e30be7c84d4aefe17702320311b40a5d1e90f4828d74253783ee68d921a654
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131006518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b39b875c5dde0758addb327f3a167bd4107a3a75486abd22fcc434be63879a2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:11:45 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:11:48 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:11:50 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:11:52 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:11:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:12:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:13:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:13:50 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:13:51 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:13:53 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:14:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:14:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:14:07 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:14:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca5699fb702d52f4be5f401b0b316ae92d3baab98564d2b0b84eecc516df096`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b492b24a4b7340ae935879af5d26812ceba33c86871c88c71ad05191d4262a6`  
		Last Modified: Sat, 30 Apr 2022 01:24:49 GMT  
		Size: 84.8 MB (84792168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187e96a7eac95905880ae6cc864df5d611c28db89d7d6107310ab0cf8c887ecd`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b07dd40e72709cdb7735b15e9062c71dbbd4a2867d8930ae00587953c2450e3`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63872fc4cc07275f6e6227cbd1497d35ab28144a9f560459b47c4358876bb9e8`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:4e69699f60f4c9558ad2b647bce4d34282878341a7a614c5f247999bb6e7ee94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:50b2b331cac391840255a45a7db888a05cd3aae3ca3c4f8aa15f7ae720820908
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120118308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b4bd92cc2beffd7bc338a0d0ec06338dbb6b08c6da93a8629f09eb8240afdd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:20:05 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:20:05 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:20:05 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:20:05 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:20:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:20:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:20:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:20:37 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:20:37 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:20:37 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:20:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:20:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:20:38 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:20:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb73d705ad0a2c75a41410e21328b0bd34968d48a054220e0b5333e70846e713`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e77e97d6950896df936a43926061f2a62ffffa0d05007f4367ab46de4e4b794`  
		Last Modified: Sat, 30 Apr 2022 01:25:20 GMT  
		Size: 80.2 MB (80191360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c54b35786ca8151a16f0b7f17a7c79fb3b6fa1327e7921e5f64fc35a5b1112a`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ccdc7b428b8a56574c890ab374664f2c6d7cd8d5348430c06652b948db4f96`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10815100c7b7f595c7c7eaef8115720341e35a3f9f35fec046a27c4afe92ec61`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
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
$ docker pull mariadb@sha256:e7e30be7c84d4aefe17702320311b40a5d1e90f4828d74253783ee68d921a654
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131006518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b39b875c5dde0758addb327f3a167bd4107a3a75486abd22fcc434be63879a2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:11:45 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:11:48 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:11:50 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:11:52 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:11:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:12:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:13:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:13:50 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:13:51 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:13:53 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:14:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:14:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:14:07 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:14:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca5699fb702d52f4be5f401b0b316ae92d3baab98564d2b0b84eecc516df096`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b492b24a4b7340ae935879af5d26812ceba33c86871c88c71ad05191d4262a6`  
		Last Modified: Sat, 30 Apr 2022 01:24:49 GMT  
		Size: 84.8 MB (84792168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187e96a7eac95905880ae6cc864df5d611c28db89d7d6107310ab0cf8c887ecd`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b07dd40e72709cdb7735b15e9062c71dbbd4a2867d8930ae00587953c2450e3`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63872fc4cc07275f6e6227cbd1497d35ab28144a9f560459b47c4358876bb9e8`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.34`

```console
$ docker pull mariadb@sha256:4e69699f60f4c9558ad2b647bce4d34282878341a7a614c5f247999bb6e7ee94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.34` - linux; amd64

```console
$ docker pull mariadb@sha256:50b2b331cac391840255a45a7db888a05cd3aae3ca3c4f8aa15f7ae720820908
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120118308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b4bd92cc2beffd7bc338a0d0ec06338dbb6b08c6da93a8629f09eb8240afdd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:20:05 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:20:05 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:20:05 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:20:05 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:20:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:20:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:20:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:20:37 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:20:37 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:20:37 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:20:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:20:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:20:38 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:20:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb73d705ad0a2c75a41410e21328b0bd34968d48a054220e0b5333e70846e713`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e77e97d6950896df936a43926061f2a62ffffa0d05007f4367ab46de4e4b794`  
		Last Modified: Sat, 30 Apr 2022 01:25:20 GMT  
		Size: 80.2 MB (80191360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c54b35786ca8151a16f0b7f17a7c79fb3b6fa1327e7921e5f64fc35a5b1112a`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ccdc7b428b8a56574c890ab374664f2c6d7cd8d5348430c06652b948db4f96`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10815100c7b7f595c7c7eaef8115720341e35a3f9f35fec046a27c4afe92ec61`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
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
$ docker pull mariadb@sha256:e7e30be7c84d4aefe17702320311b40a5d1e90f4828d74253783ee68d921a654
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131006518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b39b875c5dde0758addb327f3a167bd4107a3a75486abd22fcc434be63879a2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:11:45 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:11:48 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:11:50 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:11:52 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:11:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:12:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:13:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:13:50 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:13:51 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:13:53 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:14:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:14:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:14:07 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:14:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca5699fb702d52f4be5f401b0b316ae92d3baab98564d2b0b84eecc516df096`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b492b24a4b7340ae935879af5d26812ceba33c86871c88c71ad05191d4262a6`  
		Last Modified: Sat, 30 Apr 2022 01:24:49 GMT  
		Size: 84.8 MB (84792168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187e96a7eac95905880ae6cc864df5d611c28db89d7d6107310ab0cf8c887ecd`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b07dd40e72709cdb7735b15e9062c71dbbd4a2867d8930ae00587953c2450e3`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63872fc4cc07275f6e6227cbd1497d35ab28144a9f560459b47c4358876bb9e8`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.34-focal`

```console
$ docker pull mariadb@sha256:4e69699f60f4c9558ad2b647bce4d34282878341a7a614c5f247999bb6e7ee94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.34-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:50b2b331cac391840255a45a7db888a05cd3aae3ca3c4f8aa15f7ae720820908
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120118308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b4bd92cc2beffd7bc338a0d0ec06338dbb6b08c6da93a8629f09eb8240afdd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:20:05 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:20:05 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:20:05 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:20:05 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:20:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:20:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:20:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:20:37 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:20:37 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:20:37 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:20:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:20:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:20:38 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:20:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb73d705ad0a2c75a41410e21328b0bd34968d48a054220e0b5333e70846e713`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e77e97d6950896df936a43926061f2a62ffffa0d05007f4367ab46de4e4b794`  
		Last Modified: Sat, 30 Apr 2022 01:25:20 GMT  
		Size: 80.2 MB (80191360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c54b35786ca8151a16f0b7f17a7c79fb3b6fa1327e7921e5f64fc35a5b1112a`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ccdc7b428b8a56574c890ab374664f2c6d7cd8d5348430c06652b948db4f96`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10815100c7b7f595c7c7eaef8115720341e35a3f9f35fec046a27c4afe92ec61`  
		Last Modified: Sat, 30 Apr 2022 01:25:08 GMT  
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
$ docker pull mariadb@sha256:e7e30be7c84d4aefe17702320311b40a5d1e90f4828d74253783ee68d921a654
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131006518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b39b875c5dde0758addb327f3a167bd4107a3a75486abd22fcc434be63879a2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:11:45 GMT
ARG MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:11:48 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 30 Apr 2022 01:11:50 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:11:52 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Sat, 30 Apr 2022 01:11:55 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:12:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:13:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:13:50 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:13:51 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:13:53 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:14:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:14:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:14:07 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:14:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca5699fb702d52f4be5f401b0b316ae92d3baab98564d2b0b84eecc516df096`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b492b24a4b7340ae935879af5d26812ceba33c86871c88c71ad05191d4262a6`  
		Last Modified: Sat, 30 Apr 2022 01:24:49 GMT  
		Size: 84.8 MB (84792168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187e96a7eac95905880ae6cc864df5d611c28db89d7d6107310ab0cf8c887ecd`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b07dd40e72709cdb7735b15e9062c71dbbd4a2867d8930ae00587953c2450e3`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 6.8 KB (6773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63872fc4cc07275f6e6227cbd1497d35ab28144a9f560459b47c4358876bb9e8`  
		Last Modified: Sat, 30 Apr 2022 01:24:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:988c5e2073c8f9d49b4e2b8751d83839c53a5ae5f0a082450e9d0e83f359d45a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:31ffd93952ec8e67043b4442d399848781544508a5973ea4aef3a18478aa99c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c6c06541d48a629298ea6a58723be7712a6f866368018343adb914053e5602e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:19:32 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:19:32 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:19:32 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:19:32 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:19:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:19:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:20:00 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:20:00 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:20:01 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:20:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:20:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:20:01 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:20:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c653cb741960a71b44f4d61f043db04054ca6584d06fb1b7af5be93cf098ac50`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5571e050f105e60b660470785d52e7698eefaee024a561eaf62c7f91e8a804`  
		Last Modified: Sat, 30 Apr 2022 01:24:52 GMT  
		Size: 85.8 MB (85752950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fb33950cdfb499758a2e2e0175d3276e1ae6192ed7475d2c797202ec587d50`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9282c1804e561e69e733ef8ff32d08b4c84e910b6d07682c107911599098a28`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840d845005b8287c568ff76130cc1c4f145b9dd2424a24fcfdcfb72eb8444234`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
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
$ docker pull mariadb@sha256:51fde652f9e71c731598f3faa7849fbae2a76ae50cdeec4449a3fd7d645bb0cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136560560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed495de503cba7f6e73bc47cf0dff842068da98768f39f008f01c6fc393b8d73`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:09:19 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:09:23 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:09:28 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:09:30 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:09:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:09:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:11:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:11:14 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:11:14 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:11:16 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:11:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:11:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:11:27 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:11:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d172f57c31273c2fd55f0cfbc9fa11f2ba1969befd541632c9e7b00db7565a`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4d6ee32d0879666223bed7d9a7de96bf0bd548fd6da30d40a4a2dbf9873e35`  
		Last Modified: Sat, 30 Apr 2022 01:24:10 GMT  
		Size: 90.3 MB (90346213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240c04ba26e43f570387de669839798b5b570a655a15ecb0a49e12070b8aafd4`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8de557e231927a4c3c9050f6404682dae66720d48d5180faa2eeff76bc52a0`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5c1ae5b4dab519c0622c267857cf414c7b17b9f81c3e90b88825878ab37a1`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:988c5e2073c8f9d49b4e2b8751d83839c53a5ae5f0a082450e9d0e83f359d45a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:31ffd93952ec8e67043b4442d399848781544508a5973ea4aef3a18478aa99c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c6c06541d48a629298ea6a58723be7712a6f866368018343adb914053e5602e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:19:32 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:19:32 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:19:32 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:19:32 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:19:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:19:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:20:00 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:20:00 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:20:01 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:20:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:20:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:20:01 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:20:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c653cb741960a71b44f4d61f043db04054ca6584d06fb1b7af5be93cf098ac50`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5571e050f105e60b660470785d52e7698eefaee024a561eaf62c7f91e8a804`  
		Last Modified: Sat, 30 Apr 2022 01:24:52 GMT  
		Size: 85.8 MB (85752950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fb33950cdfb499758a2e2e0175d3276e1ae6192ed7475d2c797202ec587d50`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9282c1804e561e69e733ef8ff32d08b4c84e910b6d07682c107911599098a28`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840d845005b8287c568ff76130cc1c4f145b9dd2424a24fcfdcfb72eb8444234`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
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
$ docker pull mariadb@sha256:51fde652f9e71c731598f3faa7849fbae2a76ae50cdeec4449a3fd7d645bb0cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136560560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed495de503cba7f6e73bc47cf0dff842068da98768f39f008f01c6fc393b8d73`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:09:19 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:09:23 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:09:28 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:09:30 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:09:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:09:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:11:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:11:14 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:11:14 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:11:16 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:11:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:11:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:11:27 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:11:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d172f57c31273c2fd55f0cfbc9fa11f2ba1969befd541632c9e7b00db7565a`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4d6ee32d0879666223bed7d9a7de96bf0bd548fd6da30d40a4a2dbf9873e35`  
		Last Modified: Sat, 30 Apr 2022 01:24:10 GMT  
		Size: 90.3 MB (90346213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240c04ba26e43f570387de669839798b5b570a655a15ecb0a49e12070b8aafd4`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8de557e231927a4c3c9050f6404682dae66720d48d5180faa2eeff76bc52a0`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5c1ae5b4dab519c0622c267857cf414c7b17b9f81c3e90b88825878ab37a1`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.24`

```console
$ docker pull mariadb@sha256:988c5e2073c8f9d49b4e2b8751d83839c53a5ae5f0a082450e9d0e83f359d45a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.24` - linux; amd64

```console
$ docker pull mariadb@sha256:31ffd93952ec8e67043b4442d399848781544508a5973ea4aef3a18478aa99c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c6c06541d48a629298ea6a58723be7712a6f866368018343adb914053e5602e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:19:32 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:19:32 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:19:32 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:19:32 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:19:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:19:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:20:00 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:20:00 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:20:01 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:20:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:20:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:20:01 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:20:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c653cb741960a71b44f4d61f043db04054ca6584d06fb1b7af5be93cf098ac50`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5571e050f105e60b660470785d52e7698eefaee024a561eaf62c7f91e8a804`  
		Last Modified: Sat, 30 Apr 2022 01:24:52 GMT  
		Size: 85.8 MB (85752950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fb33950cdfb499758a2e2e0175d3276e1ae6192ed7475d2c797202ec587d50`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9282c1804e561e69e733ef8ff32d08b4c84e910b6d07682c107911599098a28`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840d845005b8287c568ff76130cc1c4f145b9dd2424a24fcfdcfb72eb8444234`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
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
$ docker pull mariadb@sha256:51fde652f9e71c731598f3faa7849fbae2a76ae50cdeec4449a3fd7d645bb0cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136560560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed495de503cba7f6e73bc47cf0dff842068da98768f39f008f01c6fc393b8d73`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:09:19 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:09:23 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:09:28 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:09:30 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:09:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:09:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:11:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:11:14 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:11:14 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:11:16 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:11:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:11:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:11:27 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:11:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d172f57c31273c2fd55f0cfbc9fa11f2ba1969befd541632c9e7b00db7565a`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4d6ee32d0879666223bed7d9a7de96bf0bd548fd6da30d40a4a2dbf9873e35`  
		Last Modified: Sat, 30 Apr 2022 01:24:10 GMT  
		Size: 90.3 MB (90346213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240c04ba26e43f570387de669839798b5b570a655a15ecb0a49e12070b8aafd4`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8de557e231927a4c3c9050f6404682dae66720d48d5180faa2eeff76bc52a0`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5c1ae5b4dab519c0622c267857cf414c7b17b9f81c3e90b88825878ab37a1`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.24-focal`

```console
$ docker pull mariadb@sha256:988c5e2073c8f9d49b4e2b8751d83839c53a5ae5f0a082450e9d0e83f359d45a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.24-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:31ffd93952ec8e67043b4442d399848781544508a5973ea4aef3a18478aa99c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c6c06541d48a629298ea6a58723be7712a6f866368018343adb914053e5602e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:19:32 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:19:32 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:19:32 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:19:32 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:19:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:19:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:20:00 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:20:00 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:20:01 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:20:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:20:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:20:01 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:20:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c653cb741960a71b44f4d61f043db04054ca6584d06fb1b7af5be93cf098ac50`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5571e050f105e60b660470785d52e7698eefaee024a561eaf62c7f91e8a804`  
		Last Modified: Sat, 30 Apr 2022 01:24:52 GMT  
		Size: 85.8 MB (85752950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fb33950cdfb499758a2e2e0175d3276e1ae6192ed7475d2c797202ec587d50`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9282c1804e561e69e733ef8ff32d08b4c84e910b6d07682c107911599098a28`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
		Size: 6.8 KB (6772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840d845005b8287c568ff76130cc1c4f145b9dd2424a24fcfdcfb72eb8444234`  
		Last Modified: Sat, 30 Apr 2022 01:24:39 GMT  
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
$ docker pull mariadb@sha256:51fde652f9e71c731598f3faa7849fbae2a76ae50cdeec4449a3fd7d645bb0cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136560560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed495de503cba7f6e73bc47cf0dff842068da98768f39f008f01c6fc393b8d73`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:09:19 GMT
ARG MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:09:23 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 30 Apr 2022 01:09:28 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:09:30 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Sat, 30 Apr 2022 01:09:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:09:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:11:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:11:14 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:11:14 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:11:16 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:11:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 30 Apr 2022 01:11:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:11:27 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:11:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d172f57c31273c2fd55f0cfbc9fa11f2ba1969befd541632c9e7b00db7565a`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4d6ee32d0879666223bed7d9a7de96bf0bd548fd6da30d40a4a2dbf9873e35`  
		Last Modified: Sat, 30 Apr 2022 01:24:10 GMT  
		Size: 90.3 MB (90346213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240c04ba26e43f570387de669839798b5b570a655a15ecb0a49e12070b8aafd4`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8de557e231927a4c3c9050f6404682dae66720d48d5180faa2eeff76bc52a0`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 6.8 KB (6771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5c1ae5b4dab519c0622c267857cf414c7b17b9f81c3e90b88825878ab37a1`  
		Last Modified: Sat, 30 Apr 2022 01:23:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:eefee23fa1c4a04b267010b46e1c823b66453169917c7dd9bc2c22ea10ee2b9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:bca4e8ecce022e54a3c7439287e92fcda1e7e0f1e0e9a7134318636b0063fbf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127924188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c7d1ac0ae1b337f85eaa418fb7c16919f4d91f365184c4a1739a32ffb8d1f2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:18:58 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:18:58 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:18:58 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:18:59 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:18:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:18:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:19:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:19:25 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:19:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:19:25 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:19:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:19:25 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:19:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdad6338a726320c3708123e1d831615da54a9763efe7027c15d5047bb572067`  
		Last Modified: Sat, 30 Apr 2022 01:24:08 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9cbfcc60331b95392052f3104ad7c2542344620b53b0cc9169948f9f178086`  
		Last Modified: Sat, 30 Apr 2022 01:24:21 GMT  
		Size: 88.0 MB (87997359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54464abd2a4cf1a7c75c5102d4544daefd969d92d7f935890e7d0e0845bae32e`  
		Last Modified: Sat, 30 Apr 2022 01:24:08 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3613c950aa6edb60c0a29315b75b633a5b6cc6db53e498a0bba72464486a70d9`  
		Last Modified: Sat, 30 Apr 2022 01:24:08 GMT  
		Size: 6.8 KB (6773 bytes)  
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
$ docker pull mariadb@sha256:78aa79fe47b191e149303556ccb05c379112f56d3d2383ad6ea87df84442bb2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138782109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4b48af03c0aeb962f4a428a4db1523c45f8ec44f5a0b5831cb19b2f5775dc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:07:07 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:07:10 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:07:13 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:07:15 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:07:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:07:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:08:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:08:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:08:56 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:08:57 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:08:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:09:02 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:09:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba595f3f755e1a0be8332bddccd0968dce00bfc7cb34ca2977d60108d1252020`  
		Last Modified: Sat, 30 Apr 2022 01:23:13 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008c310140ef92ce1609d6f1f3b7d96ba431186fee0d8a6509e1f4277cc9cb2b`  
		Last Modified: Sat, 30 Apr 2022 01:23:31 GMT  
		Size: 92.6 MB (92567879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06ba3281b46add8d42725f838f300650465f0ac07f0f29ad6666c484e828841`  
		Last Modified: Sat, 30 Apr 2022 01:23:13 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd6f068dfdf03c9e67b84ea4edd2130e89418cbb314f5cfec4454ef9510cdb`  
		Last Modified: Sat, 30 Apr 2022 01:23:13 GMT  
		Size: 6.8 KB (6771 bytes)  
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
$ docker pull mariadb@sha256:eefee23fa1c4a04b267010b46e1c823b66453169917c7dd9bc2c22ea10ee2b9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:bca4e8ecce022e54a3c7439287e92fcda1e7e0f1e0e9a7134318636b0063fbf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127924188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c7d1ac0ae1b337f85eaa418fb7c16919f4d91f365184c4a1739a32ffb8d1f2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:18:58 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:18:58 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:18:58 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:18:59 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:18:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:18:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:19:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:19:25 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:19:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:19:25 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:19:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:19:25 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:19:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdad6338a726320c3708123e1d831615da54a9763efe7027c15d5047bb572067`  
		Last Modified: Sat, 30 Apr 2022 01:24:08 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9cbfcc60331b95392052f3104ad7c2542344620b53b0cc9169948f9f178086`  
		Last Modified: Sat, 30 Apr 2022 01:24:21 GMT  
		Size: 88.0 MB (87997359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54464abd2a4cf1a7c75c5102d4544daefd969d92d7f935890e7d0e0845bae32e`  
		Last Modified: Sat, 30 Apr 2022 01:24:08 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3613c950aa6edb60c0a29315b75b633a5b6cc6db53e498a0bba72464486a70d9`  
		Last Modified: Sat, 30 Apr 2022 01:24:08 GMT  
		Size: 6.8 KB (6773 bytes)  
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
$ docker pull mariadb@sha256:78aa79fe47b191e149303556ccb05c379112f56d3d2383ad6ea87df84442bb2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138782109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4b48af03c0aeb962f4a428a4db1523c45f8ec44f5a0b5831cb19b2f5775dc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:07:07 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:07:10 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:07:13 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:07:15 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:07:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:07:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:08:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:08:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:08:56 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:08:57 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:08:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:09:02 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:09:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba595f3f755e1a0be8332bddccd0968dce00bfc7cb34ca2977d60108d1252020`  
		Last Modified: Sat, 30 Apr 2022 01:23:13 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008c310140ef92ce1609d6f1f3b7d96ba431186fee0d8a6509e1f4277cc9cb2b`  
		Last Modified: Sat, 30 Apr 2022 01:23:31 GMT  
		Size: 92.6 MB (92567879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06ba3281b46add8d42725f838f300650465f0ac07f0f29ad6666c484e828841`  
		Last Modified: Sat, 30 Apr 2022 01:23:13 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd6f068dfdf03c9e67b84ea4edd2130e89418cbb314f5cfec4454ef9510cdb`  
		Last Modified: Sat, 30 Apr 2022 01:23:13 GMT  
		Size: 6.8 KB (6771 bytes)  
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
$ docker pull mariadb@sha256:eefee23fa1c4a04b267010b46e1c823b66453169917c7dd9bc2c22ea10ee2b9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.15` - linux; amd64

```console
$ docker pull mariadb@sha256:bca4e8ecce022e54a3c7439287e92fcda1e7e0f1e0e9a7134318636b0063fbf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127924188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c7d1ac0ae1b337f85eaa418fb7c16919f4d91f365184c4a1739a32ffb8d1f2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:18:58 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:18:58 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:18:58 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:18:59 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:18:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:18:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:19:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:19:25 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:19:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:19:25 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:19:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:19:25 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:19:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdad6338a726320c3708123e1d831615da54a9763efe7027c15d5047bb572067`  
		Last Modified: Sat, 30 Apr 2022 01:24:08 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9cbfcc60331b95392052f3104ad7c2542344620b53b0cc9169948f9f178086`  
		Last Modified: Sat, 30 Apr 2022 01:24:21 GMT  
		Size: 88.0 MB (87997359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54464abd2a4cf1a7c75c5102d4544daefd969d92d7f935890e7d0e0845bae32e`  
		Last Modified: Sat, 30 Apr 2022 01:24:08 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3613c950aa6edb60c0a29315b75b633a5b6cc6db53e498a0bba72464486a70d9`  
		Last Modified: Sat, 30 Apr 2022 01:24:08 GMT  
		Size: 6.8 KB (6773 bytes)  
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
$ docker pull mariadb@sha256:78aa79fe47b191e149303556ccb05c379112f56d3d2383ad6ea87df84442bb2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138782109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4b48af03c0aeb962f4a428a4db1523c45f8ec44f5a0b5831cb19b2f5775dc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:07:07 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:07:10 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:07:13 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:07:15 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:07:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:07:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:08:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:08:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:08:56 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:08:57 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:08:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:09:02 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:09:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba595f3f755e1a0be8332bddccd0968dce00bfc7cb34ca2977d60108d1252020`  
		Last Modified: Sat, 30 Apr 2022 01:23:13 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008c310140ef92ce1609d6f1f3b7d96ba431186fee0d8a6509e1f4277cc9cb2b`  
		Last Modified: Sat, 30 Apr 2022 01:23:31 GMT  
		Size: 92.6 MB (92567879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06ba3281b46add8d42725f838f300650465f0ac07f0f29ad6666c484e828841`  
		Last Modified: Sat, 30 Apr 2022 01:23:13 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd6f068dfdf03c9e67b84ea4edd2130e89418cbb314f5cfec4454ef9510cdb`  
		Last Modified: Sat, 30 Apr 2022 01:23:13 GMT  
		Size: 6.8 KB (6771 bytes)  
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
$ docker pull mariadb@sha256:eefee23fa1c4a04b267010b46e1c823b66453169917c7dd9bc2c22ea10ee2b9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.15-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:bca4e8ecce022e54a3c7439287e92fcda1e7e0f1e0e9a7134318636b0063fbf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127924188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c7d1ac0ae1b337f85eaa418fb7c16919f4d91f365184c4a1739a32ffb8d1f2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:18:58 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:18:58 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:18:58 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:18:59 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:18:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:18:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:19:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:19:25 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:19:25 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:19:25 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:19:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:19:25 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:19:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdad6338a726320c3708123e1d831615da54a9763efe7027c15d5047bb572067`  
		Last Modified: Sat, 30 Apr 2022 01:24:08 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9cbfcc60331b95392052f3104ad7c2542344620b53b0cc9169948f9f178086`  
		Last Modified: Sat, 30 Apr 2022 01:24:21 GMT  
		Size: 88.0 MB (87997359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54464abd2a4cf1a7c75c5102d4544daefd969d92d7f935890e7d0e0845bae32e`  
		Last Modified: Sat, 30 Apr 2022 01:24:08 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3613c950aa6edb60c0a29315b75b633a5b6cc6db53e498a0bba72464486a70d9`  
		Last Modified: Sat, 30 Apr 2022 01:24:08 GMT  
		Size: 6.8 KB (6773 bytes)  
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
$ docker pull mariadb@sha256:78aa79fe47b191e149303556ccb05c379112f56d3d2383ad6ea87df84442bb2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138782109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4b48af03c0aeb962f4a428a4db1523c45f8ec44f5a0b5831cb19b2f5775dc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:07:07 GMT
ARG MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:07:10 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 30 Apr 2022 01:07:13 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:07:15 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Sat, 30 Apr 2022 01:07:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:07:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:08:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:08:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:08:56 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:08:57 GMT
COPY file:c436b2c23059cf9de16997684da0d7d691080e3af50a8feff6f4c1ee6edfd4c3 in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:08:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:09:02 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:09:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba595f3f755e1a0be8332bddccd0968dce00bfc7cb34ca2977d60108d1252020`  
		Last Modified: Sat, 30 Apr 2022 01:23:13 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008c310140ef92ce1609d6f1f3b7d96ba431186fee0d8a6509e1f4277cc9cb2b`  
		Last Modified: Sat, 30 Apr 2022 01:23:31 GMT  
		Size: 92.6 MB (92567879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06ba3281b46add8d42725f838f300650465f0ac07f0f29ad6666c484e828841`  
		Last Modified: Sat, 30 Apr 2022 01:23:13 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd6f068dfdf03c9e67b84ea4edd2130e89418cbb314f5cfec4454ef9510cdb`  
		Last Modified: Sat, 30 Apr 2022 01:23:13 GMT  
		Size: 6.8 KB (6771 bytes)  
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
$ docker pull mariadb@sha256:9fb960cff340126826a2f395ccb3ae1c8ca9acc63603f477db9ca2b7e2eed744
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:97c7d6f1b0efedaa3ea9b9e3f66e0ee238702c12e9b276890e38bd071abe51ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128170182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a25dc0f17778b385ee12f40b5dadd398ec4fb710ccde51e7e4af2c9c5555d3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:18:30 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:18:30 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:18:30 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:18:30 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:18:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:18:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:55 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:55 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:18:55 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:18:56 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1109bea0ce095db6c774753a47ceba2450b4f3554b416c9aa7847cfb95da5d14`  
		Last Modified: Sat, 30 Apr 2022 01:23:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b208fdad78fb9492c1f7b3c74176e427e0787041009d2f70f34ad9c90be958`  
		Last Modified: Sat, 30 Apr 2022 01:23:52 GMT  
		Size: 88.2 MB (88243354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63854a3a9dece78e2df7318cb4e8cf17d0dc18d27da91f4a9fad8208a43c5c63`  
		Last Modified: Sat, 30 Apr 2022 01:23:39 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19cdb26b9529ade47bf241250a7665adcc6f1d1cdf6d7bc6494a67258c5c7d6`  
		Last Modified: Sat, 30 Apr 2022 01:23:39 GMT  
		Size: 6.8 KB (6774 bytes)  
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
$ docker pull mariadb@sha256:ad8ebc8263f67aa284a3101bee42c79e730299f1bd9922353baaa142d09ff49b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138841913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfc0e28bea657cd392ae393a7edb733fd1673cc0c7e794916c88aef3c9a6dfad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:04:26 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:04:31 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:04:34 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:04:35 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:04:37 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:04:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:06:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:06:42 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:06:43 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:06:45 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:06:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:06:48 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:06:50 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397f4cfe5ce3ea3e5e6ba310c8f6fde89c44fecfb3cad4fe99ce1c4ef379f32b`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1766a6253dfdf36500971b69b43944080134496e6e62848c460ec637f290314`  
		Last Modified: Sat, 30 Apr 2022 01:22:50 GMT  
		Size: 92.6 MB (92627684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2919c004f629af43b48f02efff9351fa9ea182a0bd93611a21e82081c1fbc`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319bcf6c65fe893eb0c506d853eacf3e55992a520cc1fb28d8a8c6a39869c39e`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 6.8 KB (6775 bytes)  
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
$ docker pull mariadb@sha256:9fb960cff340126826a2f395ccb3ae1c8ca9acc63603f477db9ca2b7e2eed744
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:97c7d6f1b0efedaa3ea9b9e3f66e0ee238702c12e9b276890e38bd071abe51ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128170182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a25dc0f17778b385ee12f40b5dadd398ec4fb710ccde51e7e4af2c9c5555d3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:18:30 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:18:30 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:18:30 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:18:30 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:18:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:18:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:55 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:55 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:18:55 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:18:56 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1109bea0ce095db6c774753a47ceba2450b4f3554b416c9aa7847cfb95da5d14`  
		Last Modified: Sat, 30 Apr 2022 01:23:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b208fdad78fb9492c1f7b3c74176e427e0787041009d2f70f34ad9c90be958`  
		Last Modified: Sat, 30 Apr 2022 01:23:52 GMT  
		Size: 88.2 MB (88243354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63854a3a9dece78e2df7318cb4e8cf17d0dc18d27da91f4a9fad8208a43c5c63`  
		Last Modified: Sat, 30 Apr 2022 01:23:39 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19cdb26b9529ade47bf241250a7665adcc6f1d1cdf6d7bc6494a67258c5c7d6`  
		Last Modified: Sat, 30 Apr 2022 01:23:39 GMT  
		Size: 6.8 KB (6774 bytes)  
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
$ docker pull mariadb@sha256:ad8ebc8263f67aa284a3101bee42c79e730299f1bd9922353baaa142d09ff49b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138841913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfc0e28bea657cd392ae393a7edb733fd1673cc0c7e794916c88aef3c9a6dfad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:04:26 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:04:31 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:04:34 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:04:35 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:04:37 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:04:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:06:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:06:42 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:06:43 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:06:45 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:06:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:06:48 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:06:50 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397f4cfe5ce3ea3e5e6ba310c8f6fde89c44fecfb3cad4fe99ce1c4ef379f32b`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1766a6253dfdf36500971b69b43944080134496e6e62848c460ec637f290314`  
		Last Modified: Sat, 30 Apr 2022 01:22:50 GMT  
		Size: 92.6 MB (92627684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2919c004f629af43b48f02efff9351fa9ea182a0bd93611a21e82081c1fbc`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319bcf6c65fe893eb0c506d853eacf3e55992a520cc1fb28d8a8c6a39869c39e`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 6.8 KB (6775 bytes)  
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
$ docker pull mariadb@sha256:9fb960cff340126826a2f395ccb3ae1c8ca9acc63603f477db9ca2b7e2eed744
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.7` - linux; amd64

```console
$ docker pull mariadb@sha256:97c7d6f1b0efedaa3ea9b9e3f66e0ee238702c12e9b276890e38bd071abe51ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128170182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a25dc0f17778b385ee12f40b5dadd398ec4fb710ccde51e7e4af2c9c5555d3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:18:30 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:18:30 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:18:30 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:18:30 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:18:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:18:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:55 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:55 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:18:55 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:18:56 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1109bea0ce095db6c774753a47ceba2450b4f3554b416c9aa7847cfb95da5d14`  
		Last Modified: Sat, 30 Apr 2022 01:23:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b208fdad78fb9492c1f7b3c74176e427e0787041009d2f70f34ad9c90be958`  
		Last Modified: Sat, 30 Apr 2022 01:23:52 GMT  
		Size: 88.2 MB (88243354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63854a3a9dece78e2df7318cb4e8cf17d0dc18d27da91f4a9fad8208a43c5c63`  
		Last Modified: Sat, 30 Apr 2022 01:23:39 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19cdb26b9529ade47bf241250a7665adcc6f1d1cdf6d7bc6494a67258c5c7d6`  
		Last Modified: Sat, 30 Apr 2022 01:23:39 GMT  
		Size: 6.8 KB (6774 bytes)  
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
$ docker pull mariadb@sha256:ad8ebc8263f67aa284a3101bee42c79e730299f1bd9922353baaa142d09ff49b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138841913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfc0e28bea657cd392ae393a7edb733fd1673cc0c7e794916c88aef3c9a6dfad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:04:26 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:04:31 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:04:34 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:04:35 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:04:37 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:04:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:06:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:06:42 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:06:43 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:06:45 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:06:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:06:48 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:06:50 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397f4cfe5ce3ea3e5e6ba310c8f6fde89c44fecfb3cad4fe99ce1c4ef379f32b`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1766a6253dfdf36500971b69b43944080134496e6e62848c460ec637f290314`  
		Last Modified: Sat, 30 Apr 2022 01:22:50 GMT  
		Size: 92.6 MB (92627684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2919c004f629af43b48f02efff9351fa9ea182a0bd93611a21e82081c1fbc`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319bcf6c65fe893eb0c506d853eacf3e55992a520cc1fb28d8a8c6a39869c39e`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 6.8 KB (6775 bytes)  
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
$ docker pull mariadb@sha256:9fb960cff340126826a2f395ccb3ae1c8ca9acc63603f477db9ca2b7e2eed744
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:97c7d6f1b0efedaa3ea9b9e3f66e0ee238702c12e9b276890e38bd071abe51ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128170182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a25dc0f17778b385ee12f40b5dadd398ec4fb710ccde51e7e4af2c9c5555d3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:18:30 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:18:30 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:18:30 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:18:30 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:18:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:18:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:55 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:55 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:55 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:18:55 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:18:56 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1109bea0ce095db6c774753a47ceba2450b4f3554b416c9aa7847cfb95da5d14`  
		Last Modified: Sat, 30 Apr 2022 01:23:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b208fdad78fb9492c1f7b3c74176e427e0787041009d2f70f34ad9c90be958`  
		Last Modified: Sat, 30 Apr 2022 01:23:52 GMT  
		Size: 88.2 MB (88243354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63854a3a9dece78e2df7318cb4e8cf17d0dc18d27da91f4a9fad8208a43c5c63`  
		Last Modified: Sat, 30 Apr 2022 01:23:39 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19cdb26b9529ade47bf241250a7665adcc6f1d1cdf6d7bc6494a67258c5c7d6`  
		Last Modified: Sat, 30 Apr 2022 01:23:39 GMT  
		Size: 6.8 KB (6774 bytes)  
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
$ docker pull mariadb@sha256:ad8ebc8263f67aa284a3101bee42c79e730299f1bd9922353baaa142d09ff49b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138841913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfc0e28bea657cd392ae393a7edb733fd1673cc0c7e794916c88aef3c9a6dfad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:04:26 GMT
ARG MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:04:31 GMT
ENV MARIADB_MAJOR=10.6
# Sat, 30 Apr 2022 01:04:34 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:04:35 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Sat, 30 Apr 2022 01:04:37 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:04:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:06:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:06:42 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:06:43 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:06:45 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:06:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:06:48 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:06:50 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397f4cfe5ce3ea3e5e6ba310c8f6fde89c44fecfb3cad4fe99ce1c4ef379f32b`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1766a6253dfdf36500971b69b43944080134496e6e62848c460ec637f290314`  
		Last Modified: Sat, 30 Apr 2022 01:22:50 GMT  
		Size: 92.6 MB (92627684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2919c004f629af43b48f02efff9351fa9ea182a0bd93611a21e82081c1fbc`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319bcf6c65fe893eb0c506d853eacf3e55992a520cc1fb28d8a8c6a39869c39e`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 6.8 KB (6775 bytes)  
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
$ docker pull mariadb@sha256:07e06f2e7ae9dfc63707a83130a62e00167c827f08fcac7a9aa33f4b6dc34e0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7` - linux; amd64

```console
$ docker pull mariadb@sha256:a252cb5322f288f0bbba2c289828db981ed4df92ecc35bce77881ec774982a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daf0f023c28d0a811ba382b5645b71cc771c49fd15d53b8075018fb15e677d05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:17:56 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:17:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:24 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:18:24 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:18:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c0075a397aba5c127769d6a6215111fd53df47f5c7b95491172709c21c210f`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a5800afaceb66771d7d7d5d6290e5dbb1cf69e96fa8cb9e218623d2d70178`  
		Last Modified: Sat, 30 Apr 2022 01:23:11 GMT  
		Size: 88.7 MB (88741718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27261e54ed45f6cf3697709e7fe0f23952ef5fd6123cefcadaf1f65296e72737`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18f8f832430d5c46086dbcd197ccdb6fe2ba4b1467e9e755ad2c6a8b205292`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
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
$ docker pull mariadb@sha256:9f0a93c25897df9a9b2ca3becf35fccdfd9531009c57b1481d8d027f8722dc49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139538393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9fdde589bdb89bddd62d2076c08de8ca866b15932b15f44b9809efd0a2c54d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:59:29 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:47 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:55 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:09 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:00:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:03:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:03:59 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:04:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:04:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:04:08 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:04:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38d1aea9df71e0e7b7a07ebbf73d3df047d6925b8517612731ce14b29d81e6f`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219c8b280b85bfcb106c1c23cb4f820d20c27c361c26bc4b7b20b972ae0e550d`  
		Last Modified: Sat, 30 Apr 2022 01:21:50 GMT  
		Size: 93.3 MB (93324167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca5c34dd9a2fb0cbcf95168f69c6aa33df79bce1e843d573af62fc0ca0bf60`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ec7c5c6f4af575453b8a299723e99a51c614cf4d411dc507c8c4970ecaf71`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 6.8 KB (6774 bytes)  
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
$ docker pull mariadb@sha256:07e06f2e7ae9dfc63707a83130a62e00167c827f08fcac7a9aa33f4b6dc34e0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:a252cb5322f288f0bbba2c289828db981ed4df92ecc35bce77881ec774982a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daf0f023c28d0a811ba382b5645b71cc771c49fd15d53b8075018fb15e677d05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:17:56 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:17:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:24 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:18:24 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:18:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c0075a397aba5c127769d6a6215111fd53df47f5c7b95491172709c21c210f`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a5800afaceb66771d7d7d5d6290e5dbb1cf69e96fa8cb9e218623d2d70178`  
		Last Modified: Sat, 30 Apr 2022 01:23:11 GMT  
		Size: 88.7 MB (88741718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27261e54ed45f6cf3697709e7fe0f23952ef5fd6123cefcadaf1f65296e72737`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18f8f832430d5c46086dbcd197ccdb6fe2ba4b1467e9e755ad2c6a8b205292`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
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
$ docker pull mariadb@sha256:9f0a93c25897df9a9b2ca3becf35fccdfd9531009c57b1481d8d027f8722dc49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139538393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9fdde589bdb89bddd62d2076c08de8ca866b15932b15f44b9809efd0a2c54d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:59:29 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:47 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:55 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:09 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:00:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:03:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:03:59 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:04:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:04:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:04:08 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:04:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38d1aea9df71e0e7b7a07ebbf73d3df047d6925b8517612731ce14b29d81e6f`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219c8b280b85bfcb106c1c23cb4f820d20c27c361c26bc4b7b20b972ae0e550d`  
		Last Modified: Sat, 30 Apr 2022 01:21:50 GMT  
		Size: 93.3 MB (93324167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca5c34dd9a2fb0cbcf95168f69c6aa33df79bce1e843d573af62fc0ca0bf60`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ec7c5c6f4af575453b8a299723e99a51c614cf4d411dc507c8c4970ecaf71`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 6.8 KB (6774 bytes)  
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
$ docker pull mariadb@sha256:07e06f2e7ae9dfc63707a83130a62e00167c827f08fcac7a9aa33f4b6dc34e0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.3` - linux; amd64

```console
$ docker pull mariadb@sha256:a252cb5322f288f0bbba2c289828db981ed4df92ecc35bce77881ec774982a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daf0f023c28d0a811ba382b5645b71cc771c49fd15d53b8075018fb15e677d05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:17:56 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:17:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:24 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:18:24 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:18:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c0075a397aba5c127769d6a6215111fd53df47f5c7b95491172709c21c210f`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a5800afaceb66771d7d7d5d6290e5dbb1cf69e96fa8cb9e218623d2d70178`  
		Last Modified: Sat, 30 Apr 2022 01:23:11 GMT  
		Size: 88.7 MB (88741718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27261e54ed45f6cf3697709e7fe0f23952ef5fd6123cefcadaf1f65296e72737`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18f8f832430d5c46086dbcd197ccdb6fe2ba4b1467e9e755ad2c6a8b205292`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
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
$ docker pull mariadb@sha256:9f0a93c25897df9a9b2ca3becf35fccdfd9531009c57b1481d8d027f8722dc49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139538393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9fdde589bdb89bddd62d2076c08de8ca866b15932b15f44b9809efd0a2c54d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:59:29 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:47 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:55 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:09 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:00:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:03:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:03:59 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:04:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:04:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:04:08 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:04:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38d1aea9df71e0e7b7a07ebbf73d3df047d6925b8517612731ce14b29d81e6f`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219c8b280b85bfcb106c1c23cb4f820d20c27c361c26bc4b7b20b972ae0e550d`  
		Last Modified: Sat, 30 Apr 2022 01:21:50 GMT  
		Size: 93.3 MB (93324167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca5c34dd9a2fb0cbcf95168f69c6aa33df79bce1e843d573af62fc0ca0bf60`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ec7c5c6f4af575453b8a299723e99a51c614cf4d411dc507c8c4970ecaf71`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 6.8 KB (6774 bytes)  
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
$ docker pull mariadb@sha256:07e06f2e7ae9dfc63707a83130a62e00167c827f08fcac7a9aa33f4b6dc34e0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:a252cb5322f288f0bbba2c289828db981ed4df92ecc35bce77881ec774982a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daf0f023c28d0a811ba382b5645b71cc771c49fd15d53b8075018fb15e677d05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:17:56 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:17:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:24 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:18:24 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:18:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c0075a397aba5c127769d6a6215111fd53df47f5c7b95491172709c21c210f`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a5800afaceb66771d7d7d5d6290e5dbb1cf69e96fa8cb9e218623d2d70178`  
		Last Modified: Sat, 30 Apr 2022 01:23:11 GMT  
		Size: 88.7 MB (88741718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27261e54ed45f6cf3697709e7fe0f23952ef5fd6123cefcadaf1f65296e72737`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18f8f832430d5c46086dbcd197ccdb6fe2ba4b1467e9e755ad2c6a8b205292`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
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
$ docker pull mariadb@sha256:9f0a93c25897df9a9b2ca3becf35fccdfd9531009c57b1481d8d027f8722dc49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139538393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9fdde589bdb89bddd62d2076c08de8ca866b15932b15f44b9809efd0a2c54d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:59:29 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:47 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:55 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:09 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:00:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:03:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:03:59 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:04:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:04:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:04:08 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:04:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38d1aea9df71e0e7b7a07ebbf73d3df047d6925b8517612731ce14b29d81e6f`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219c8b280b85bfcb106c1c23cb4f820d20c27c361c26bc4b7b20b972ae0e550d`  
		Last Modified: Sat, 30 Apr 2022 01:21:50 GMT  
		Size: 93.3 MB (93324167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca5c34dd9a2fb0cbcf95168f69c6aa33df79bce1e843d573af62fc0ca0bf60`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ec7c5c6f4af575453b8a299723e99a51c614cf4d411dc507c8c4970ecaf71`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 6.8 KB (6774 bytes)  
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
$ docker pull mariadb@sha256:36214a0d32b17241c59b9966123ad64aa856fd64b0705194141afd002f72f3ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:4415142fe915021c0db56834766fcb787e2894517674de64026da1a18fc8f020
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04eb8c05b24de2d0581955797400462bd23b5e3302c981eb934b9261a50325bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:17:16 GMT
ARG MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 01:17:16 GMT
ENV MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 01:17:16 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 01:17:16 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 01:17:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:17:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:17:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:17:48 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:17:48 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:17:48 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:17:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:17:48 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:17:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b424305f7024755ce7ad5bc0f5b349609ca2456df41bf3be0e63186bf059d`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cceffd624bc1cec34f970f083547faf548645f8ff892294f8fda2e05623894`  
		Last Modified: Sat, 30 Apr 2022 01:22:42 GMT  
		Size: 88.7 MB (88651844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c99300ba876c01c8df4bc535f9eaf53fe48709d075376af5d9ffc26333ea6ee`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88263bf2999c90ca605a1303e92744972fdeaa37320078090eccf5f07b80f11`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 6.8 KB (6776 bytes)  
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
$ docker pull mariadb@sha256:2ff6324e7031f6eaf425bfccd9c54ba7df32cdc316baded2dd11ffcfc3b2271f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139620503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c5b5ffc12cc645b0012916f56ca152507be891acb7da898b77bd01fa07bf670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:54:09 GMT
ARG MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:54:12 GMT
ENV MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:54:19 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:54:32 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:54:37 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:54:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:58:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:58:24 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:58:30 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:58:36 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:58:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:58:58 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:59:05 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653af7c27575f2ceffbcfa641fb0b9a4f8ece5cc5b539410aa1a5ba50627dce1`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39532867da8b3f965b7d43f5a9faf9e34b8635f029eaf9e4db744dfe4fcd52d7`  
		Last Modified: Sat, 30 Apr 2022 01:21:09 GMT  
		Size: 93.4 MB (93406273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597818766ffdc878d236ac547b19d7ad6a0d19004339b4a1f4169b69fddcf7f7`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465ffe791a92ca9f06192e9539610e566fb4be4b4e5634630944701c5f359eec`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 6.8 KB (6777 bytes)  
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
$ docker pull mariadb@sha256:36214a0d32b17241c59b9966123ad64aa856fd64b0705194141afd002f72f3ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-rc-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:4415142fe915021c0db56834766fcb787e2894517674de64026da1a18fc8f020
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04eb8c05b24de2d0581955797400462bd23b5e3302c981eb934b9261a50325bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:17:16 GMT
ARG MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 01:17:16 GMT
ENV MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 01:17:16 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 01:17:16 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 01:17:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:17:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:17:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:17:48 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:17:48 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:17:48 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:17:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:17:48 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:17:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b424305f7024755ce7ad5bc0f5b349609ca2456df41bf3be0e63186bf059d`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cceffd624bc1cec34f970f083547faf548645f8ff892294f8fda2e05623894`  
		Last Modified: Sat, 30 Apr 2022 01:22:42 GMT  
		Size: 88.7 MB (88651844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c99300ba876c01c8df4bc535f9eaf53fe48709d075376af5d9ffc26333ea6ee`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88263bf2999c90ca605a1303e92744972fdeaa37320078090eccf5f07b80f11`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 6.8 KB (6776 bytes)  
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
$ docker pull mariadb@sha256:2ff6324e7031f6eaf425bfccd9c54ba7df32cdc316baded2dd11ffcfc3b2271f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139620503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c5b5ffc12cc645b0012916f56ca152507be891acb7da898b77bd01fa07bf670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:54:09 GMT
ARG MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:54:12 GMT
ENV MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:54:19 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:54:32 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:54:37 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:54:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:58:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:58:24 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:58:30 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:58:36 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:58:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:58:58 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:59:05 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653af7c27575f2ceffbcfa641fb0b9a4f8ece5cc5b539410aa1a5ba50627dce1`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39532867da8b3f965b7d43f5a9faf9e34b8635f029eaf9e4db744dfe4fcd52d7`  
		Last Modified: Sat, 30 Apr 2022 01:21:09 GMT  
		Size: 93.4 MB (93406273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597818766ffdc878d236ac547b19d7ad6a0d19004339b4a1f4169b69fddcf7f7`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465ffe791a92ca9f06192e9539610e566fb4be4b4e5634630944701c5f359eec`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 6.8 KB (6777 bytes)  
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
$ docker pull mariadb@sha256:36214a0d32b17241c59b9966123ad64aa856fd64b0705194141afd002f72f3ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8.2-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:4415142fe915021c0db56834766fcb787e2894517674de64026da1a18fc8f020
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04eb8c05b24de2d0581955797400462bd23b5e3302c981eb934b9261a50325bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:17:16 GMT
ARG MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 01:17:16 GMT
ENV MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 01:17:16 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 01:17:16 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 01:17:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:17:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:17:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:17:48 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:17:48 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:17:48 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:17:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:17:48 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:17:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b424305f7024755ce7ad5bc0f5b349609ca2456df41bf3be0e63186bf059d`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cceffd624bc1cec34f970f083547faf548645f8ff892294f8fda2e05623894`  
		Last Modified: Sat, 30 Apr 2022 01:22:42 GMT  
		Size: 88.7 MB (88651844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c99300ba876c01c8df4bc535f9eaf53fe48709d075376af5d9ffc26333ea6ee`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88263bf2999c90ca605a1303e92744972fdeaa37320078090eccf5f07b80f11`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 6.8 KB (6776 bytes)  
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
$ docker pull mariadb@sha256:2ff6324e7031f6eaf425bfccd9c54ba7df32cdc316baded2dd11ffcfc3b2271f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139620503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c5b5ffc12cc645b0012916f56ca152507be891acb7da898b77bd01fa07bf670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:54:09 GMT
ARG MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:54:12 GMT
ENV MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:54:19 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:54:32 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:54:37 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:54:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:58:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:58:24 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:58:30 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:58:36 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:58:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:58:58 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:59:05 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653af7c27575f2ceffbcfa641fb0b9a4f8ece5cc5b539410aa1a5ba50627dce1`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39532867da8b3f965b7d43f5a9faf9e34b8635f029eaf9e4db744dfe4fcd52d7`  
		Last Modified: Sat, 30 Apr 2022 01:21:09 GMT  
		Size: 93.4 MB (93406273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597818766ffdc878d236ac547b19d7ad6a0d19004339b4a1f4169b69fddcf7f7`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465ffe791a92ca9f06192e9539610e566fb4be4b4e5634630944701c5f359eec`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 6.8 KB (6777 bytes)  
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
$ docker pull mariadb@sha256:36214a0d32b17241c59b9966123ad64aa856fd64b0705194141afd002f72f3ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8.2-rc-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:4415142fe915021c0db56834766fcb787e2894517674de64026da1a18fc8f020
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04eb8c05b24de2d0581955797400462bd23b5e3302c981eb934b9261a50325bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:17:16 GMT
ARG MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 01:17:16 GMT
ENV MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 01:17:16 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 01:17:16 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 01:17:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:17:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:17:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:17:48 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:17:48 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:17:48 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:17:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:17:48 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:17:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b424305f7024755ce7ad5bc0f5b349609ca2456df41bf3be0e63186bf059d`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cceffd624bc1cec34f970f083547faf548645f8ff892294f8fda2e05623894`  
		Last Modified: Sat, 30 Apr 2022 01:22:42 GMT  
		Size: 88.7 MB (88651844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c99300ba876c01c8df4bc535f9eaf53fe48709d075376af5d9ffc26333ea6ee`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88263bf2999c90ca605a1303e92744972fdeaa37320078090eccf5f07b80f11`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 6.8 KB (6776 bytes)  
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
$ docker pull mariadb@sha256:2ff6324e7031f6eaf425bfccd9c54ba7df32cdc316baded2dd11ffcfc3b2271f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139620503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c5b5ffc12cc645b0012916f56ca152507be891acb7da898b77bd01fa07bf670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:54:09 GMT
ARG MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:54:12 GMT
ENV MARIADB_MAJOR=10.8
# Sat, 30 Apr 2022 00:54:19 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:54:32 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Sat, 30 Apr 2022 00:54:37 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 00:54:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 00:58:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 00:58:24 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 00:58:30 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 00:58:36 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:58:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 00:58:58 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 00:59:05 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653af7c27575f2ceffbcfa641fb0b9a4f8ece5cc5b539410aa1a5ba50627dce1`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39532867da8b3f965b7d43f5a9faf9e34b8635f029eaf9e4db744dfe4fcd52d7`  
		Last Modified: Sat, 30 Apr 2022 01:21:09 GMT  
		Size: 93.4 MB (93406273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597818766ffdc878d236ac547b19d7ad6a0d19004339b4a1f4169b69fddcf7f7`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465ffe791a92ca9f06192e9539610e566fb4be4b4e5634630944701c5f359eec`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 6.8 KB (6777 bytes)  
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
$ docker pull mariadb@sha256:07e06f2e7ae9dfc63707a83130a62e00167c827f08fcac7a9aa33f4b6dc34e0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:a252cb5322f288f0bbba2c289828db981ed4df92ecc35bce77881ec774982a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daf0f023c28d0a811ba382b5645b71cc771c49fd15d53b8075018fb15e677d05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:17:56 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:17:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:24 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:18:24 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:18:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c0075a397aba5c127769d6a6215111fd53df47f5c7b95491172709c21c210f`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a5800afaceb66771d7d7d5d6290e5dbb1cf69e96fa8cb9e218623d2d70178`  
		Last Modified: Sat, 30 Apr 2022 01:23:11 GMT  
		Size: 88.7 MB (88741718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27261e54ed45f6cf3697709e7fe0f23952ef5fd6123cefcadaf1f65296e72737`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18f8f832430d5c46086dbcd197ccdb6fe2ba4b1467e9e755ad2c6a8b205292`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
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
$ docker pull mariadb@sha256:9f0a93c25897df9a9b2ca3becf35fccdfd9531009c57b1481d8d027f8722dc49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139538393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9fdde589bdb89bddd62d2076c08de8ca866b15932b15f44b9809efd0a2c54d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:59:29 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:47 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:55 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:09 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:00:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:03:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:03:59 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:04:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:04:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:04:08 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:04:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38d1aea9df71e0e7b7a07ebbf73d3df047d6925b8517612731ce14b29d81e6f`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219c8b280b85bfcb106c1c23cb4f820d20c27c361c26bc4b7b20b972ae0e550d`  
		Last Modified: Sat, 30 Apr 2022 01:21:50 GMT  
		Size: 93.3 MB (93324167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca5c34dd9a2fb0cbcf95168f69c6aa33df79bce1e843d573af62fc0ca0bf60`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ec7c5c6f4af575453b8a299723e99a51c614cf4d411dc507c8c4970ecaf71`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 6.8 KB (6774 bytes)  
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
$ docker pull mariadb@sha256:07e06f2e7ae9dfc63707a83130a62e00167c827f08fcac7a9aa33f4b6dc34e0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:a252cb5322f288f0bbba2c289828db981ed4df92ecc35bce77881ec774982a5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daf0f023c28d0a811ba382b5645b71cc771c49fd15d53b8075018fb15e677d05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:16:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 01:16:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:16:55 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 01:17:07 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 01:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 01:17:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:17:15 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 01:17:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 01:17:56 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 01:17:57 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:17:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:17:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:18:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:18:24 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:18:24 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:18:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:18:24 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:18:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b1cc1f34f74fc1ef5dd49efc65ab71f7cda8881fbd8440bb9714f33fe03295`  
		Last Modified: Sat, 30 Apr 2022 01:22:33 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924a2c30493a95ca3ce67ffd9aed8e190edc64a82297070c7378030a492d2f5`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 5.5 MB (5488600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb7d6219cef6538fe5475f4854cda05e2bb051f9e260d41dedf41505528663`  
		Last Modified: Sat, 30 Apr 2022 01:22:32 GMT  
		Size: 3.6 MB (3585003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2e9991ec911de9347a941d4ae56490b3826b5bdfacaa6df17443bc29369`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbaef7da8806ab739a844d813efff5f36b9c315efd17325aed5cda1754bd8c8`  
		Last Modified: Sat, 30 Apr 2022 01:22:31 GMT  
		Size: 2.3 MB (2272020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f39675d129096173bc4e513eee53078b5060609640d4caf4f19788a7025e07`  
		Last Modified: Sat, 30 Apr 2022 01:22:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c0075a397aba5c127769d6a6215111fd53df47f5c7b95491172709c21c210f`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a5800afaceb66771d7d7d5d6290e5dbb1cf69e96fa8cb9e218623d2d70178`  
		Last Modified: Sat, 30 Apr 2022 01:23:11 GMT  
		Size: 88.7 MB (88741718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27261e54ed45f6cf3697709e7fe0f23952ef5fd6123cefcadaf1f65296e72737`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b18f8f832430d5c46086dbcd197ccdb6fe2ba4b1467e9e755ad2c6a8b205292`  
		Last Modified: Sat, 30 Apr 2022 01:22:58 GMT  
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
$ docker pull mariadb@sha256:9f0a93c25897df9a9b2ca3becf35fccdfd9531009c57b1481d8d027f8722dc49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139538393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9fdde589bdb89bddd62d2076c08de8ca866b15932b15f44b9809efd0a2c54d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:50:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 30 Apr 2022 00:52:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:52:19 GMT
ENV GOSU_VERSION=1.14
# Sat, 30 Apr 2022 00:53:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 30 Apr 2022 00:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 30 Apr 2022 00:53:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:53:51 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 30 Apr 2022 00:54:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Sat, 30 Apr 2022 00:59:29 GMT
ARG MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:47 GMT
ENV MARIADB_MAJOR=10.7
# Sat, 30 Apr 2022 00:59:55 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:09 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Sat, 30 Apr 2022 01:00:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Sat, 30 Apr 2022 01:00:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 30 Apr 2022 01:03:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Sat, 30 Apr 2022 01:03:59 GMT
VOLUME [/var/lib/mysql]
# Sat, 30 Apr 2022 01:04:00 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Sat, 30 Apr 2022 01:04:02 GMT
COPY file:1e9733e3c770304d3250be6325e07d0f6b8ea7fd42808808cc6b2919d42a9a5e in /usr/local/bin/ 
# Sat, 30 Apr 2022 01:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Apr 2022 01:04:08 GMT
EXPOSE 3306
# Sat, 30 Apr 2022 01:04:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933fb2862e2716afd28ee38ed71eb9097a647fd38b4378b802ba4928e819c444`  
		Last Modified: Sat, 30 Apr 2022 01:20:57 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6899bc35ca339b1fbd966c280b0f1a2c3acd469ad358d3b3f48b1e6a1b7bd5`  
		Last Modified: Sat, 30 Apr 2022 01:20:56 GMT  
		Size: 6.7 MB (6667588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185278c53367843a392ed443f9de142076add930e26c0765cd604902e7e0026f`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 3.7 MB (3672592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d5cab0b98f71595c34fffd4c19a0d48f05279ac84eb9068b1090bafb87d6f`  
		Last Modified: Sat, 30 Apr 2022 01:20:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd37e664a57394de1d81b89e36f57a4318e77c9dcbd17a16966cc7924f323fa`  
		Last Modified: Sat, 30 Apr 2022 01:20:55 GMT  
		Size: 2.6 MB (2568397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc301781015b0c1df07f994700ffdfde0f31a2be7b1063ae698b5280f77aa5`  
		Last Modified: Sat, 30 Apr 2022 01:20:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38d1aea9df71e0e7b7a07ebbf73d3df047d6925b8517612731ce14b29d81e6f`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219c8b280b85bfcb106c1c23cb4f820d20c27c361c26bc4b7b20b972ae0e550d`  
		Last Modified: Sat, 30 Apr 2022 01:21:50 GMT  
		Size: 93.3 MB (93324167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca5c34dd9a2fb0cbcf95168f69c6aa33df79bce1e843d573af62fc0ca0bf60`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86ec7c5c6f4af575453b8a299723e99a51c614cf4d411dc507c8c4970ecaf71`  
		Last Modified: Sat, 30 Apr 2022 01:21:32 GMT  
		Size: 6.8 KB (6774 bytes)  
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
