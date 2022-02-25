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
-	[`mariadb:10.8`](#mariadb108)
-	[`mariadb:10.8-focal`](#mariadb108-focal)
-	[`mariadb:10.8.2`](#mariadb1082)
-	[`mariadb:10.8.2-focal`](#mariadb1082-focal)
-	[`mariadb:focal`](#mariadbfocal)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:9e1b5f318c0255eae6bb0877b0762c560cde9f7e6186f673060189761202615a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:0fed5d91ed5beb07acfb64b268e29d4c958b2692cba3911c596d6021537e5149
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539871f8c20e7bf54159322bfe2b3c25eddb9f6ff61074c1ceeb42c9c81d96d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:45:03 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 03:45:04 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 19:01:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:01:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:02:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:02:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:02:12 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:02:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caac2a47a26c1d5ac110c8c8160d78c46633c515fabc02aeead42a929abb3f34`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d95be4fc3ed23b3da3e0b23d8207ff984583950c9f475029a113d470656273`  
		Last Modified: Fri, 25 Feb 2022 19:07:50 GMT  
		Size: 88.7 MB (88742109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1a87df3e4e40283a0f746897cbb88bfbd00077e0fa0548901288ab4bf7eee`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f323680a6eb6da7bb7518c7bc1e4ea7ed5ee8ae6d9743a0ab57b622438a3b788`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:63aaeb42ea87e3fcd3dc9b95d351db22517700c92df3361c2dfc02a9e5a80b9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125723761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ffdf1c8b8c51c02922ad33ef21d0d10f9b90be60cf34707f4ec8d44b6cd03e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:41:18 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 04:41:19 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:40:56 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:40:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:41:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:41:27 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:41:29 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:41:30 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:41:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:41:31 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:41:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d5701620936a9434a752e612b26e7ef401d732951312b4cb3ba8e0d56624b6`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a445807beccaa6654d95ccc8bb6a1200f1e1254b7dbace6227db6d2ddcdcf6`  
		Last Modified: Fri, 25 Feb 2022 17:46:58 GMT  
		Size: 87.6 MB (87644355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c712675c67566e4c76372be2b231f84dc1b13f6085a0f37c58638c4468f0cac`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea1c89bb7bfd6f10e08bb4a0e0b25a8c7c515a62ce859975be7258b7bef85ed`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:26365cfc20ce97ce9359b32d5774b0cd623e503cd1dc0a5ddbc065b92fa9e70a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137783748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737496717e740b26172016c9c63dbeb5ae8ee2a178eb689b4f8a4c9176d37b99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:14:03 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 06:14:05 GMT
ENV MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 06:14:07 GMT
ARG MARIADB_VERSION=1:10.6.5+maria~focal
# Wed, 02 Feb 2022 06:14:08 GMT
ENV MARIADB_VERSION=1:10.6.5+maria~focal
# Wed, 02 Feb 2022 06:14:11 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:14:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:16:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:17:15 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:17:18 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:17:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:17:28 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:17:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4683b2a4076da23a58c3d55ec3193591331e38c1da0cd871cb108e31c76984ec`  
		Last Modified: Wed, 02 Feb 2022 06:39:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cedf38ea121b3c6203ec8682b97afed76dc9815da29af531bf48951ecbed21`  
		Last Modified: Wed, 02 Feb 2022 06:39:57 GMT  
		Size: 91.6 MB (91579209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca079698384d698aa1ec8a2a18c8458fbed546951d84d331a3d168d4dd4acba`  
		Last Modified: Wed, 02 Feb 2022 06:39:39 GMT  
		Size: 5.6 KB (5626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; s390x

```console
$ docker pull mariadb@sha256:86ecdcd726c86e5fdfd4a6e9d0806aa37120a54429b66fd9c4e917abc4fdc2fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127759644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c3482b60cba3773e4a8f8e0d1cdc804d03bb9b8e394a4cec25ab7f053d8b0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:01:20 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 02:01:20 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:42:33 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:42:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:58 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702f91bfef0abb95f814177f9a921283357b4afaa60cdb435acb8fe7a1402906`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543833eab2dd4901ece63b421429338ce5cca212daecd891f1ee2712a30b103`  
		Last Modified: Fri, 25 Feb 2022 17:45:35 GMT  
		Size: 89.8 MB (89815037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097c2f2236be70639eba7442cd4ceacf28eb6da74d1e88f4bef031bc88dd2150`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c175ac6918dcd13672765a8d1719eec85eeeca8fe4dffe912f427f6499d8d7`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 6.6 KB (6597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:9e1b5f318c0255eae6bb0877b0762c560cde9f7e6186f673060189761202615a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:0fed5d91ed5beb07acfb64b268e29d4c958b2692cba3911c596d6021537e5149
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539871f8c20e7bf54159322bfe2b3c25eddb9f6ff61074c1ceeb42c9c81d96d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:45:03 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 03:45:04 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 19:01:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:01:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:02:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:02:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:02:12 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:02:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caac2a47a26c1d5ac110c8c8160d78c46633c515fabc02aeead42a929abb3f34`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d95be4fc3ed23b3da3e0b23d8207ff984583950c9f475029a113d470656273`  
		Last Modified: Fri, 25 Feb 2022 19:07:50 GMT  
		Size: 88.7 MB (88742109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1a87df3e4e40283a0f746897cbb88bfbd00077e0fa0548901288ab4bf7eee`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f323680a6eb6da7bb7518c7bc1e4ea7ed5ee8ae6d9743a0ab57b622438a3b788`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:63aaeb42ea87e3fcd3dc9b95d351db22517700c92df3361c2dfc02a9e5a80b9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125723761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ffdf1c8b8c51c02922ad33ef21d0d10f9b90be60cf34707f4ec8d44b6cd03e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:41:18 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 04:41:19 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:40:56 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:40:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:41:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:41:27 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:41:29 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:41:30 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:41:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:41:31 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:41:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d5701620936a9434a752e612b26e7ef401d732951312b4cb3ba8e0d56624b6`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a445807beccaa6654d95ccc8bb6a1200f1e1254b7dbace6227db6d2ddcdcf6`  
		Last Modified: Fri, 25 Feb 2022 17:46:58 GMT  
		Size: 87.6 MB (87644355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c712675c67566e4c76372be2b231f84dc1b13f6085a0f37c58638c4468f0cac`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea1c89bb7bfd6f10e08bb4a0e0b25a8c7c515a62ce859975be7258b7bef85ed`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:26365cfc20ce97ce9359b32d5774b0cd623e503cd1dc0a5ddbc065b92fa9e70a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137783748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737496717e740b26172016c9c63dbeb5ae8ee2a178eb689b4f8a4c9176d37b99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:14:03 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 06:14:05 GMT
ENV MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 06:14:07 GMT
ARG MARIADB_VERSION=1:10.6.5+maria~focal
# Wed, 02 Feb 2022 06:14:08 GMT
ENV MARIADB_VERSION=1:10.6.5+maria~focal
# Wed, 02 Feb 2022 06:14:11 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:14:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:16:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:17:15 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:17:18 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:17:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:17:28 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:17:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4683b2a4076da23a58c3d55ec3193591331e38c1da0cd871cb108e31c76984ec`  
		Last Modified: Wed, 02 Feb 2022 06:39:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cedf38ea121b3c6203ec8682b97afed76dc9815da29af531bf48951ecbed21`  
		Last Modified: Wed, 02 Feb 2022 06:39:57 GMT  
		Size: 91.6 MB (91579209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca079698384d698aa1ec8a2a18c8458fbed546951d84d331a3d168d4dd4acba`  
		Last Modified: Wed, 02 Feb 2022 06:39:39 GMT  
		Size: 5.6 KB (5626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:86ecdcd726c86e5fdfd4a6e9d0806aa37120a54429b66fd9c4e917abc4fdc2fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127759644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c3482b60cba3773e4a8f8e0d1cdc804d03bb9b8e394a4cec25ab7f053d8b0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:01:20 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 02:01:20 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:42:33 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:42:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:58 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702f91bfef0abb95f814177f9a921283357b4afaa60cdb435acb8fe7a1402906`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543833eab2dd4901ece63b421429338ce5cca212daecd891f1ee2712a30b103`  
		Last Modified: Fri, 25 Feb 2022 17:45:35 GMT  
		Size: 89.8 MB (89815037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097c2f2236be70639eba7442cd4ceacf28eb6da74d1e88f4bef031bc88dd2150`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c175ac6918dcd13672765a8d1719eec85eeeca8fe4dffe912f427f6499d8d7`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 6.6 KB (6597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:43ff0618c8cc9ac788e96529d7526978a0e5e7c6d88ab8a50368386ca650bcb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:223648f62ed3f709232ed449274b571bc7dc3e31a2d020ce8002bb481ded99c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109314517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2fe61c51d112be6fe439cdd14714554b0413a9cf36940e6820f563f931ac2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:36 GMT
ADD file:c6039a4f004b6b6c2e4c281a228d64d8410cb9fdf0c67776f84bb173d3522be1 in / 
# Wed, 02 Feb 2022 02:14:36 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:48:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:48:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:48:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:48:36 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:48:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:48:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:48:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:49:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:49:21 GMT
ARG MARIADB_MAJOR=10.2
# Wed, 02 Feb 2022 03:49:21 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 25 Feb 2022 19:05:13 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 25 Feb 2022 19:05:13 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 25 Feb 2022 19:05:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 25 Feb 2022 19:05:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:06:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:06:07 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:06:07 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:06:07 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:06:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 19:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:06:09 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:68e7bb398b9ff421236990bfeaf5c1feab26c590eed93489e245375c23551e2a`  
		Last Modified: Sat, 29 Jan 2022 14:35:20 GMT  
		Size: 26.7 MB (26708066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07efdb86cae7e435924d7a9e50100f074c88cba99444bfff1d80715115980a97`  
		Last Modified: Wed, 02 Feb 2022 03:53:25 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060731bdf4df0f74621d939ac11c89e450590bf7c1dbfb105ac8b7f9c98f0955`  
		Last Modified: Wed, 02 Feb 2022 03:53:24 GMT  
		Size: 4.8 MB (4813104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f687d67df15eef4572ca1225fb9c265057a09f90f8d9feab521301db6a7edb9`  
		Last Modified: Wed, 02 Feb 2022 03:53:24 GMT  
		Size: 3.6 MB (3552933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323b153f8d8f0a953f57b7826a84da98ce091b402f27cb8a08c2863b34c02155`  
		Last Modified: Wed, 02 Feb 2022 03:53:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3694ff0bb5f01f872cf149cd4a44ade573695d2f8cc1e34fa78109cbc4e73e`  
		Last Modified: Wed, 02 Feb 2022 03:53:23 GMT  
		Size: 1.6 MB (1583439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be50f6f15fc5e2b073a82c355d1aa91461c24ef7587f679e9e701768123eaa9e`  
		Last Modified: Wed, 02 Feb 2022 03:53:21 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20894d37f30ec98e97246f995150981ff1fcf540ddd23e7683ae57094329ec6`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c43503ec3e128d0945557ae479c34330bdbd94ff8ac79261066d09d744f1125`  
		Last Modified: Fri, 25 Feb 2022 19:10:51 GMT  
		Size: 72.6 MB (72639284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fb4aa2e111d7114c503d64e520d7571b9a4ea7a91e10354808a2512e958092`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 3.5 KB (3457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4ba929c4a13c53a8f8b810b145ca525062a82389a2cc83332912d70a1cfccf`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 6.6 KB (6592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7036bda4af7b8bda44067121496ca6e9de1d1b56832c921a0f93353a7c33954e`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:037f2a18cf7603c2e0abcabbf473a47033e2844299afef52e9d75e25ac8daf98
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104236656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af1a2a8b723f2432291c45b98b044ae96240e022f39a8c8dd4907e7d684fdf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:18 GMT
ADD file:6c6588e8deb686903374087994742c9d5e77393babbbffd56aea9d4e6c888aa7 in / 
# Wed, 02 Feb 2022 03:19:18 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:52:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:52:53 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:52:54 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:53:16 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:53:32 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:53:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:54:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:54:11 GMT
ARG MARIADB_MAJOR=10.2
# Wed, 02 Feb 2022 04:54:12 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 02 Feb 2022 04:54:13 GMT
ARG MARIADB_VERSION=1:10.2.41+maria~bionic
# Wed, 02 Feb 2022 04:54:14 GMT
ENV MARIADB_VERSION=1:10.2.41+maria~bionic
# Wed, 02 Feb 2022 04:54:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
# Wed, 02 Feb 2022 04:54:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 04:56:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 04:56:24 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 04:56:26 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 04:56:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 02 Feb 2022 04:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 04:56:28 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 04:56:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:02b7ffdbddc71205d24598c17b9c600df7cc8d35fb49e550250299ce97e1c96e`  
		Last Modified: Wed, 02 Feb 2022 03:21:06 GMT  
		Size: 23.7 MB (23729736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324d51d5555b0be323004789a04cced02ff0e994d6f064b233ba55f2726783a5`  
		Last Modified: Wed, 02 Feb 2022 05:00:54 GMT  
		Size: 1.9 KB (1851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41f080fb063742c7cdc76ad616a47481da1dedcb1af5c6f33945940fdd731ab`  
		Last Modified: Wed, 02 Feb 2022 05:00:52 GMT  
		Size: 4.3 MB (4261558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bf986fb556112d7708edf0691efbf12e3c96272d66d64a23f482fed60196b1`  
		Last Modified: Wed, 02 Feb 2022 05:00:52 GMT  
		Size: 3.2 MB (3207341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f4aef644fe2bd25dd2f14a2d5c045c287b4ecb29b20b230570f72556d3eb03`  
		Last Modified: Wed, 02 Feb 2022 05:00:51 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243e84742e7b6d15fc971bd7866e82c5199dd4fd6974c566d30acb0d11cc536`  
		Last Modified: Wed, 02 Feb 2022 05:00:52 GMT  
		Size: 1.5 MB (1529550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53ce770cae28b46d4ac524f9bd2cc33d3addc94350747a5a75a2a16346bdbe2`  
		Last Modified: Wed, 02 Feb 2022 05:00:49 GMT  
		Size: 5.1 KB (5147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1a1e628afb1ef1aaf8495a07d9404153bfc33f67f1abd15d77c2a747817660`  
		Last Modified: Wed, 02 Feb 2022 05:00:49 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b429f0258d8be046f3dd1d898cd67cc76fc03b6f3c22de3210b231b80a38eab`  
		Last Modified: Wed, 02 Feb 2022 05:01:00 GMT  
		Size: 71.5 MB (71495285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c683bd532a9dd067683f9b4b93037c1e5603affbee76a346e0a9dc2e0b268ef6`  
		Last Modified: Wed, 02 Feb 2022 05:00:49 GMT  
		Size: 5.6 KB (5626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb263c423a2c8a3ed22929cdd18072d3a484d1900e88c05419216ea19d8e763`  
		Last Modified: Wed, 02 Feb 2022 05:00:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e958613c57ccbf4e8768d163d6957ba27059861f569d6d112b92e5653a98fe65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117704061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e8c49875d8331251cd8570bfe137e21fd43ad3159d8d18147c469ca3b0a79b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:49:58 GMT
ADD file:19b6b516bfde37805273abae0012aaceb45030dcc0c1dbc11828a4dfa6549c29 in / 
# Wed, 02 Feb 2022 03:50:03 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:29:38 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:31:37 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:31:41 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:32:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:32:52 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:33:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:33:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:34:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:34:19 GMT
ARG MARIADB_MAJOR=10.2
# Wed, 02 Feb 2022 06:34:23 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 02 Feb 2022 06:34:26 GMT
ARG MARIADB_VERSION=1:10.2.41+maria~bionic
# Wed, 02 Feb 2022 06:34:31 GMT
ENV MARIADB_VERSION=1:10.2.41+maria~bionic
# Wed, 02 Feb 2022 06:34:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
# Wed, 02 Feb 2022 06:34:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:37:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:37:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:37:32 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:37:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 02 Feb 2022 06:37:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:37:48 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:37:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1dc99fe180768d17487534d27fca7d2aea3e7473c284314a65af7be77144eeaa`  
		Last Modified: Wed, 02 Feb 2022 03:52:51 GMT  
		Size: 30.4 MB (30437685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3793cab5129185e888d0cee887241418d1ab6bc8f9732c017ce237abf9ba603f`  
		Last Modified: Wed, 02 Feb 2022 06:42:30 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f854f2b0750783f2c07f28d4092d70b3f72c8cacbc291ccabaf20c127e4a8197`  
		Last Modified: Wed, 02 Feb 2022 06:42:28 GMT  
		Size: 5.6 MB (5630392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd0ff847987b2597bfce989e412181c3a87e74caf26341386b3e44512468fce`  
		Last Modified: Wed, 02 Feb 2022 06:42:28 GMT  
		Size: 3.5 MB (3533539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e94deaa3d6268f01abfaad4b94e150724f7ccde85fdc38aaedbc56aa82a33a`  
		Last Modified: Wed, 02 Feb 2022 06:42:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2fd884dff08b0b653b850c03d468bc1f5e8e12118d26593d7e1536f8c067b0`  
		Last Modified: Wed, 02 Feb 2022 06:42:27 GMT  
		Size: 1.9 MB (1936987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a364db5113e11c5a0ab07dc75a3015c70ad00c20c361a8229ff1fc89125b2e1`  
		Last Modified: Wed, 02 Feb 2022 06:42:24 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8eea891be4608f10efd1189eced892aa2a3f9f106ca6b915b601f6dc97819f`  
		Last Modified: Wed, 02 Feb 2022 06:42:24 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0f079ad3feda07854f4daea77cbbce606947624731953c8d3a32ff1f6ecd28`  
		Last Modified: Wed, 02 Feb 2022 06:42:39 GMT  
		Size: 76.2 MB (76152173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226296a8caaf21598031e74515460ed40cc4517ef7d0b9fbc0af24e31881f1d9`  
		Last Modified: Wed, 02 Feb 2022 06:42:24 GMT  
		Size: 5.6 KB (5627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0dd6375913a29fac6d04e896628cfb3858ae0756379cb88439e4628434739b`  
		Last Modified: Wed, 02 Feb 2022 06:42:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:43ff0618c8cc9ac788e96529d7526978a0e5e7c6d88ab8a50368386ca650bcb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:223648f62ed3f709232ed449274b571bc7dc3e31a2d020ce8002bb481ded99c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109314517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2fe61c51d112be6fe439cdd14714554b0413a9cf36940e6820f563f931ac2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:36 GMT
ADD file:c6039a4f004b6b6c2e4c281a228d64d8410cb9fdf0c67776f84bb173d3522be1 in / 
# Wed, 02 Feb 2022 02:14:36 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:48:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:48:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:48:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:48:36 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:48:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:48:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:48:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:49:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:49:21 GMT
ARG MARIADB_MAJOR=10.2
# Wed, 02 Feb 2022 03:49:21 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 25 Feb 2022 19:05:13 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 25 Feb 2022 19:05:13 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 25 Feb 2022 19:05:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 25 Feb 2022 19:05:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:06:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:06:07 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:06:07 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:06:07 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:06:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 19:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:06:09 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:68e7bb398b9ff421236990bfeaf5c1feab26c590eed93489e245375c23551e2a`  
		Last Modified: Sat, 29 Jan 2022 14:35:20 GMT  
		Size: 26.7 MB (26708066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07efdb86cae7e435924d7a9e50100f074c88cba99444bfff1d80715115980a97`  
		Last Modified: Wed, 02 Feb 2022 03:53:25 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060731bdf4df0f74621d939ac11c89e450590bf7c1dbfb105ac8b7f9c98f0955`  
		Last Modified: Wed, 02 Feb 2022 03:53:24 GMT  
		Size: 4.8 MB (4813104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f687d67df15eef4572ca1225fb9c265057a09f90f8d9feab521301db6a7edb9`  
		Last Modified: Wed, 02 Feb 2022 03:53:24 GMT  
		Size: 3.6 MB (3552933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323b153f8d8f0a953f57b7826a84da98ce091b402f27cb8a08c2863b34c02155`  
		Last Modified: Wed, 02 Feb 2022 03:53:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3694ff0bb5f01f872cf149cd4a44ade573695d2f8cc1e34fa78109cbc4e73e`  
		Last Modified: Wed, 02 Feb 2022 03:53:23 GMT  
		Size: 1.6 MB (1583439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be50f6f15fc5e2b073a82c355d1aa91461c24ef7587f679e9e701768123eaa9e`  
		Last Modified: Wed, 02 Feb 2022 03:53:21 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20894d37f30ec98e97246f995150981ff1fcf540ddd23e7683ae57094329ec6`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c43503ec3e128d0945557ae479c34330bdbd94ff8ac79261066d09d744f1125`  
		Last Modified: Fri, 25 Feb 2022 19:10:51 GMT  
		Size: 72.6 MB (72639284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fb4aa2e111d7114c503d64e520d7571b9a4ea7a91e10354808a2512e958092`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 3.5 KB (3457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4ba929c4a13c53a8f8b810b145ca525062a82389a2cc83332912d70a1cfccf`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 6.6 KB (6592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7036bda4af7b8bda44067121496ca6e9de1d1b56832c921a0f93353a7c33954e`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:037f2a18cf7603c2e0abcabbf473a47033e2844299afef52e9d75e25ac8daf98
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104236656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af1a2a8b723f2432291c45b98b044ae96240e022f39a8c8dd4907e7d684fdf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:18 GMT
ADD file:6c6588e8deb686903374087994742c9d5e77393babbbffd56aea9d4e6c888aa7 in / 
# Wed, 02 Feb 2022 03:19:18 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:52:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:52:53 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:52:54 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:53:16 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:53:32 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:53:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:54:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:54:11 GMT
ARG MARIADB_MAJOR=10.2
# Wed, 02 Feb 2022 04:54:12 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 02 Feb 2022 04:54:13 GMT
ARG MARIADB_VERSION=1:10.2.41+maria~bionic
# Wed, 02 Feb 2022 04:54:14 GMT
ENV MARIADB_VERSION=1:10.2.41+maria~bionic
# Wed, 02 Feb 2022 04:54:15 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
# Wed, 02 Feb 2022 04:54:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 04:56:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 04:56:24 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 04:56:26 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 04:56:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 02 Feb 2022 04:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 04:56:28 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 04:56:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:02b7ffdbddc71205d24598c17b9c600df7cc8d35fb49e550250299ce97e1c96e`  
		Last Modified: Wed, 02 Feb 2022 03:21:06 GMT  
		Size: 23.7 MB (23729736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324d51d5555b0be323004789a04cced02ff0e994d6f064b233ba55f2726783a5`  
		Last Modified: Wed, 02 Feb 2022 05:00:54 GMT  
		Size: 1.9 KB (1851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41f080fb063742c7cdc76ad616a47481da1dedcb1af5c6f33945940fdd731ab`  
		Last Modified: Wed, 02 Feb 2022 05:00:52 GMT  
		Size: 4.3 MB (4261558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bf986fb556112d7708edf0691efbf12e3c96272d66d64a23f482fed60196b1`  
		Last Modified: Wed, 02 Feb 2022 05:00:52 GMT  
		Size: 3.2 MB (3207341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f4aef644fe2bd25dd2f14a2d5c045c287b4ecb29b20b230570f72556d3eb03`  
		Last Modified: Wed, 02 Feb 2022 05:00:51 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243e84742e7b6d15fc971bd7866e82c5199dd4fd6974c566d30acb0d11cc536`  
		Last Modified: Wed, 02 Feb 2022 05:00:52 GMT  
		Size: 1.5 MB (1529550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53ce770cae28b46d4ac524f9bd2cc33d3addc94350747a5a75a2a16346bdbe2`  
		Last Modified: Wed, 02 Feb 2022 05:00:49 GMT  
		Size: 5.1 KB (5147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1a1e628afb1ef1aaf8495a07d9404153bfc33f67f1abd15d77c2a747817660`  
		Last Modified: Wed, 02 Feb 2022 05:00:49 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b429f0258d8be046f3dd1d898cd67cc76fc03b6f3c22de3210b231b80a38eab`  
		Last Modified: Wed, 02 Feb 2022 05:01:00 GMT  
		Size: 71.5 MB (71495285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c683bd532a9dd067683f9b4b93037c1e5603affbee76a346e0a9dc2e0b268ef6`  
		Last Modified: Wed, 02 Feb 2022 05:00:49 GMT  
		Size: 5.6 KB (5626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb263c423a2c8a3ed22929cdd18072d3a484d1900e88c05419216ea19d8e763`  
		Last Modified: Wed, 02 Feb 2022 05:00:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e958613c57ccbf4e8768d163d6957ba27059861f569d6d112b92e5653a98fe65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117704061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e8c49875d8331251cd8570bfe137e21fd43ad3159d8d18147c469ca3b0a79b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:49:58 GMT
ADD file:19b6b516bfde37805273abae0012aaceb45030dcc0c1dbc11828a4dfa6549c29 in / 
# Wed, 02 Feb 2022 03:50:03 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:29:38 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:31:37 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:31:41 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:32:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:32:52 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:33:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:33:29 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:34:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:34:19 GMT
ARG MARIADB_MAJOR=10.2
# Wed, 02 Feb 2022 06:34:23 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 02 Feb 2022 06:34:26 GMT
ARG MARIADB_VERSION=1:10.2.41+maria~bionic
# Wed, 02 Feb 2022 06:34:31 GMT
ENV MARIADB_VERSION=1:10.2.41+maria~bionic
# Wed, 02 Feb 2022 06:34:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
# Wed, 02 Feb 2022 06:34:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:37:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:37:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:37:32 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:37:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.41/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 02 Feb 2022 06:37:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:37:48 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:37:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1dc99fe180768d17487534d27fca7d2aea3e7473c284314a65af7be77144eeaa`  
		Last Modified: Wed, 02 Feb 2022 03:52:51 GMT  
		Size: 30.4 MB (30437685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3793cab5129185e888d0cee887241418d1ab6bc8f9732c017ce237abf9ba603f`  
		Last Modified: Wed, 02 Feb 2022 06:42:30 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f854f2b0750783f2c07f28d4092d70b3f72c8cacbc291ccabaf20c127e4a8197`  
		Last Modified: Wed, 02 Feb 2022 06:42:28 GMT  
		Size: 5.6 MB (5630392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd0ff847987b2597bfce989e412181c3a87e74caf26341386b3e44512468fce`  
		Last Modified: Wed, 02 Feb 2022 06:42:28 GMT  
		Size: 3.5 MB (3533539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e94deaa3d6268f01abfaad4b94e150724f7ccde85fdc38aaedbc56aa82a33a`  
		Last Modified: Wed, 02 Feb 2022 06:42:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2fd884dff08b0b653b850c03d468bc1f5e8e12118d26593d7e1536f8c067b0`  
		Last Modified: Wed, 02 Feb 2022 06:42:27 GMT  
		Size: 1.9 MB (1936987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a364db5113e11c5a0ab07dc75a3015c70ad00c20c361a8229ff1fc89125b2e1`  
		Last Modified: Wed, 02 Feb 2022 06:42:24 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8eea891be4608f10efd1189eced892aa2a3f9f106ca6b915b601f6dc97819f`  
		Last Modified: Wed, 02 Feb 2022 06:42:24 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0f079ad3feda07854f4daea77cbbce606947624731953c8d3a32ff1f6ecd28`  
		Last Modified: Wed, 02 Feb 2022 06:42:39 GMT  
		Size: 76.2 MB (76152173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226296a8caaf21598031e74515460ed40cc4517ef7d0b9fbc0af24e31881f1d9`  
		Last Modified: Wed, 02 Feb 2022 06:42:24 GMT  
		Size: 5.6 KB (5627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0dd6375913a29fac6d04e896628cfb3858ae0756379cb88439e4628434739b`  
		Last Modified: Wed, 02 Feb 2022 06:42:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.43`

```console
$ docker pull mariadb@sha256:33024b58198fa53bcb0cea6bb454cac0629eb9430a1d673c38a8138d274cb1b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mariadb:10.2.43` - linux; amd64

```console
$ docker pull mariadb@sha256:223648f62ed3f709232ed449274b571bc7dc3e31a2d020ce8002bb481ded99c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109314517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2fe61c51d112be6fe439cdd14714554b0413a9cf36940e6820f563f931ac2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:36 GMT
ADD file:c6039a4f004b6b6c2e4c281a228d64d8410cb9fdf0c67776f84bb173d3522be1 in / 
# Wed, 02 Feb 2022 02:14:36 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:48:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:48:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:48:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:48:36 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:48:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:48:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:48:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:49:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:49:21 GMT
ARG MARIADB_MAJOR=10.2
# Wed, 02 Feb 2022 03:49:21 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 25 Feb 2022 19:05:13 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 25 Feb 2022 19:05:13 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 25 Feb 2022 19:05:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 25 Feb 2022 19:05:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:06:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:06:07 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:06:07 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:06:07 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:06:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 19:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:06:09 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:68e7bb398b9ff421236990bfeaf5c1feab26c590eed93489e245375c23551e2a`  
		Last Modified: Sat, 29 Jan 2022 14:35:20 GMT  
		Size: 26.7 MB (26708066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07efdb86cae7e435924d7a9e50100f074c88cba99444bfff1d80715115980a97`  
		Last Modified: Wed, 02 Feb 2022 03:53:25 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060731bdf4df0f74621d939ac11c89e450590bf7c1dbfb105ac8b7f9c98f0955`  
		Last Modified: Wed, 02 Feb 2022 03:53:24 GMT  
		Size: 4.8 MB (4813104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f687d67df15eef4572ca1225fb9c265057a09f90f8d9feab521301db6a7edb9`  
		Last Modified: Wed, 02 Feb 2022 03:53:24 GMT  
		Size: 3.6 MB (3552933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323b153f8d8f0a953f57b7826a84da98ce091b402f27cb8a08c2863b34c02155`  
		Last Modified: Wed, 02 Feb 2022 03:53:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3694ff0bb5f01f872cf149cd4a44ade573695d2f8cc1e34fa78109cbc4e73e`  
		Last Modified: Wed, 02 Feb 2022 03:53:23 GMT  
		Size: 1.6 MB (1583439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be50f6f15fc5e2b073a82c355d1aa91461c24ef7587f679e9e701768123eaa9e`  
		Last Modified: Wed, 02 Feb 2022 03:53:21 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20894d37f30ec98e97246f995150981ff1fcf540ddd23e7683ae57094329ec6`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c43503ec3e128d0945557ae479c34330bdbd94ff8ac79261066d09d744f1125`  
		Last Modified: Fri, 25 Feb 2022 19:10:51 GMT  
		Size: 72.6 MB (72639284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fb4aa2e111d7114c503d64e520d7571b9a4ea7a91e10354808a2512e958092`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 3.5 KB (3457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4ba929c4a13c53a8f8b810b145ca525062a82389a2cc83332912d70a1cfccf`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 6.6 KB (6592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7036bda4af7b8bda44067121496ca6e9de1d1b56832c921a0f93353a7c33954e`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.43-bionic`

```console
$ docker pull mariadb@sha256:33024b58198fa53bcb0cea6bb454cac0629eb9430a1d673c38a8138d274cb1b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mariadb:10.2.43-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:223648f62ed3f709232ed449274b571bc7dc3e31a2d020ce8002bb481ded99c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109314517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2fe61c51d112be6fe439cdd14714554b0413a9cf36940e6820f563f931ac2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:36 GMT
ADD file:c6039a4f004b6b6c2e4c281a228d64d8410cb9fdf0c67776f84bb173d3522be1 in / 
# Wed, 02 Feb 2022 02:14:36 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:48:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:48:22 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:48:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:48:36 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:48:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:48:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:48:45 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:49:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:49:21 GMT
ARG MARIADB_MAJOR=10.2
# Wed, 02 Feb 2022 03:49:21 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 25 Feb 2022 19:05:13 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 25 Feb 2022 19:05:13 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 25 Feb 2022 19:05:13 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 25 Feb 2022 19:05:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:06:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:06:07 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:06:07 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:06:07 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:06:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 19:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:06:09 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:68e7bb398b9ff421236990bfeaf5c1feab26c590eed93489e245375c23551e2a`  
		Last Modified: Sat, 29 Jan 2022 14:35:20 GMT  
		Size: 26.7 MB (26708066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07efdb86cae7e435924d7a9e50100f074c88cba99444bfff1d80715115980a97`  
		Last Modified: Wed, 02 Feb 2022 03:53:25 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060731bdf4df0f74621d939ac11c89e450590bf7c1dbfb105ac8b7f9c98f0955`  
		Last Modified: Wed, 02 Feb 2022 03:53:24 GMT  
		Size: 4.8 MB (4813104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f687d67df15eef4572ca1225fb9c265057a09f90f8d9feab521301db6a7edb9`  
		Last Modified: Wed, 02 Feb 2022 03:53:24 GMT  
		Size: 3.6 MB (3552933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323b153f8d8f0a953f57b7826a84da98ce091b402f27cb8a08c2863b34c02155`  
		Last Modified: Wed, 02 Feb 2022 03:53:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3694ff0bb5f01f872cf149cd4a44ade573695d2f8cc1e34fa78109cbc4e73e`  
		Last Modified: Wed, 02 Feb 2022 03:53:23 GMT  
		Size: 1.6 MB (1583439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be50f6f15fc5e2b073a82c355d1aa91461c24ef7587f679e9e701768123eaa9e`  
		Last Modified: Wed, 02 Feb 2022 03:53:21 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20894d37f30ec98e97246f995150981ff1fcf540ddd23e7683ae57094329ec6`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c43503ec3e128d0945557ae479c34330bdbd94ff8ac79261066d09d744f1125`  
		Last Modified: Fri, 25 Feb 2022 19:10:51 GMT  
		Size: 72.6 MB (72639284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fb4aa2e111d7114c503d64e520d7571b9a4ea7a91e10354808a2512e958092`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 3.5 KB (3457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4ba929c4a13c53a8f8b810b145ca525062a82389a2cc83332912d70a1cfccf`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 6.6 KB (6592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7036bda4af7b8bda44067121496ca6e9de1d1b56832c921a0f93353a7c33954e`  
		Last Modified: Fri, 25 Feb 2022 19:10:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:fcbed9f7f550d256ec987502fbfd01513ac365ff10ff989e39e36b87b0431056
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:5ff563719b69c13176d018523117206ed0928c3a15ea4547618c14eb493d2fa8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120117250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9c4d949b520a3bda2d53cc35b87df84af0655aade4c6a4b77cc86bcece148f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:47:26 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 02 Feb 2022 03:47:26 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 25 Feb 2022 19:04:24 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 19:04:24 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 19:04:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:04:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:04:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:05:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:05:00 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:05:01 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:05:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 19:05:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:05:03 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:05:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09068eced0b633eec0c4c85f6e82fb884de56a7285f4d36b3504a6d72fa23731`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf18bfce1213ed3f88c5333e6112a6cba219ecf61b0f8dc45a9b87a166ecac2`  
		Last Modified: Fri, 25 Feb 2022 19:10:17 GMT  
		Size: 80.2 MB (80191098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e703ab2dfb1ebabf11b526ea6418cc872fde0e9228699534ca6502316f429f5`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdbba010e4a1689eccb4971867b3ba3a08564e795ec18a5e3c34e415cee1706`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 6.6 KB (6591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472da57979151992035cff2e784a9c871aaef0799eb0ca04a3a3f7ccf8b5777`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:a400461e3b881915005f5b583dcb9c64682c678bb86309e2b7ef874cfa3765ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117610762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7966d5a395ec7a1f1d9c371fb5ef96bf4ae1143c8031a440c596f127c0b2efcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:49:43 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 02 Feb 2022 04:49:44 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 25 Feb 2022 17:44:00 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 17:44:01 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 17:44:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:44:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:44:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:44:36 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:44:38 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:44:39 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:44:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 17:44:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:44:41 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:44:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbda986a1859ae04347f486c41518b50dca07012a3d2a1a94d0637613db3733`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d27aee3559e3999b8de951b4194fb6741fd48fe8dee089fd69e89516671a40`  
		Last Modified: Fri, 25 Feb 2022 17:49:22 GMT  
		Size: 79.5 MB (79531239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5841ec44f4f001ca7f7bc11b8eb0a7def983285051a345efb0c443c4983105b0`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 3.5 KB (3460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeafb1bb5822eca866ec3b8d6d071c757682bb0ebca067cd3b0ced4e204128ee`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 6.6 KB (6592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff165a38d310d5b8e9e7f999f2a43af4264ad59bbf87cbc62f53f8968d95d15`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0a9f3761f792825d26131e6dd836b389c11d9744570cd4c28decef9b4fb74adf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (130989765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73a16fc01c356f2cef9736753d4be409542af6a7eb671c891274a684d29bfbf1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:24:11 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 02 Feb 2022 06:24:14 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 02 Feb 2022 06:24:18 GMT
ARG MARIADB_VERSION=1:10.3.32+maria~focal
# Wed, 02 Feb 2022 06:24:21 GMT
ENV MARIADB_VERSION=1:10.3.32+maria~focal
# Wed, 02 Feb 2022 06:24:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.32/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:24:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.32/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:28:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.32/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:28:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:28:34 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:28:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.32/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 02 Feb 2022 06:28:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:28:54 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:29:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b3b1ab7b85e06c4533dfd28abcf42980715b35a04ebbfeae2b2d7e5c7b3ef6`  
		Last Modified: Wed, 02 Feb 2022 06:41:44 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f8905242f2496fc2affaeaf880ea5a6a5b3d74f5462a15c116c91e9a376bc9`  
		Last Modified: Wed, 02 Feb 2022 06:42:01 GMT  
		Size: 84.8 MB (84785104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678426eb561b01ae11ac3b45e61f1d4b24b0da25b0a83da69fb58be44188ce20`  
		Last Modified: Wed, 02 Feb 2022 06:41:44 GMT  
		Size: 5.6 KB (5626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931d168ecad36931705df37e8bf67cca09f3ff3a704e7bf7f8fc11778d1842e5`  
		Last Modified: Wed, 02 Feb 2022 06:41:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:fcbed9f7f550d256ec987502fbfd01513ac365ff10ff989e39e36b87b0431056
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:5ff563719b69c13176d018523117206ed0928c3a15ea4547618c14eb493d2fa8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120117250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9c4d949b520a3bda2d53cc35b87df84af0655aade4c6a4b77cc86bcece148f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:47:26 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 02 Feb 2022 03:47:26 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 25 Feb 2022 19:04:24 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 19:04:24 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 19:04:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:04:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:04:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:05:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:05:00 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:05:01 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:05:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 19:05:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:05:03 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:05:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09068eced0b633eec0c4c85f6e82fb884de56a7285f4d36b3504a6d72fa23731`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf18bfce1213ed3f88c5333e6112a6cba219ecf61b0f8dc45a9b87a166ecac2`  
		Last Modified: Fri, 25 Feb 2022 19:10:17 GMT  
		Size: 80.2 MB (80191098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e703ab2dfb1ebabf11b526ea6418cc872fde0e9228699534ca6502316f429f5`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdbba010e4a1689eccb4971867b3ba3a08564e795ec18a5e3c34e415cee1706`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 6.6 KB (6591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472da57979151992035cff2e784a9c871aaef0799eb0ca04a3a3f7ccf8b5777`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:a400461e3b881915005f5b583dcb9c64682c678bb86309e2b7ef874cfa3765ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117610762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7966d5a395ec7a1f1d9c371fb5ef96bf4ae1143c8031a440c596f127c0b2efcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:49:43 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 02 Feb 2022 04:49:44 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 25 Feb 2022 17:44:00 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 17:44:01 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 17:44:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:44:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:44:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:44:36 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:44:38 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:44:39 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:44:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 17:44:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:44:41 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:44:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbda986a1859ae04347f486c41518b50dca07012a3d2a1a94d0637613db3733`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d27aee3559e3999b8de951b4194fb6741fd48fe8dee089fd69e89516671a40`  
		Last Modified: Fri, 25 Feb 2022 17:49:22 GMT  
		Size: 79.5 MB (79531239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5841ec44f4f001ca7f7bc11b8eb0a7def983285051a345efb0c443c4983105b0`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 3.5 KB (3460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeafb1bb5822eca866ec3b8d6d071c757682bb0ebca067cd3b0ced4e204128ee`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 6.6 KB (6592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff165a38d310d5b8e9e7f999f2a43af4264ad59bbf87cbc62f53f8968d95d15`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0a9f3761f792825d26131e6dd836b389c11d9744570cd4c28decef9b4fb74adf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (130989765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73a16fc01c356f2cef9736753d4be409542af6a7eb671c891274a684d29bfbf1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:24:11 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 02 Feb 2022 06:24:14 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 02 Feb 2022 06:24:18 GMT
ARG MARIADB_VERSION=1:10.3.32+maria~focal
# Wed, 02 Feb 2022 06:24:21 GMT
ENV MARIADB_VERSION=1:10.3.32+maria~focal
# Wed, 02 Feb 2022 06:24:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.32/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:24:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.32/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:28:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.32/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:28:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:28:34 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:28:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.32/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 02 Feb 2022 06:28:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:28:54 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:29:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b3b1ab7b85e06c4533dfd28abcf42980715b35a04ebbfeae2b2d7e5c7b3ef6`  
		Last Modified: Wed, 02 Feb 2022 06:41:44 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f8905242f2496fc2affaeaf880ea5a6a5b3d74f5462a15c116c91e9a376bc9`  
		Last Modified: Wed, 02 Feb 2022 06:42:01 GMT  
		Size: 84.8 MB (84785104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678426eb561b01ae11ac3b45e61f1d4b24b0da25b0a83da69fb58be44188ce20`  
		Last Modified: Wed, 02 Feb 2022 06:41:44 GMT  
		Size: 5.6 KB (5626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931d168ecad36931705df37e8bf67cca09f3ff3a704e7bf7f8fc11778d1842e5`  
		Last Modified: Wed, 02 Feb 2022 06:41:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.34`

```console
$ docker pull mariadb@sha256:47b19fb6a1cf0367ccfda2c301932a22c53427bcc6b525d70d2922c2e5ac55f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.3.34` - linux; amd64

```console
$ docker pull mariadb@sha256:5ff563719b69c13176d018523117206ed0928c3a15ea4547618c14eb493d2fa8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120117250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9c4d949b520a3bda2d53cc35b87df84af0655aade4c6a4b77cc86bcece148f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:47:26 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 02 Feb 2022 03:47:26 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 25 Feb 2022 19:04:24 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 19:04:24 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 19:04:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:04:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:04:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:05:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:05:00 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:05:01 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:05:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 19:05:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:05:03 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:05:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09068eced0b633eec0c4c85f6e82fb884de56a7285f4d36b3504a6d72fa23731`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf18bfce1213ed3f88c5333e6112a6cba219ecf61b0f8dc45a9b87a166ecac2`  
		Last Modified: Fri, 25 Feb 2022 19:10:17 GMT  
		Size: 80.2 MB (80191098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e703ab2dfb1ebabf11b526ea6418cc872fde0e9228699534ca6502316f429f5`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdbba010e4a1689eccb4971867b3ba3a08564e795ec18a5e3c34e415cee1706`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 6.6 KB (6591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472da57979151992035cff2e784a9c871aaef0799eb0ca04a3a3f7ccf8b5777`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:a400461e3b881915005f5b583dcb9c64682c678bb86309e2b7ef874cfa3765ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117610762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7966d5a395ec7a1f1d9c371fb5ef96bf4ae1143c8031a440c596f127c0b2efcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:49:43 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 02 Feb 2022 04:49:44 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 25 Feb 2022 17:44:00 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 17:44:01 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 17:44:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:44:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:44:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:44:36 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:44:38 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:44:39 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:44:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 17:44:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:44:41 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:44:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbda986a1859ae04347f486c41518b50dca07012a3d2a1a94d0637613db3733`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d27aee3559e3999b8de951b4194fb6741fd48fe8dee089fd69e89516671a40`  
		Last Modified: Fri, 25 Feb 2022 17:49:22 GMT  
		Size: 79.5 MB (79531239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5841ec44f4f001ca7f7bc11b8eb0a7def983285051a345efb0c443c4983105b0`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 3.5 KB (3460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeafb1bb5822eca866ec3b8d6d071c757682bb0ebca067cd3b0ced4e204128ee`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 6.6 KB (6592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff165a38d310d5b8e9e7f999f2a43af4264ad59bbf87cbc62f53f8968d95d15`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.34-focal`

```console
$ docker pull mariadb@sha256:47b19fb6a1cf0367ccfda2c301932a22c53427bcc6b525d70d2922c2e5ac55f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.3.34-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:5ff563719b69c13176d018523117206ed0928c3a15ea4547618c14eb493d2fa8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120117250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9c4d949b520a3bda2d53cc35b87df84af0655aade4c6a4b77cc86bcece148f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:47:26 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 02 Feb 2022 03:47:26 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 25 Feb 2022 19:04:24 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 19:04:24 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 19:04:24 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:04:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:04:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:05:00 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:05:00 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:05:01 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:05:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 19:05:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:05:03 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:05:03 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09068eced0b633eec0c4c85f6e82fb884de56a7285f4d36b3504a6d72fa23731`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf18bfce1213ed3f88c5333e6112a6cba219ecf61b0f8dc45a9b87a166ecac2`  
		Last Modified: Fri, 25 Feb 2022 19:10:17 GMT  
		Size: 80.2 MB (80191098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e703ab2dfb1ebabf11b526ea6418cc872fde0e9228699534ca6502316f429f5`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdbba010e4a1689eccb4971867b3ba3a08564e795ec18a5e3c34e415cee1706`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 6.6 KB (6591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472da57979151992035cff2e784a9c871aaef0799eb0ca04a3a3f7ccf8b5777`  
		Last Modified: Fri, 25 Feb 2022 19:10:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:a400461e3b881915005f5b583dcb9c64682c678bb86309e2b7ef874cfa3765ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117610762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7966d5a395ec7a1f1d9c371fb5ef96bf4ae1143c8031a440c596f127c0b2efcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:49:43 GMT
ARG MARIADB_MAJOR=10.3
# Wed, 02 Feb 2022 04:49:44 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 25 Feb 2022 17:44:00 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 17:44:01 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 25 Feb 2022 17:44:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:44:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:44:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:44:36 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:44:38 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:44:39 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:44:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 17:44:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:44:41 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:44:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbda986a1859ae04347f486c41518b50dca07012a3d2a1a94d0637613db3733`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d27aee3559e3999b8de951b4194fb6741fd48fe8dee089fd69e89516671a40`  
		Last Modified: Fri, 25 Feb 2022 17:49:22 GMT  
		Size: 79.5 MB (79531239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5841ec44f4f001ca7f7bc11b8eb0a7def983285051a345efb0c443c4983105b0`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 3.5 KB (3460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeafb1bb5822eca866ec3b8d6d071c757682bb0ebca067cd3b0ced4e204128ee`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 6.6 KB (6592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff165a38d310d5b8e9e7f999f2a43af4264ad59bbf87cbc62f53f8968d95d15`  
		Last Modified: Fri, 25 Feb 2022 17:49:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:07b41aa88b1e1af6dab61daa7cdc2fb304baece345beaf18864d278f73bc80d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:4f6a6149b44efcf25e7f42d9eaa0ecfa1064309d52f1010b107be61ef78edd04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b7e43bdc7cb4b6250eeb8b31049fd432d63f0def53b66039495acf5061bf381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:46:52 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 02 Feb 2022 03:46:52 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 25 Feb 2022 19:03:42 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 19:03:43 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 19:03:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:03:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:04:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:04:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:04:15 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:04:15 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:04:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 19:04:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:04:17 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:04:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6156b5ae3eab330f960e987f6f8909e66383b40568023750502e35592c3386`  
		Last Modified: Fri, 25 Feb 2022 19:09:24 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a164602a707b12618fd4f4bd8aaec0793caa4758d50ff5c1ca2e8f94ce42168`  
		Last Modified: Fri, 25 Feb 2022 19:09:41 GMT  
		Size: 85.8 MB (85753048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7737b42b2f9d437e71347b905f24a0b9f609a82deab811d1f7b0c54f30887435`  
		Last Modified: Fri, 25 Feb 2022 19:09:23 GMT  
		Size: 3.5 KB (3458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85df6a2eee8e484d15aee5deaf795e069c4fb33338acd2d415183a514d767927`  
		Last Modified: Fri, 25 Feb 2022 19:09:23 GMT  
		Size: 6.6 KB (6590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b89880e212bf6dd24e0eee0e0395baebdc93b2997fd22003d8c2717525c0f4`  
		Last Modified: Fri, 25 Feb 2022 19:09:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5712948438b5f793066e0bfc1a912865d31a58cc47e91630af0d78bff721fe01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123005216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8278c2d9931dd3f7d1f9d81e83bd271ff07319d1f64f232cbc0201827610e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:47:00 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 02 Feb 2022 04:47:00 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 25 Feb 2022 17:43:09 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 17:43:10 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 17:43:11 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:43:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:43:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:43:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:43:46 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:43:47 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:43:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 17:43:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:43:49 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:43:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b4cd5c6baf7ad79fff81296377b291354c76f16821f66ad252fe8f1cec5f2e`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1015ba2785f5a9a3f43b1a4f641be3bc53a424b846d040b979523771f5de44b8`  
		Last Modified: Fri, 25 Feb 2022 17:48:50 GMT  
		Size: 84.9 MB (84925692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20192bff400583959ad4bca722f8712ef0ed5ec95dcb121b172457779357294e`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e342d92f9497f68fcc76e2f3f814b592656595e7027749f4f1d85b1d7b8bb0`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 6.6 KB (6594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398e538a06ec46a957e2eadb1e23731ec49800079766412adf7b0987186715cc`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8ac062e3f5787cb5f91688cc9349d0d2aac79264fce394210445ba675e47fc5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135595732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:955d19710c1ca20a943bfe61843818ddc6523c80045c4b892ee4f06ffb298167`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:20:45 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 02 Feb 2022 06:20:47 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 02 Feb 2022 06:20:49 GMT
ARG MARIADB_VERSION=1:10.4.22+maria~focal
# Wed, 02 Feb 2022 06:20:53 GMT
ENV MARIADB_VERSION=1:10.4.22+maria~focal
# Wed, 02 Feb 2022 06:21:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.22/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:21:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.22/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:23:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.22/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:23:20 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:23:23 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:23:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.22/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 02 Feb 2022 06:23:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:23:46 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:23:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6570be9de70a14fcc9de9959b7a1c8d984bdfbddb345e8689dff921e8c5a33d3`  
		Last Modified: Wed, 02 Feb 2022 06:41:07 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07a6cb8d20b19032086d6e8896d2f8204e31c015733e580eb0e89d0d31d8a7f`  
		Last Modified: Wed, 02 Feb 2022 06:41:25 GMT  
		Size: 89.4 MB (89391070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba8b71ab431fd2487c83a51e490389713822d6d774fa474caba5b867e239576`  
		Last Modified: Wed, 02 Feb 2022 06:41:07 GMT  
		Size: 5.6 KB (5628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e345e87748fa5e011bd5cc0661e58b534f6ea21d33f14a37f5cac4563892a0`  
		Last Modified: Wed, 02 Feb 2022 06:41:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:07b41aa88b1e1af6dab61daa7cdc2fb304baece345beaf18864d278f73bc80d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:4f6a6149b44efcf25e7f42d9eaa0ecfa1064309d52f1010b107be61ef78edd04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b7e43bdc7cb4b6250eeb8b31049fd432d63f0def53b66039495acf5061bf381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:46:52 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 02 Feb 2022 03:46:52 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 25 Feb 2022 19:03:42 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 19:03:43 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 19:03:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:03:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:04:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:04:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:04:15 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:04:15 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:04:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 19:04:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:04:17 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:04:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6156b5ae3eab330f960e987f6f8909e66383b40568023750502e35592c3386`  
		Last Modified: Fri, 25 Feb 2022 19:09:24 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a164602a707b12618fd4f4bd8aaec0793caa4758d50ff5c1ca2e8f94ce42168`  
		Last Modified: Fri, 25 Feb 2022 19:09:41 GMT  
		Size: 85.8 MB (85753048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7737b42b2f9d437e71347b905f24a0b9f609a82deab811d1f7b0c54f30887435`  
		Last Modified: Fri, 25 Feb 2022 19:09:23 GMT  
		Size: 3.5 KB (3458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85df6a2eee8e484d15aee5deaf795e069c4fb33338acd2d415183a514d767927`  
		Last Modified: Fri, 25 Feb 2022 19:09:23 GMT  
		Size: 6.6 KB (6590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b89880e212bf6dd24e0eee0e0395baebdc93b2997fd22003d8c2717525c0f4`  
		Last Modified: Fri, 25 Feb 2022 19:09:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5712948438b5f793066e0bfc1a912865d31a58cc47e91630af0d78bff721fe01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123005216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8278c2d9931dd3f7d1f9d81e83bd271ff07319d1f64f232cbc0201827610e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:47:00 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 02 Feb 2022 04:47:00 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 25 Feb 2022 17:43:09 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 17:43:10 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 17:43:11 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:43:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:43:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:43:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:43:46 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:43:47 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:43:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 17:43:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:43:49 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:43:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b4cd5c6baf7ad79fff81296377b291354c76f16821f66ad252fe8f1cec5f2e`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1015ba2785f5a9a3f43b1a4f641be3bc53a424b846d040b979523771f5de44b8`  
		Last Modified: Fri, 25 Feb 2022 17:48:50 GMT  
		Size: 84.9 MB (84925692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20192bff400583959ad4bca722f8712ef0ed5ec95dcb121b172457779357294e`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e342d92f9497f68fcc76e2f3f814b592656595e7027749f4f1d85b1d7b8bb0`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 6.6 KB (6594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398e538a06ec46a957e2eadb1e23731ec49800079766412adf7b0987186715cc`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8ac062e3f5787cb5f91688cc9349d0d2aac79264fce394210445ba675e47fc5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135595732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:955d19710c1ca20a943bfe61843818ddc6523c80045c4b892ee4f06ffb298167`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:20:45 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 02 Feb 2022 06:20:47 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 02 Feb 2022 06:20:49 GMT
ARG MARIADB_VERSION=1:10.4.22+maria~focal
# Wed, 02 Feb 2022 06:20:53 GMT
ENV MARIADB_VERSION=1:10.4.22+maria~focal
# Wed, 02 Feb 2022 06:21:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.22/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:21:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.22/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:23:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.22/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:23:20 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:23:23 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:23:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.22/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 02 Feb 2022 06:23:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:23:46 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:23:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6570be9de70a14fcc9de9959b7a1c8d984bdfbddb345e8689dff921e8c5a33d3`  
		Last Modified: Wed, 02 Feb 2022 06:41:07 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07a6cb8d20b19032086d6e8896d2f8204e31c015733e580eb0e89d0d31d8a7f`  
		Last Modified: Wed, 02 Feb 2022 06:41:25 GMT  
		Size: 89.4 MB (89391070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba8b71ab431fd2487c83a51e490389713822d6d774fa474caba5b867e239576`  
		Last Modified: Wed, 02 Feb 2022 06:41:07 GMT  
		Size: 5.6 KB (5628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e345e87748fa5e011bd5cc0661e58b534f6ea21d33f14a37f5cac4563892a0`  
		Last Modified: Wed, 02 Feb 2022 06:41:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.24`

```console
$ docker pull mariadb@sha256:dffb0b4c3c24652e32e438efbbf8082180a1b506407d8397be46b55096057969
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.4.24` - linux; amd64

```console
$ docker pull mariadb@sha256:4f6a6149b44efcf25e7f42d9eaa0ecfa1064309d52f1010b107be61ef78edd04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b7e43bdc7cb4b6250eeb8b31049fd432d63f0def53b66039495acf5061bf381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:46:52 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 02 Feb 2022 03:46:52 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 25 Feb 2022 19:03:42 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 19:03:43 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 19:03:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:03:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:04:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:04:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:04:15 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:04:15 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:04:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 19:04:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:04:17 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:04:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6156b5ae3eab330f960e987f6f8909e66383b40568023750502e35592c3386`  
		Last Modified: Fri, 25 Feb 2022 19:09:24 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a164602a707b12618fd4f4bd8aaec0793caa4758d50ff5c1ca2e8f94ce42168`  
		Last Modified: Fri, 25 Feb 2022 19:09:41 GMT  
		Size: 85.8 MB (85753048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7737b42b2f9d437e71347b905f24a0b9f609a82deab811d1f7b0c54f30887435`  
		Last Modified: Fri, 25 Feb 2022 19:09:23 GMT  
		Size: 3.5 KB (3458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85df6a2eee8e484d15aee5deaf795e069c4fb33338acd2d415183a514d767927`  
		Last Modified: Fri, 25 Feb 2022 19:09:23 GMT  
		Size: 6.6 KB (6590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b89880e212bf6dd24e0eee0e0395baebdc93b2997fd22003d8c2717525c0f4`  
		Last Modified: Fri, 25 Feb 2022 19:09:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5712948438b5f793066e0bfc1a912865d31a58cc47e91630af0d78bff721fe01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123005216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8278c2d9931dd3f7d1f9d81e83bd271ff07319d1f64f232cbc0201827610e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:47:00 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 02 Feb 2022 04:47:00 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 25 Feb 2022 17:43:09 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 17:43:10 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 17:43:11 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:43:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:43:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:43:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:43:46 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:43:47 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:43:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 17:43:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:43:49 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:43:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b4cd5c6baf7ad79fff81296377b291354c76f16821f66ad252fe8f1cec5f2e`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1015ba2785f5a9a3f43b1a4f641be3bc53a424b846d040b979523771f5de44b8`  
		Last Modified: Fri, 25 Feb 2022 17:48:50 GMT  
		Size: 84.9 MB (84925692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20192bff400583959ad4bca722f8712ef0ed5ec95dcb121b172457779357294e`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e342d92f9497f68fcc76e2f3f814b592656595e7027749f4f1d85b1d7b8bb0`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 6.6 KB (6594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398e538a06ec46a957e2eadb1e23731ec49800079766412adf7b0987186715cc`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.24-focal`

```console
$ docker pull mariadb@sha256:dffb0b4c3c24652e32e438efbbf8082180a1b506407d8397be46b55096057969
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mariadb:10.4.24-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:4f6a6149b44efcf25e7f42d9eaa0ecfa1064309d52f1010b107be61ef78edd04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125679196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b7e43bdc7cb4b6250eeb8b31049fd432d63f0def53b66039495acf5061bf381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:46:52 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 02 Feb 2022 03:46:52 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 25 Feb 2022 19:03:42 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 19:03:43 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 19:03:43 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:03:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:04:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:04:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:04:15 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:04:15 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:04:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 19:04:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:04:17 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:04:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6156b5ae3eab330f960e987f6f8909e66383b40568023750502e35592c3386`  
		Last Modified: Fri, 25 Feb 2022 19:09:24 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a164602a707b12618fd4f4bd8aaec0793caa4758d50ff5c1ca2e8f94ce42168`  
		Last Modified: Fri, 25 Feb 2022 19:09:41 GMT  
		Size: 85.8 MB (85753048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7737b42b2f9d437e71347b905f24a0b9f609a82deab811d1f7b0c54f30887435`  
		Last Modified: Fri, 25 Feb 2022 19:09:23 GMT  
		Size: 3.5 KB (3458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85df6a2eee8e484d15aee5deaf795e069c4fb33338acd2d415183a514d767927`  
		Last Modified: Fri, 25 Feb 2022 19:09:23 GMT  
		Size: 6.6 KB (6590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b89880e212bf6dd24e0eee0e0395baebdc93b2997fd22003d8c2717525c0f4`  
		Last Modified: Fri, 25 Feb 2022 19:09:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5712948438b5f793066e0bfc1a912865d31a58cc47e91630af0d78bff721fe01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123005216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8278c2d9931dd3f7d1f9d81e83bd271ff07319d1f64f232cbc0201827610e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:47:00 GMT
ARG MARIADB_MAJOR=10.4
# Wed, 02 Feb 2022 04:47:00 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 25 Feb 2022 17:43:09 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 17:43:10 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 25 Feb 2022 17:43:11 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:43:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:43:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:43:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:43:46 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:43:47 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:43:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Feb 2022 17:43:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:43:49 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:43:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b4cd5c6baf7ad79fff81296377b291354c76f16821f66ad252fe8f1cec5f2e`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1015ba2785f5a9a3f43b1a4f641be3bc53a424b846d040b979523771f5de44b8`  
		Last Modified: Fri, 25 Feb 2022 17:48:50 GMT  
		Size: 84.9 MB (84925692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20192bff400583959ad4bca722f8712ef0ed5ec95dcb121b172457779357294e`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e342d92f9497f68fcc76e2f3f814b592656595e7027749f4f1d85b1d7b8bb0`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 6.6 KB (6594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398e538a06ec46a957e2eadb1e23731ec49800079766412adf7b0987186715cc`  
		Last Modified: Fri, 25 Feb 2022 17:48:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:70e3c450633262efb6f0483896d8f45d904d0e1addee15dc3d5017cf39ff9093
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:7485ec97845ab634ae5d20c6d77cf7e75074a5bf25fdc5fa43d56c02e276b13b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127922535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de390e78f76e36b80d2058fe2d03b412dfc2d27a1e9b6adba86046dc4ab6cb8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:46:24 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 03:46:24 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Feb 2022 19:03:01 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 19:03:02 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 19:03:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:03:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:03:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:03:34 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:03:34 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:03:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:03:34 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:03:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04ebe61f0f28bd5b0152200a2b2b391d70185963444625f748b1965b5cc3ed`  
		Last Modified: Fri, 25 Feb 2022 19:08:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1636f5af837d6842067e5e608bfce498c31c97fac419e1f5d28f31033ca664`  
		Last Modified: Fri, 25 Feb 2022 19:09:06 GMT  
		Size: 88.0 MB (87996503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db85d8041fbf13d2aec88efee1942f6ab98624568e4cfcb05b55384b27d7b51c`  
		Last Modified: Fri, 25 Feb 2022 19:08:49 GMT  
		Size: 3.5 KB (3460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6007a391685787b262bb862b952fead864d6d88545870ffad22a6032836a5a`  
		Last Modified: Fri, 25 Feb 2022 19:08:50 GMT  
		Size: 6.6 KB (6594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5449562c72310ad7d6f0c560fe311ee10f7e6ca0b6447f811f9b380c3d201575
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125188522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db6d25607e066e9ffc7ae78ec9ccf68c81fda9620521cc6b0fd0429d3f30cd9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:45:33 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 04:45:34 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Feb 2022 17:42:25 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:42:26 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:42:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:42:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:59 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:43:00 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:43:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909ddc1e4a924d2fbfd551aeb58b73f53118882a59ae7b8b1292c0ab3bbc336f`  
		Last Modified: Fri, 25 Feb 2022 17:48:04 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceeaa1aba9629ebab0f92ef65bd246f55e53655725a62939b96ccf32c21d539`  
		Last Modified: Fri, 25 Feb 2022 17:48:18 GMT  
		Size: 87.1 MB (87109125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf475978b17dcc6e7a56f414b7cdbbe3d145f485ce0cc0f912ad2c451f3db1b3`  
		Last Modified: Fri, 25 Feb 2022 17:48:04 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176678d169626ab22126e1a95e800d56737e2333c528502c949f7a4b6ebf083e`  
		Last Modified: Fri, 25 Feb 2022 17:48:04 GMT  
		Size: 6.6 KB (6593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f86309b5a56f8b47101d59b7c9793f3ba34ffdc2ce74e8c781c7f14e840dede2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137739655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a170e658df65dde6947464925b6b410cf0502bea0f83d26e733735e0d2aec108`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:17:47 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 06:17:51 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 06:17:53 GMT
ARG MARIADB_VERSION=1:10.5.13+maria~focal
# Wed, 02 Feb 2022 06:17:54 GMT
ENV MARIADB_VERSION=1:10.5.13+maria~focal
# Wed, 02 Feb 2022 06:17:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.13/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:18:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.13/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:20:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.13/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:20:25 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:20:27 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:20:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:20:32 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:20:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbd46e649db8d71980e62fd014d8e9857cdb4f7bf0136bf0697e34bc369fc89`  
		Last Modified: Wed, 02 Feb 2022 06:40:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7781f6d5825ff6d2e9b6090a9150ce7e1d919d6f944d283e9bfdb85d6607dda2`  
		Last Modified: Wed, 02 Feb 2022 06:40:48 GMT  
		Size: 91.5 MB (91535115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685e421fd251f8ee6e6b7be7f7a3062d234ca234a48942b62a4617f357b5ca9a`  
		Last Modified: Wed, 02 Feb 2022 06:40:30 GMT  
		Size: 5.6 KB (5628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; s390x

```console
$ docker pull mariadb@sha256:0d0dfc3591ac91d09c16a8b27c4af93b64817679596c4d6ba75d5137140cfc3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127235090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:157dd9f0b06e1e49af8d7d2ba67569370f1ed08c70dfb3ac8d930e2d0a49002a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:02:40 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 02:02:41 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Feb 2022 17:43:40 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:43:40 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:43:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:43:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:44:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:44:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:44:05 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:44:06 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:44:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:44:06 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:44:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bbeaa7740ccfdc136df7f83f134c65c756afb9c4c1323685e6c5a09ea1bbe2`  
		Last Modified: Fri, 25 Feb 2022 17:46:25 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24124520ec6939f21bcac64b99e3c8864ba8ae77cd97256f3f8a0d8946be22ab`  
		Last Modified: Fri, 25 Feb 2022 17:46:38 GMT  
		Size: 89.3 MB (89290484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a605e22dadbd681fdfaa2ed8d6006bee185eb062f4b61dfa3e9dadcec2846bb5`  
		Last Modified: Fri, 25 Feb 2022 17:46:25 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751922a191ab74d97794b5c0b261e4535f5fb030227f2147379fb6350fa15565`  
		Last Modified: Fri, 25 Feb 2022 17:46:25 GMT  
		Size: 6.6 KB (6593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:70e3c450633262efb6f0483896d8f45d904d0e1addee15dc3d5017cf39ff9093
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:7485ec97845ab634ae5d20c6d77cf7e75074a5bf25fdc5fa43d56c02e276b13b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127922535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de390e78f76e36b80d2058fe2d03b412dfc2d27a1e9b6adba86046dc4ab6cb8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:46:24 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 03:46:24 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Feb 2022 19:03:01 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 19:03:02 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 19:03:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:03:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:03:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:03:34 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:03:34 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:03:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:03:34 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:03:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04ebe61f0f28bd5b0152200a2b2b391d70185963444625f748b1965b5cc3ed`  
		Last Modified: Fri, 25 Feb 2022 19:08:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1636f5af837d6842067e5e608bfce498c31c97fac419e1f5d28f31033ca664`  
		Last Modified: Fri, 25 Feb 2022 19:09:06 GMT  
		Size: 88.0 MB (87996503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db85d8041fbf13d2aec88efee1942f6ab98624568e4cfcb05b55384b27d7b51c`  
		Last Modified: Fri, 25 Feb 2022 19:08:49 GMT  
		Size: 3.5 KB (3460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6007a391685787b262bb862b952fead864d6d88545870ffad22a6032836a5a`  
		Last Modified: Fri, 25 Feb 2022 19:08:50 GMT  
		Size: 6.6 KB (6594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5449562c72310ad7d6f0c560fe311ee10f7e6ca0b6447f811f9b380c3d201575
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125188522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db6d25607e066e9ffc7ae78ec9ccf68c81fda9620521cc6b0fd0429d3f30cd9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:45:33 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 04:45:34 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Feb 2022 17:42:25 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:42:26 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:42:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:42:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:59 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:43:00 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:43:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909ddc1e4a924d2fbfd551aeb58b73f53118882a59ae7b8b1292c0ab3bbc336f`  
		Last Modified: Fri, 25 Feb 2022 17:48:04 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceeaa1aba9629ebab0f92ef65bd246f55e53655725a62939b96ccf32c21d539`  
		Last Modified: Fri, 25 Feb 2022 17:48:18 GMT  
		Size: 87.1 MB (87109125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf475978b17dcc6e7a56f414b7cdbbe3d145f485ce0cc0f912ad2c451f3db1b3`  
		Last Modified: Fri, 25 Feb 2022 17:48:04 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176678d169626ab22126e1a95e800d56737e2333c528502c949f7a4b6ebf083e`  
		Last Modified: Fri, 25 Feb 2022 17:48:04 GMT  
		Size: 6.6 KB (6593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f86309b5a56f8b47101d59b7c9793f3ba34ffdc2ce74e8c781c7f14e840dede2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137739655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a170e658df65dde6947464925b6b410cf0502bea0f83d26e733735e0d2aec108`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:17:47 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 06:17:51 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 06:17:53 GMT
ARG MARIADB_VERSION=1:10.5.13+maria~focal
# Wed, 02 Feb 2022 06:17:54 GMT
ENV MARIADB_VERSION=1:10.5.13+maria~focal
# Wed, 02 Feb 2022 06:17:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.13/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:18:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.13/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:20:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.13/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:20:25 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:20:27 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:20:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:20:32 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:20:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbd46e649db8d71980e62fd014d8e9857cdb4f7bf0136bf0697e34bc369fc89`  
		Last Modified: Wed, 02 Feb 2022 06:40:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7781f6d5825ff6d2e9b6090a9150ce7e1d919d6f944d283e9bfdb85d6607dda2`  
		Last Modified: Wed, 02 Feb 2022 06:40:48 GMT  
		Size: 91.5 MB (91535115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685e421fd251f8ee6e6b7be7f7a3062d234ca234a48942b62a4617f357b5ca9a`  
		Last Modified: Wed, 02 Feb 2022 06:40:30 GMT  
		Size: 5.6 KB (5628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:0d0dfc3591ac91d09c16a8b27c4af93b64817679596c4d6ba75d5137140cfc3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127235090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:157dd9f0b06e1e49af8d7d2ba67569370f1ed08c70dfb3ac8d930e2d0a49002a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:02:40 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 02:02:41 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Feb 2022 17:43:40 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:43:40 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:43:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:43:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:44:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:44:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:44:05 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:44:06 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:44:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:44:06 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:44:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bbeaa7740ccfdc136df7f83f134c65c756afb9c4c1323685e6c5a09ea1bbe2`  
		Last Modified: Fri, 25 Feb 2022 17:46:25 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24124520ec6939f21bcac64b99e3c8864ba8ae77cd97256f3f8a0d8946be22ab`  
		Last Modified: Fri, 25 Feb 2022 17:46:38 GMT  
		Size: 89.3 MB (89290484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a605e22dadbd681fdfaa2ed8d6006bee185eb062f4b61dfa3e9dadcec2846bb5`  
		Last Modified: Fri, 25 Feb 2022 17:46:25 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751922a191ab74d97794b5c0b261e4535f5fb030227f2147379fb6350fa15565`  
		Last Modified: Fri, 25 Feb 2022 17:46:25 GMT  
		Size: 6.6 KB (6593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.15`

```console
$ docker pull mariadb@sha256:9b83e1082d7cd382be057af28e20d8bd553e629070f643e691736c7b59113048
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.5.15` - linux; amd64

```console
$ docker pull mariadb@sha256:7485ec97845ab634ae5d20c6d77cf7e75074a5bf25fdc5fa43d56c02e276b13b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127922535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de390e78f76e36b80d2058fe2d03b412dfc2d27a1e9b6adba86046dc4ab6cb8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:46:24 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 03:46:24 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Feb 2022 19:03:01 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 19:03:02 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 19:03:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:03:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:03:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:03:34 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:03:34 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:03:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:03:34 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:03:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04ebe61f0f28bd5b0152200a2b2b391d70185963444625f748b1965b5cc3ed`  
		Last Modified: Fri, 25 Feb 2022 19:08:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1636f5af837d6842067e5e608bfce498c31c97fac419e1f5d28f31033ca664`  
		Last Modified: Fri, 25 Feb 2022 19:09:06 GMT  
		Size: 88.0 MB (87996503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db85d8041fbf13d2aec88efee1942f6ab98624568e4cfcb05b55384b27d7b51c`  
		Last Modified: Fri, 25 Feb 2022 19:08:49 GMT  
		Size: 3.5 KB (3460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6007a391685787b262bb862b952fead864d6d88545870ffad22a6032836a5a`  
		Last Modified: Fri, 25 Feb 2022 19:08:50 GMT  
		Size: 6.6 KB (6594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5449562c72310ad7d6f0c560fe311ee10f7e6ca0b6447f811f9b380c3d201575
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125188522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db6d25607e066e9ffc7ae78ec9ccf68c81fda9620521cc6b0fd0429d3f30cd9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:45:33 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 04:45:34 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Feb 2022 17:42:25 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:42:26 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:42:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:42:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:59 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:43:00 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:43:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909ddc1e4a924d2fbfd551aeb58b73f53118882a59ae7b8b1292c0ab3bbc336f`  
		Last Modified: Fri, 25 Feb 2022 17:48:04 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceeaa1aba9629ebab0f92ef65bd246f55e53655725a62939b96ccf32c21d539`  
		Last Modified: Fri, 25 Feb 2022 17:48:18 GMT  
		Size: 87.1 MB (87109125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf475978b17dcc6e7a56f414b7cdbbe3d145f485ce0cc0f912ad2c451f3db1b3`  
		Last Modified: Fri, 25 Feb 2022 17:48:04 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176678d169626ab22126e1a95e800d56737e2333c528502c949f7a4b6ebf083e`  
		Last Modified: Fri, 25 Feb 2022 17:48:04 GMT  
		Size: 6.6 KB (6593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; s390x

```console
$ docker pull mariadb@sha256:0d0dfc3591ac91d09c16a8b27c4af93b64817679596c4d6ba75d5137140cfc3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127235090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:157dd9f0b06e1e49af8d7d2ba67569370f1ed08c70dfb3ac8d930e2d0a49002a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:02:40 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 02:02:41 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Feb 2022 17:43:40 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:43:40 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:43:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:43:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:44:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:44:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:44:05 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:44:06 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:44:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:44:06 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:44:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bbeaa7740ccfdc136df7f83f134c65c756afb9c4c1323685e6c5a09ea1bbe2`  
		Last Modified: Fri, 25 Feb 2022 17:46:25 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24124520ec6939f21bcac64b99e3c8864ba8ae77cd97256f3f8a0d8946be22ab`  
		Last Modified: Fri, 25 Feb 2022 17:46:38 GMT  
		Size: 89.3 MB (89290484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a605e22dadbd681fdfaa2ed8d6006bee185eb062f4b61dfa3e9dadcec2846bb5`  
		Last Modified: Fri, 25 Feb 2022 17:46:25 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751922a191ab74d97794b5c0b261e4535f5fb030227f2147379fb6350fa15565`  
		Last Modified: Fri, 25 Feb 2022 17:46:25 GMT  
		Size: 6.6 KB (6593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.15-focal`

```console
$ docker pull mariadb@sha256:9b83e1082d7cd382be057af28e20d8bd553e629070f643e691736c7b59113048
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.5.15-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:7485ec97845ab634ae5d20c6d77cf7e75074a5bf25fdc5fa43d56c02e276b13b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127922535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de390e78f76e36b80d2058fe2d03b412dfc2d27a1e9b6adba86046dc4ab6cb8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:46:24 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 03:46:24 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Feb 2022 19:03:01 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 19:03:02 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 19:03:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:03:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:03:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:03:34 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:03:34 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:03:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:03:34 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:03:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04ebe61f0f28bd5b0152200a2b2b391d70185963444625f748b1965b5cc3ed`  
		Last Modified: Fri, 25 Feb 2022 19:08:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1636f5af837d6842067e5e608bfce498c31c97fac419e1f5d28f31033ca664`  
		Last Modified: Fri, 25 Feb 2022 19:09:06 GMT  
		Size: 88.0 MB (87996503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db85d8041fbf13d2aec88efee1942f6ab98624568e4cfcb05b55384b27d7b51c`  
		Last Modified: Fri, 25 Feb 2022 19:08:49 GMT  
		Size: 3.5 KB (3460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6007a391685787b262bb862b952fead864d6d88545870ffad22a6032836a5a`  
		Last Modified: Fri, 25 Feb 2022 19:08:50 GMT  
		Size: 6.6 KB (6594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5449562c72310ad7d6f0c560fe311ee10f7e6ca0b6447f811f9b380c3d201575
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125188522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2db6d25607e066e9ffc7ae78ec9ccf68c81fda9620521cc6b0fd0429d3f30cd9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:45:33 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 04:45:34 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Feb 2022 17:42:25 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:42:26 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:42:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:42:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:59 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:43:00 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:43:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909ddc1e4a924d2fbfd551aeb58b73f53118882a59ae7b8b1292c0ab3bbc336f`  
		Last Modified: Fri, 25 Feb 2022 17:48:04 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dceeaa1aba9629ebab0f92ef65bd246f55e53655725a62939b96ccf32c21d539`  
		Last Modified: Fri, 25 Feb 2022 17:48:18 GMT  
		Size: 87.1 MB (87109125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf475978b17dcc6e7a56f414b7cdbbe3d145f485ce0cc0f912ad2c451f3db1b3`  
		Last Modified: Fri, 25 Feb 2022 17:48:04 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176678d169626ab22126e1a95e800d56737e2333c528502c949f7a4b6ebf083e`  
		Last Modified: Fri, 25 Feb 2022 17:48:04 GMT  
		Size: 6.6 KB (6593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:0d0dfc3591ac91d09c16a8b27c4af93b64817679596c4d6ba75d5137140cfc3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127235090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:157dd9f0b06e1e49af8d7d2ba67569370f1ed08c70dfb3ac8d930e2d0a49002a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:02:40 GMT
ARG MARIADB_MAJOR=10.5
# Wed, 02 Feb 2022 02:02:41 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 25 Feb 2022 17:43:40 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:43:40 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 25 Feb 2022 17:43:40 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:43:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:44:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:44:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:44:05 GMT
COPY file:7b2b830b1a87b166f4a5a732707acff0251efb190222ea81169b87df1e30b0c1 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:44:06 GMT
COPY file:33a8142f1ef606149777b7c7100f497729a65097239aa974a0160afddf7b5c26 in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:44:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:44:06 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:44:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bbeaa7740ccfdc136df7f83f134c65c756afb9c4c1323685e6c5a09ea1bbe2`  
		Last Modified: Fri, 25 Feb 2022 17:46:25 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24124520ec6939f21bcac64b99e3c8864ba8ae77cd97256f3f8a0d8946be22ab`  
		Last Modified: Fri, 25 Feb 2022 17:46:38 GMT  
		Size: 89.3 MB (89290484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a605e22dadbd681fdfaa2ed8d6006bee185eb062f4b61dfa3e9dadcec2846bb5`  
		Last Modified: Fri, 25 Feb 2022 17:46:25 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751922a191ab74d97794b5c0b261e4535f5fb030227f2147379fb6350fa15565`  
		Last Modified: Fri, 25 Feb 2022 17:46:25 GMT  
		Size: 6.6 KB (6593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:d7621611bc109dad8983f5eb1e56f4a0f0fba0b95e1d6721c2e4687204dfe827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:008e0a5cd570889de96550f509a6a7a0cac1dbbf7e94265f5de497b45de97a1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128169486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ca1bb790d953c74b114c4ff3b7b5bdad99850bee6e9490e087c3abc57406d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:45:54 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 03:45:54 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 25 Feb 2022 19:02:20 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 19:02:20 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 19:02:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:02:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:02:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:02:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:02:56 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:02:57 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:02:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:02:57 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:02:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4becccd3dd4bfdd537199df53c49d74271a594ce337d1995892367406caf71`  
		Last Modified: Fri, 25 Feb 2022 19:08:19 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73da7c2ac5af5a9e3ba4bafa57276a54b5b51db2f48e9b4098d6fc542e7cef17`  
		Last Modified: Fri, 25 Feb 2022 19:08:33 GMT  
		Size: 88.2 MB (88243453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31163609685e6a5f3a3a18b64e38c1ac6a938f373308b6bf346e7abc80a3f157`  
		Last Modified: Fri, 25 Feb 2022 19:08:19 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9162f300b21308a5df5bb223206f4e2f3d2e251c179c6be1defdce49b111602`  
		Last Modified: Fri, 25 Feb 2022 19:08:19 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ae493c7b33cd9283f20896c891cf51ef8835e1d28742ba576b2435fd31dd5010
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125272637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:482dfce2aec58426a2445430dc5199dc257766a2f91890bd254b461a27d8b043`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:42:06 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 04:42:06 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 25 Feb 2022 17:41:40 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:41:41 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:41:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:41:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:16 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:17 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:18 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:19 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d49800d26cc57960935b2b51c925d67989ccf5ea2e6cb9efdaada4c97de7fe`  
		Last Modified: Fri, 25 Feb 2022 17:47:32 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f644e931eabfa9683592bffd84d2b6877afeb86e1d0a891fe930cd61e2240ba`  
		Last Modified: Fri, 25 Feb 2022 17:47:46 GMT  
		Size: 87.2 MB (87193233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0ecd2ff84ca16016cd11046f2bc070eefd4caa25f24dbc8b751962a8e2c741`  
		Last Modified: Fri, 25 Feb 2022 17:47:32 GMT  
		Size: 3.5 KB (3457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0e36c3d259009a7af93b32530988630438a12fd235661dc5c66cdc9268eb6b`  
		Last Modified: Fri, 25 Feb 2022 17:47:32 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:26365cfc20ce97ce9359b32d5774b0cd623e503cd1dc0a5ddbc065b92fa9e70a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137783748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737496717e740b26172016c9c63dbeb5ae8ee2a178eb689b4f8a4c9176d37b99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:14:03 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 06:14:05 GMT
ENV MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 06:14:07 GMT
ARG MARIADB_VERSION=1:10.6.5+maria~focal
# Wed, 02 Feb 2022 06:14:08 GMT
ENV MARIADB_VERSION=1:10.6.5+maria~focal
# Wed, 02 Feb 2022 06:14:11 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:14:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:16:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:17:15 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:17:18 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:17:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:17:28 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:17:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4683b2a4076da23a58c3d55ec3193591331e38c1da0cd871cb108e31c76984ec`  
		Last Modified: Wed, 02 Feb 2022 06:39:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cedf38ea121b3c6203ec8682b97afed76dc9815da29af531bf48951ecbed21`  
		Last Modified: Wed, 02 Feb 2022 06:39:57 GMT  
		Size: 91.6 MB (91579209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca079698384d698aa1ec8a2a18c8458fbed546951d84d331a3d168d4dd4acba`  
		Last Modified: Wed, 02 Feb 2022 06:39:39 GMT  
		Size: 5.6 KB (5626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; s390x

```console
$ docker pull mariadb@sha256:381ac4edf0b5ea109043605c9a6de2eec3f97de63d3b074f64d8b3401b128801
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127260924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff65a1eb5e3840fb92355287b2d21516d4ec40b7f92a676f906569915d4c602`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:02:03 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 02:02:03 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 25 Feb 2022 17:43:08 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:43:08 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:43:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:43:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:43:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:43:32 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:43:32 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:43:32 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:43:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:43:32 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:43:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124a747d11e0921bbf0eb728acae7edcd82997ff2e2f55fad0a6b88090a5e914`  
		Last Modified: Fri, 25 Feb 2022 17:45:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26577ed88062a982e95a549f67d31c62a66df5a03788d1dd2e8142893536b111`  
		Last Modified: Fri, 25 Feb 2022 17:46:12 GMT  
		Size: 89.3 MB (89316314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1514e9c8ee8928126cf584076b4cab9461c25df37b8683545d8a2d9ac1b80985`  
		Last Modified: Fri, 25 Feb 2022 17:45:59 GMT  
		Size: 3.5 KB (3460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db5d0528ce79652461e22b17f2f45f07fb01e18d7c0f9da5daca005a2b00f1f`  
		Last Modified: Fri, 25 Feb 2022 17:45:59 GMT  
		Size: 6.6 KB (6600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:d7621611bc109dad8983f5eb1e56f4a0f0fba0b95e1d6721c2e4687204dfe827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:008e0a5cd570889de96550f509a6a7a0cac1dbbf7e94265f5de497b45de97a1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128169486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ca1bb790d953c74b114c4ff3b7b5bdad99850bee6e9490e087c3abc57406d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:45:54 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 03:45:54 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 25 Feb 2022 19:02:20 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 19:02:20 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 19:02:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:02:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:02:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:02:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:02:56 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:02:57 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:02:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:02:57 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:02:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4becccd3dd4bfdd537199df53c49d74271a594ce337d1995892367406caf71`  
		Last Modified: Fri, 25 Feb 2022 19:08:19 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73da7c2ac5af5a9e3ba4bafa57276a54b5b51db2f48e9b4098d6fc542e7cef17`  
		Last Modified: Fri, 25 Feb 2022 19:08:33 GMT  
		Size: 88.2 MB (88243453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31163609685e6a5f3a3a18b64e38c1ac6a938f373308b6bf346e7abc80a3f157`  
		Last Modified: Fri, 25 Feb 2022 19:08:19 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9162f300b21308a5df5bb223206f4e2f3d2e251c179c6be1defdce49b111602`  
		Last Modified: Fri, 25 Feb 2022 19:08:19 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ae493c7b33cd9283f20896c891cf51ef8835e1d28742ba576b2435fd31dd5010
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125272637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:482dfce2aec58426a2445430dc5199dc257766a2f91890bd254b461a27d8b043`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:42:06 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 04:42:06 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 25 Feb 2022 17:41:40 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:41:41 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:41:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:41:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:16 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:17 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:18 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:19 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d49800d26cc57960935b2b51c925d67989ccf5ea2e6cb9efdaada4c97de7fe`  
		Last Modified: Fri, 25 Feb 2022 17:47:32 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f644e931eabfa9683592bffd84d2b6877afeb86e1d0a891fe930cd61e2240ba`  
		Last Modified: Fri, 25 Feb 2022 17:47:46 GMT  
		Size: 87.2 MB (87193233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0ecd2ff84ca16016cd11046f2bc070eefd4caa25f24dbc8b751962a8e2c741`  
		Last Modified: Fri, 25 Feb 2022 17:47:32 GMT  
		Size: 3.5 KB (3457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0e36c3d259009a7af93b32530988630438a12fd235661dc5c66cdc9268eb6b`  
		Last Modified: Fri, 25 Feb 2022 17:47:32 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:26365cfc20ce97ce9359b32d5774b0cd623e503cd1dc0a5ddbc065b92fa9e70a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137783748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737496717e740b26172016c9c63dbeb5ae8ee2a178eb689b4f8a4c9176d37b99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:14:03 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 06:14:05 GMT
ENV MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 06:14:07 GMT
ARG MARIADB_VERSION=1:10.6.5+maria~focal
# Wed, 02 Feb 2022 06:14:08 GMT
ENV MARIADB_VERSION=1:10.6.5+maria~focal
# Wed, 02 Feb 2022 06:14:11 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:14:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:16:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:17:15 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:17:18 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:17:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:17:28 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:17:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4683b2a4076da23a58c3d55ec3193591331e38c1da0cd871cb108e31c76984ec`  
		Last Modified: Wed, 02 Feb 2022 06:39:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cedf38ea121b3c6203ec8682b97afed76dc9815da29af531bf48951ecbed21`  
		Last Modified: Wed, 02 Feb 2022 06:39:57 GMT  
		Size: 91.6 MB (91579209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca079698384d698aa1ec8a2a18c8458fbed546951d84d331a3d168d4dd4acba`  
		Last Modified: Wed, 02 Feb 2022 06:39:39 GMT  
		Size: 5.6 KB (5626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:381ac4edf0b5ea109043605c9a6de2eec3f97de63d3b074f64d8b3401b128801
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127260924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff65a1eb5e3840fb92355287b2d21516d4ec40b7f92a676f906569915d4c602`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:02:03 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 02:02:03 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 25 Feb 2022 17:43:08 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:43:08 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:43:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:43:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:43:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:43:32 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:43:32 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:43:32 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:43:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:43:32 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:43:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124a747d11e0921bbf0eb728acae7edcd82997ff2e2f55fad0a6b88090a5e914`  
		Last Modified: Fri, 25 Feb 2022 17:45:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26577ed88062a982e95a549f67d31c62a66df5a03788d1dd2e8142893536b111`  
		Last Modified: Fri, 25 Feb 2022 17:46:12 GMT  
		Size: 89.3 MB (89316314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1514e9c8ee8928126cf584076b4cab9461c25df37b8683545d8a2d9ac1b80985`  
		Last Modified: Fri, 25 Feb 2022 17:45:59 GMT  
		Size: 3.5 KB (3460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db5d0528ce79652461e22b17f2f45f07fb01e18d7c0f9da5daca005a2b00f1f`  
		Last Modified: Fri, 25 Feb 2022 17:45:59 GMT  
		Size: 6.6 KB (6600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.7`

```console
$ docker pull mariadb@sha256:83258d2cd99e94128675aae598bc1cb30f444d5a215c0f0334e72940f3ee3988
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.6.7` - linux; amd64

```console
$ docker pull mariadb@sha256:008e0a5cd570889de96550f509a6a7a0cac1dbbf7e94265f5de497b45de97a1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128169486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ca1bb790d953c74b114c4ff3b7b5bdad99850bee6e9490e087c3abc57406d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:45:54 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 03:45:54 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 25 Feb 2022 19:02:20 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 19:02:20 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 19:02:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:02:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:02:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:02:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:02:56 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:02:57 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:02:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:02:57 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:02:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4becccd3dd4bfdd537199df53c49d74271a594ce337d1995892367406caf71`  
		Last Modified: Fri, 25 Feb 2022 19:08:19 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73da7c2ac5af5a9e3ba4bafa57276a54b5b51db2f48e9b4098d6fc542e7cef17`  
		Last Modified: Fri, 25 Feb 2022 19:08:33 GMT  
		Size: 88.2 MB (88243453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31163609685e6a5f3a3a18b64e38c1ac6a938f373308b6bf346e7abc80a3f157`  
		Last Modified: Fri, 25 Feb 2022 19:08:19 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9162f300b21308a5df5bb223206f4e2f3d2e251c179c6be1defdce49b111602`  
		Last Modified: Fri, 25 Feb 2022 19:08:19 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ae493c7b33cd9283f20896c891cf51ef8835e1d28742ba576b2435fd31dd5010
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125272637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:482dfce2aec58426a2445430dc5199dc257766a2f91890bd254b461a27d8b043`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:42:06 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 04:42:06 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 25 Feb 2022 17:41:40 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:41:41 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:41:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:41:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:16 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:17 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:18 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:19 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d49800d26cc57960935b2b51c925d67989ccf5ea2e6cb9efdaada4c97de7fe`  
		Last Modified: Fri, 25 Feb 2022 17:47:32 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f644e931eabfa9683592bffd84d2b6877afeb86e1d0a891fe930cd61e2240ba`  
		Last Modified: Fri, 25 Feb 2022 17:47:46 GMT  
		Size: 87.2 MB (87193233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0ecd2ff84ca16016cd11046f2bc070eefd4caa25f24dbc8b751962a8e2c741`  
		Last Modified: Fri, 25 Feb 2022 17:47:32 GMT  
		Size: 3.5 KB (3457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0e36c3d259009a7af93b32530988630438a12fd235661dc5c66cdc9268eb6b`  
		Last Modified: Fri, 25 Feb 2022 17:47:32 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; s390x

```console
$ docker pull mariadb@sha256:381ac4edf0b5ea109043605c9a6de2eec3f97de63d3b074f64d8b3401b128801
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127260924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff65a1eb5e3840fb92355287b2d21516d4ec40b7f92a676f906569915d4c602`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:02:03 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 02:02:03 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 25 Feb 2022 17:43:08 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:43:08 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:43:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:43:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:43:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:43:32 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:43:32 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:43:32 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:43:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:43:32 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:43:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124a747d11e0921bbf0eb728acae7edcd82997ff2e2f55fad0a6b88090a5e914`  
		Last Modified: Fri, 25 Feb 2022 17:45:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26577ed88062a982e95a549f67d31c62a66df5a03788d1dd2e8142893536b111`  
		Last Modified: Fri, 25 Feb 2022 17:46:12 GMT  
		Size: 89.3 MB (89316314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1514e9c8ee8928126cf584076b4cab9461c25df37b8683545d8a2d9ac1b80985`  
		Last Modified: Fri, 25 Feb 2022 17:45:59 GMT  
		Size: 3.5 KB (3460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db5d0528ce79652461e22b17f2f45f07fb01e18d7c0f9da5daca005a2b00f1f`  
		Last Modified: Fri, 25 Feb 2022 17:45:59 GMT  
		Size: 6.6 KB (6600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.7-focal`

```console
$ docker pull mariadb@sha256:83258d2cd99e94128675aae598bc1cb30f444d5a215c0f0334e72940f3ee3988
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.6.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:008e0a5cd570889de96550f509a6a7a0cac1dbbf7e94265f5de497b45de97a1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128169486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ca1bb790d953c74b114c4ff3b7b5bdad99850bee6e9490e087c3abc57406d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:45:54 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 03:45:54 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 25 Feb 2022 19:02:20 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 19:02:20 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 19:02:20 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:02:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:02:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:02:56 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:02:56 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:02:57 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:02:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:02:57 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:02:57 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4becccd3dd4bfdd537199df53c49d74271a594ce337d1995892367406caf71`  
		Last Modified: Fri, 25 Feb 2022 19:08:19 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73da7c2ac5af5a9e3ba4bafa57276a54b5b51db2f48e9b4098d6fc542e7cef17`  
		Last Modified: Fri, 25 Feb 2022 19:08:33 GMT  
		Size: 88.2 MB (88243453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31163609685e6a5f3a3a18b64e38c1ac6a938f373308b6bf346e7abc80a3f157`  
		Last Modified: Fri, 25 Feb 2022 19:08:19 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9162f300b21308a5df5bb223206f4e2f3d2e251c179c6be1defdce49b111602`  
		Last Modified: Fri, 25 Feb 2022 19:08:19 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ae493c7b33cd9283f20896c891cf51ef8835e1d28742ba576b2435fd31dd5010
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125272637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:482dfce2aec58426a2445430dc5199dc257766a2f91890bd254b461a27d8b043`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:42:06 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 04:42:06 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 25 Feb 2022 17:41:40 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:41:41 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:41:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:41:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:14 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:16 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:17 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:18 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:19 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d49800d26cc57960935b2b51c925d67989ccf5ea2e6cb9efdaada4c97de7fe`  
		Last Modified: Fri, 25 Feb 2022 17:47:32 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f644e931eabfa9683592bffd84d2b6877afeb86e1d0a891fe930cd61e2240ba`  
		Last Modified: Fri, 25 Feb 2022 17:47:46 GMT  
		Size: 87.2 MB (87193233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0ecd2ff84ca16016cd11046f2bc070eefd4caa25f24dbc8b751962a8e2c741`  
		Last Modified: Fri, 25 Feb 2022 17:47:32 GMT  
		Size: 3.5 KB (3457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0e36c3d259009a7af93b32530988630438a12fd235661dc5c66cdc9268eb6b`  
		Last Modified: Fri, 25 Feb 2022 17:47:32 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:381ac4edf0b5ea109043605c9a6de2eec3f97de63d3b074f64d8b3401b128801
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127260924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff65a1eb5e3840fb92355287b2d21516d4ec40b7f92a676f906569915d4c602`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:02:03 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 02:02:03 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 25 Feb 2022 17:43:08 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:43:08 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 25 Feb 2022 17:43:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:43:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:43:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:43:32 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:43:32 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:43:32 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:43:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:43:32 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:43:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124a747d11e0921bbf0eb728acae7edcd82997ff2e2f55fad0a6b88090a5e914`  
		Last Modified: Fri, 25 Feb 2022 17:45:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26577ed88062a982e95a549f67d31c62a66df5a03788d1dd2e8142893536b111`  
		Last Modified: Fri, 25 Feb 2022 17:46:12 GMT  
		Size: 89.3 MB (89316314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1514e9c8ee8928126cf584076b4cab9461c25df37b8683545d8a2d9ac1b80985`  
		Last Modified: Fri, 25 Feb 2022 17:45:59 GMT  
		Size: 3.5 KB (3460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db5d0528ce79652461e22b17f2f45f07fb01e18d7c0f9da5daca005a2b00f1f`  
		Last Modified: Fri, 25 Feb 2022 17:45:59 GMT  
		Size: 6.6 KB (6600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7`

```console
$ docker pull mariadb@sha256:0e210d47c39727cf1c21fdf739e6d0ca0f93831a0f77ce72f0f94181286871aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7` - linux; amd64

```console
$ docker pull mariadb@sha256:0fed5d91ed5beb07acfb64b268e29d4c958b2692cba3911c596d6021537e5149
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539871f8c20e7bf54159322bfe2b3c25eddb9f6ff61074c1ceeb42c9c81d96d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:45:03 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 03:45:04 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 19:01:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:01:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:02:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:02:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:02:12 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:02:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caac2a47a26c1d5ac110c8c8160d78c46633c515fabc02aeead42a929abb3f34`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d95be4fc3ed23b3da3e0b23d8207ff984583950c9f475029a113d470656273`  
		Last Modified: Fri, 25 Feb 2022 19:07:50 GMT  
		Size: 88.7 MB (88742109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1a87df3e4e40283a0f746897cbb88bfbd00077e0fa0548901288ab4bf7eee`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f323680a6eb6da7bb7518c7bc1e4ea7ed5ee8ae6d9743a0ab57b622438a3b788`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:63aaeb42ea87e3fcd3dc9b95d351db22517700c92df3361c2dfc02a9e5a80b9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125723761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ffdf1c8b8c51c02922ad33ef21d0d10f9b90be60cf34707f4ec8d44b6cd03e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:41:18 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 04:41:19 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:40:56 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:40:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:41:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:41:27 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:41:29 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:41:30 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:41:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:41:31 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:41:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d5701620936a9434a752e612b26e7ef401d732951312b4cb3ba8e0d56624b6`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a445807beccaa6654d95ccc8bb6a1200f1e1254b7dbace6227db6d2ddcdcf6`  
		Last Modified: Fri, 25 Feb 2022 17:46:58 GMT  
		Size: 87.6 MB (87644355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c712675c67566e4c76372be2b231f84dc1b13f6085a0f37c58638c4468f0cac`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea1c89bb7bfd6f10e08bb4a0e0b25a8c7c515a62ce859975be7258b7bef85ed`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e78f45a4fd3b6d3d5bf092d77d619cb5e87da4610cb05973595539351ab7b889
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138431241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1add620545f586c51173aa45cbb8f0f7722302aa7f01c0e6740ebd193cc33d4c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:10:08 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 06:10:12 GMT
ENV MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 06:10:15 GMT
ARG MARIADB_VERSION=1:10.7.1+maria~focal
# Wed, 02 Feb 2022 06:10:17 GMT
ENV MARIADB_VERSION=1:10.7.1+maria~focal
# Wed, 02 Feb 2022 06:10:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.1/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:10:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.1/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:13:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.1/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:13:31 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:13:33 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:13:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:13:39 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:13:44 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3da0822a098c42c0d8f9ca68906bb94fd6d49a76dd4a6b21b980ba7ba33d87`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb178f81363c8e872ae4193eac1a1f08bbaf95fea23ae74a8f7155c24ecfe030`  
		Last Modified: Wed, 02 Feb 2022 06:39:20 GMT  
		Size: 92.2 MB (92226700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752395e0c34c6e94de81e5c5783e7f0a8e972fb82fa795676a992f2b8da62e53`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 5.6 KB (5629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; s390x

```console
$ docker pull mariadb@sha256:86ecdcd726c86e5fdfd4a6e9d0806aa37120a54429b66fd9c4e917abc4fdc2fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127759644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c3482b60cba3773e4a8f8e0d1cdc804d03bb9b8e394a4cec25ab7f053d8b0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:01:20 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 02:01:20 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:42:33 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:42:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:58 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702f91bfef0abb95f814177f9a921283357b4afaa60cdb435acb8fe7a1402906`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543833eab2dd4901ece63b421429338ce5cca212daecd891f1ee2712a30b103`  
		Last Modified: Fri, 25 Feb 2022 17:45:35 GMT  
		Size: 89.8 MB (89815037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097c2f2236be70639eba7442cd4ceacf28eb6da74d1e88f4bef031bc88dd2150`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c175ac6918dcd13672765a8d1719eec85eeeca8fe4dffe912f427f6499d8d7`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 6.6 KB (6597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7-focal`

```console
$ docker pull mariadb@sha256:0e210d47c39727cf1c21fdf739e6d0ca0f93831a0f77ce72f0f94181286871aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:0fed5d91ed5beb07acfb64b268e29d4c958b2692cba3911c596d6021537e5149
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539871f8c20e7bf54159322bfe2b3c25eddb9f6ff61074c1ceeb42c9c81d96d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:45:03 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 03:45:04 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 19:01:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:01:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:02:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:02:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:02:12 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:02:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caac2a47a26c1d5ac110c8c8160d78c46633c515fabc02aeead42a929abb3f34`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d95be4fc3ed23b3da3e0b23d8207ff984583950c9f475029a113d470656273`  
		Last Modified: Fri, 25 Feb 2022 19:07:50 GMT  
		Size: 88.7 MB (88742109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1a87df3e4e40283a0f746897cbb88bfbd00077e0fa0548901288ab4bf7eee`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f323680a6eb6da7bb7518c7bc1e4ea7ed5ee8ae6d9743a0ab57b622438a3b788`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:63aaeb42ea87e3fcd3dc9b95d351db22517700c92df3361c2dfc02a9e5a80b9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125723761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ffdf1c8b8c51c02922ad33ef21d0d10f9b90be60cf34707f4ec8d44b6cd03e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:41:18 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 04:41:19 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:40:56 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:40:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:41:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:41:27 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:41:29 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:41:30 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:41:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:41:31 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:41:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d5701620936a9434a752e612b26e7ef401d732951312b4cb3ba8e0d56624b6`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a445807beccaa6654d95ccc8bb6a1200f1e1254b7dbace6227db6d2ddcdcf6`  
		Last Modified: Fri, 25 Feb 2022 17:46:58 GMT  
		Size: 87.6 MB (87644355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c712675c67566e4c76372be2b231f84dc1b13f6085a0f37c58638c4468f0cac`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea1c89bb7bfd6f10e08bb4a0e0b25a8c7c515a62ce859975be7258b7bef85ed`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e78f45a4fd3b6d3d5bf092d77d619cb5e87da4610cb05973595539351ab7b889
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138431241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1add620545f586c51173aa45cbb8f0f7722302aa7f01c0e6740ebd193cc33d4c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:10:08 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 06:10:12 GMT
ENV MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 06:10:15 GMT
ARG MARIADB_VERSION=1:10.7.1+maria~focal
# Wed, 02 Feb 2022 06:10:17 GMT
ENV MARIADB_VERSION=1:10.7.1+maria~focal
# Wed, 02 Feb 2022 06:10:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.1/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:10:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.1/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:13:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.1/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:13:31 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:13:33 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:13:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:13:39 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:13:44 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3da0822a098c42c0d8f9ca68906bb94fd6d49a76dd4a6b21b980ba7ba33d87`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb178f81363c8e872ae4193eac1a1f08bbaf95fea23ae74a8f7155c24ecfe030`  
		Last Modified: Wed, 02 Feb 2022 06:39:20 GMT  
		Size: 92.2 MB (92226700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752395e0c34c6e94de81e5c5783e7f0a8e972fb82fa795676a992f2b8da62e53`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 5.6 KB (5629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:86ecdcd726c86e5fdfd4a6e9d0806aa37120a54429b66fd9c4e917abc4fdc2fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127759644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c3482b60cba3773e4a8f8e0d1cdc804d03bb9b8e394a4cec25ab7f053d8b0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:01:20 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 02:01:20 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:42:33 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:42:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:58 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702f91bfef0abb95f814177f9a921283357b4afaa60cdb435acb8fe7a1402906`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543833eab2dd4901ece63b421429338ce5cca212daecd891f1ee2712a30b103`  
		Last Modified: Fri, 25 Feb 2022 17:45:35 GMT  
		Size: 89.8 MB (89815037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097c2f2236be70639eba7442cd4ceacf28eb6da74d1e88f4bef031bc88dd2150`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c175ac6918dcd13672765a8d1719eec85eeeca8fe4dffe912f427f6499d8d7`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 6.6 KB (6597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.3`

```console
$ docker pull mariadb@sha256:a91018842201436beb0d7c244558ed6887aefd2945835542f2e2eb3818680bad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.7.3` - linux; amd64

```console
$ docker pull mariadb@sha256:0fed5d91ed5beb07acfb64b268e29d4c958b2692cba3911c596d6021537e5149
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539871f8c20e7bf54159322bfe2b3c25eddb9f6ff61074c1ceeb42c9c81d96d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:45:03 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 03:45:04 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 19:01:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:01:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:02:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:02:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:02:12 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:02:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caac2a47a26c1d5ac110c8c8160d78c46633c515fabc02aeead42a929abb3f34`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d95be4fc3ed23b3da3e0b23d8207ff984583950c9f475029a113d470656273`  
		Last Modified: Fri, 25 Feb 2022 19:07:50 GMT  
		Size: 88.7 MB (88742109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1a87df3e4e40283a0f746897cbb88bfbd00077e0fa0548901288ab4bf7eee`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f323680a6eb6da7bb7518c7bc1e4ea7ed5ee8ae6d9743a0ab57b622438a3b788`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:63aaeb42ea87e3fcd3dc9b95d351db22517700c92df3361c2dfc02a9e5a80b9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125723761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ffdf1c8b8c51c02922ad33ef21d0d10f9b90be60cf34707f4ec8d44b6cd03e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:41:18 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 04:41:19 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:40:56 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:40:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:41:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:41:27 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:41:29 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:41:30 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:41:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:41:31 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:41:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d5701620936a9434a752e612b26e7ef401d732951312b4cb3ba8e0d56624b6`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a445807beccaa6654d95ccc8bb6a1200f1e1254b7dbace6227db6d2ddcdcf6`  
		Last Modified: Fri, 25 Feb 2022 17:46:58 GMT  
		Size: 87.6 MB (87644355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c712675c67566e4c76372be2b231f84dc1b13f6085a0f37c58638c4468f0cac`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea1c89bb7bfd6f10e08bb4a0e0b25a8c7c515a62ce859975be7258b7bef85ed`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3` - linux; s390x

```console
$ docker pull mariadb@sha256:86ecdcd726c86e5fdfd4a6e9d0806aa37120a54429b66fd9c4e917abc4fdc2fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127759644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c3482b60cba3773e4a8f8e0d1cdc804d03bb9b8e394a4cec25ab7f053d8b0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:01:20 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 02:01:20 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:42:33 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:42:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:58 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702f91bfef0abb95f814177f9a921283357b4afaa60cdb435acb8fe7a1402906`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543833eab2dd4901ece63b421429338ce5cca212daecd891f1ee2712a30b103`  
		Last Modified: Fri, 25 Feb 2022 17:45:35 GMT  
		Size: 89.8 MB (89815037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097c2f2236be70639eba7442cd4ceacf28eb6da74d1e88f4bef031bc88dd2150`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c175ac6918dcd13672765a8d1719eec85eeeca8fe4dffe912f427f6499d8d7`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 6.6 KB (6597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.3-focal`

```console
$ docker pull mariadb@sha256:a91018842201436beb0d7c244558ed6887aefd2945835542f2e2eb3818680bad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.7.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:0fed5d91ed5beb07acfb64b268e29d4c958b2692cba3911c596d6021537e5149
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539871f8c20e7bf54159322bfe2b3c25eddb9f6ff61074c1ceeb42c9c81d96d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:45:03 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 03:45:04 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 19:01:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:01:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:02:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:02:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:02:12 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:02:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caac2a47a26c1d5ac110c8c8160d78c46633c515fabc02aeead42a929abb3f34`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d95be4fc3ed23b3da3e0b23d8207ff984583950c9f475029a113d470656273`  
		Last Modified: Fri, 25 Feb 2022 19:07:50 GMT  
		Size: 88.7 MB (88742109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1a87df3e4e40283a0f746897cbb88bfbd00077e0fa0548901288ab4bf7eee`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f323680a6eb6da7bb7518c7bc1e4ea7ed5ee8ae6d9743a0ab57b622438a3b788`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:63aaeb42ea87e3fcd3dc9b95d351db22517700c92df3361c2dfc02a9e5a80b9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125723761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ffdf1c8b8c51c02922ad33ef21d0d10f9b90be60cf34707f4ec8d44b6cd03e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:41:18 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 04:41:19 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:40:56 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:40:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:41:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:41:27 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:41:29 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:41:30 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:41:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:41:31 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:41:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d5701620936a9434a752e612b26e7ef401d732951312b4cb3ba8e0d56624b6`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a445807beccaa6654d95ccc8bb6a1200f1e1254b7dbace6227db6d2ddcdcf6`  
		Last Modified: Fri, 25 Feb 2022 17:46:58 GMT  
		Size: 87.6 MB (87644355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c712675c67566e4c76372be2b231f84dc1b13f6085a0f37c58638c4468f0cac`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea1c89bb7bfd6f10e08bb4a0e0b25a8c7c515a62ce859975be7258b7bef85ed`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:86ecdcd726c86e5fdfd4a6e9d0806aa37120a54429b66fd9c4e917abc4fdc2fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127759644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c3482b60cba3773e4a8f8e0d1cdc804d03bb9b8e394a4cec25ab7f053d8b0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:01:20 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 02:01:20 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:42:33 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:42:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:58 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702f91bfef0abb95f814177f9a921283357b4afaa60cdb435acb8fe7a1402906`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543833eab2dd4901ece63b421429338ce5cca212daecd891f1ee2712a30b103`  
		Last Modified: Fri, 25 Feb 2022 17:45:35 GMT  
		Size: 89.8 MB (89815037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097c2f2236be70639eba7442cd4ceacf28eb6da74d1e88f4bef031bc88dd2150`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c175ac6918dcd13672765a8d1719eec85eeeca8fe4dffe912f427f6499d8d7`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 6.6 KB (6597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8`

```console
$ docker pull mariadb@sha256:bbd7b2a604239bacedd60b1378eeba076a20c635d293869b62a0267eb1db4d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.8` - linux; amd64

```console
$ docker pull mariadb@sha256:3b0bcb3cfed690280020b6debb452e402756e6d350b5cfd301e6105d556bcee1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51adad759c7457e217a7b467f682591800c1f888c81f8beb556b5a8f02700b9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 25 Feb 2022 19:00:29 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 19:00:30 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 19:00:30 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 19:00:30 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 19:00:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:00:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:01:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:01:30 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:01:31 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:01:31 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:01:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:01:32 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:01:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ee39c28fa6926da814ff529e574f7f087bfd03170725480bffcf19d523d08a`  
		Last Modified: Fri, 25 Feb 2022 19:07:03 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee45abd643a594ebf03c5067e2edc2b83bb508140778c4cee469f538f9e0c3e`  
		Last Modified: Fri, 25 Feb 2022 19:07:19 GMT  
		Size: 88.7 MB (88652054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f20114a997595499acdcb7fb3eee18d1f5c30d727cc02b3aae8fa9db79907e`  
		Last Modified: Fri, 25 Feb 2022 19:07:03 GMT  
		Size: 3.5 KB (3457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59b42092777a064b3944b8cf22107aa0fe97925f2354106daf2bfac8b63d5d5`  
		Last Modified: Fri, 25 Feb 2022 19:07:02 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f82d88b95bcd3c8804bbdc63dbc1601170099a43a278188151f310f43533eac6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125653695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f72cfff79518f8f68b99d313d1610bbf91ef8f2775db84bf4fd44b30d56c870`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 25 Feb 2022 17:40:05 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:40:05 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:40:06 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:40:07 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:40:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:40:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:40:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:40:39 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:40:41 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:40:42 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:40:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:40:43 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:40:44 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf563ddfeccb077f605d11cb85db1f63dde8f511a61ac8c6b9068a3ceb696c5f`  
		Last Modified: Fri, 25 Feb 2022 17:46:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018598e8609f71798ea3313231b403bac97cb7a512e2bbff25f4e842ca9369c1`  
		Last Modified: Fri, 25 Feb 2022 17:46:27 GMT  
		Size: 87.6 MB (87574287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a5af72a81bd3494765615960a78d9a9b2bed0209154826d8a8032c730ceb10`  
		Last Modified: Fri, 25 Feb 2022 17:46:13 GMT  
		Size: 3.5 KB (3458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b1ccae977bfbeba1ccdf69a8f33ba095abc7a765d0068d195decdb9f2782cd`  
		Last Modified: Fri, 25 Feb 2022 17:46:13 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; s390x

```console
$ docker pull mariadb@sha256:40af03fb20c513533052ace03ed7a22e6388155af56677841aae040401c1b987
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127724127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d230b13c83f22c7fdc3637bf5e2e088b2a74a7eadf8151e0be308f8c07043e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 25 Feb 2022 17:41:48 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:41:49 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:41:49 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:41:50 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:41:50 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:41:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:22 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:23 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:23 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:23 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fc756bd7cc38827f64e2e9271c3a39e72cb00a329f75cf8d122bbc8d3df32a`  
		Last Modified: Fri, 25 Feb 2022 17:44:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf11b0e320f1600632a2c68dacfadf3ebf1d1f4d2fa617c961143de2badf2924`  
		Last Modified: Fri, 25 Feb 2022 17:45:06 GMT  
		Size: 89.8 MB (89779518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d51d433e94e8e372d5aacaeb38bdfebd01d572ca4439ee1b924422426f9559`  
		Last Modified: Fri, 25 Feb 2022 17:44:53 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c583ef5d28b7f43d39033283bdbb71b3ae4caa93a2b99ef45cc76c23d43ec4`  
		Last Modified: Fri, 25 Feb 2022 17:44:53 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8-focal`

```console
$ docker pull mariadb@sha256:bbd7b2a604239bacedd60b1378eeba076a20c635d293869b62a0267eb1db4d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.8-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:3b0bcb3cfed690280020b6debb452e402756e6d350b5cfd301e6105d556bcee1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51adad759c7457e217a7b467f682591800c1f888c81f8beb556b5a8f02700b9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 25 Feb 2022 19:00:29 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 19:00:30 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 19:00:30 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 19:00:30 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 19:00:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:00:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:01:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:01:30 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:01:31 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:01:31 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:01:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:01:32 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:01:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ee39c28fa6926da814ff529e574f7f087bfd03170725480bffcf19d523d08a`  
		Last Modified: Fri, 25 Feb 2022 19:07:03 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee45abd643a594ebf03c5067e2edc2b83bb508140778c4cee469f538f9e0c3e`  
		Last Modified: Fri, 25 Feb 2022 19:07:19 GMT  
		Size: 88.7 MB (88652054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f20114a997595499acdcb7fb3eee18d1f5c30d727cc02b3aae8fa9db79907e`  
		Last Modified: Fri, 25 Feb 2022 19:07:03 GMT  
		Size: 3.5 KB (3457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59b42092777a064b3944b8cf22107aa0fe97925f2354106daf2bfac8b63d5d5`  
		Last Modified: Fri, 25 Feb 2022 19:07:02 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f82d88b95bcd3c8804bbdc63dbc1601170099a43a278188151f310f43533eac6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125653695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f72cfff79518f8f68b99d313d1610bbf91ef8f2775db84bf4fd44b30d56c870`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 25 Feb 2022 17:40:05 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:40:05 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:40:06 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:40:07 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:40:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:40:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:40:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:40:39 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:40:41 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:40:42 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:40:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:40:43 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:40:44 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf563ddfeccb077f605d11cb85db1f63dde8f511a61ac8c6b9068a3ceb696c5f`  
		Last Modified: Fri, 25 Feb 2022 17:46:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018598e8609f71798ea3313231b403bac97cb7a512e2bbff25f4e842ca9369c1`  
		Last Modified: Fri, 25 Feb 2022 17:46:27 GMT  
		Size: 87.6 MB (87574287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a5af72a81bd3494765615960a78d9a9b2bed0209154826d8a8032c730ceb10`  
		Last Modified: Fri, 25 Feb 2022 17:46:13 GMT  
		Size: 3.5 KB (3458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b1ccae977bfbeba1ccdf69a8f33ba095abc7a765d0068d195decdb9f2782cd`  
		Last Modified: Fri, 25 Feb 2022 17:46:13 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:40af03fb20c513533052ace03ed7a22e6388155af56677841aae040401c1b987
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127724127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d230b13c83f22c7fdc3637bf5e2e088b2a74a7eadf8151e0be308f8c07043e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 25 Feb 2022 17:41:48 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:41:49 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:41:49 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:41:50 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:41:50 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:41:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:22 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:23 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:23 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:23 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fc756bd7cc38827f64e2e9271c3a39e72cb00a329f75cf8d122bbc8d3df32a`  
		Last Modified: Fri, 25 Feb 2022 17:44:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf11b0e320f1600632a2c68dacfadf3ebf1d1f4d2fa617c961143de2badf2924`  
		Last Modified: Fri, 25 Feb 2022 17:45:06 GMT  
		Size: 89.8 MB (89779518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d51d433e94e8e372d5aacaeb38bdfebd01d572ca4439ee1b924422426f9559`  
		Last Modified: Fri, 25 Feb 2022 17:44:53 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c583ef5d28b7f43d39033283bdbb71b3ae4caa93a2b99ef45cc76c23d43ec4`  
		Last Modified: Fri, 25 Feb 2022 17:44:53 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.2`

```console
$ docker pull mariadb@sha256:bbd7b2a604239bacedd60b1378eeba076a20c635d293869b62a0267eb1db4d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.8.2` - linux; amd64

```console
$ docker pull mariadb@sha256:3b0bcb3cfed690280020b6debb452e402756e6d350b5cfd301e6105d556bcee1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51adad759c7457e217a7b467f682591800c1f888c81f8beb556b5a8f02700b9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 25 Feb 2022 19:00:29 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 19:00:30 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 19:00:30 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 19:00:30 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 19:00:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:00:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:01:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:01:30 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:01:31 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:01:31 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:01:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:01:32 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:01:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ee39c28fa6926da814ff529e574f7f087bfd03170725480bffcf19d523d08a`  
		Last Modified: Fri, 25 Feb 2022 19:07:03 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee45abd643a594ebf03c5067e2edc2b83bb508140778c4cee469f538f9e0c3e`  
		Last Modified: Fri, 25 Feb 2022 19:07:19 GMT  
		Size: 88.7 MB (88652054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f20114a997595499acdcb7fb3eee18d1f5c30d727cc02b3aae8fa9db79907e`  
		Last Modified: Fri, 25 Feb 2022 19:07:03 GMT  
		Size: 3.5 KB (3457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59b42092777a064b3944b8cf22107aa0fe97925f2354106daf2bfac8b63d5d5`  
		Last Modified: Fri, 25 Feb 2022 19:07:02 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f82d88b95bcd3c8804bbdc63dbc1601170099a43a278188151f310f43533eac6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125653695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f72cfff79518f8f68b99d313d1610bbf91ef8f2775db84bf4fd44b30d56c870`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 25 Feb 2022 17:40:05 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:40:05 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:40:06 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:40:07 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:40:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:40:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:40:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:40:39 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:40:41 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:40:42 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:40:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:40:43 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:40:44 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf563ddfeccb077f605d11cb85db1f63dde8f511a61ac8c6b9068a3ceb696c5f`  
		Last Modified: Fri, 25 Feb 2022 17:46:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018598e8609f71798ea3313231b403bac97cb7a512e2bbff25f4e842ca9369c1`  
		Last Modified: Fri, 25 Feb 2022 17:46:27 GMT  
		Size: 87.6 MB (87574287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a5af72a81bd3494765615960a78d9a9b2bed0209154826d8a8032c730ceb10`  
		Last Modified: Fri, 25 Feb 2022 17:46:13 GMT  
		Size: 3.5 KB (3458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b1ccae977bfbeba1ccdf69a8f33ba095abc7a765d0068d195decdb9f2782cd`  
		Last Modified: Fri, 25 Feb 2022 17:46:13 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2` - linux; s390x

```console
$ docker pull mariadb@sha256:40af03fb20c513533052ace03ed7a22e6388155af56677841aae040401c1b987
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127724127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d230b13c83f22c7fdc3637bf5e2e088b2a74a7eadf8151e0be308f8c07043e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 25 Feb 2022 17:41:48 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:41:49 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:41:49 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:41:50 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:41:50 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:41:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:22 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:23 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:23 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:23 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fc756bd7cc38827f64e2e9271c3a39e72cb00a329f75cf8d122bbc8d3df32a`  
		Last Modified: Fri, 25 Feb 2022 17:44:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf11b0e320f1600632a2c68dacfadf3ebf1d1f4d2fa617c961143de2badf2924`  
		Last Modified: Fri, 25 Feb 2022 17:45:06 GMT  
		Size: 89.8 MB (89779518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d51d433e94e8e372d5aacaeb38bdfebd01d572ca4439ee1b924422426f9559`  
		Last Modified: Fri, 25 Feb 2022 17:44:53 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c583ef5d28b7f43d39033283bdbb71b3ae4caa93a2b99ef45cc76c23d43ec4`  
		Last Modified: Fri, 25 Feb 2022 17:44:53 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.2-focal`

```console
$ docker pull mariadb@sha256:bbd7b2a604239bacedd60b1378eeba076a20c635d293869b62a0267eb1db4d23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mariadb:10.8.2-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:3b0bcb3cfed690280020b6debb452e402756e6d350b5cfd301e6105d556bcee1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128578092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51adad759c7457e217a7b467f682591800c1f888c81f8beb556b5a8f02700b9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 25 Feb 2022 19:00:29 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 19:00:30 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 19:00:30 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 19:00:30 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 19:00:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:00:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:01:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:01:30 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:01:31 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:01:31 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:01:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:01:32 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:01:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ee39c28fa6926da814ff529e574f7f087bfd03170725480bffcf19d523d08a`  
		Last Modified: Fri, 25 Feb 2022 19:07:03 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee45abd643a594ebf03c5067e2edc2b83bb508140778c4cee469f538f9e0c3e`  
		Last Modified: Fri, 25 Feb 2022 19:07:19 GMT  
		Size: 88.7 MB (88652054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f20114a997595499acdcb7fb3eee18d1f5c30d727cc02b3aae8fa9db79907e`  
		Last Modified: Fri, 25 Feb 2022 19:07:03 GMT  
		Size: 3.5 KB (3457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59b42092777a064b3944b8cf22107aa0fe97925f2354106daf2bfac8b63d5d5`  
		Last Modified: Fri, 25 Feb 2022 19:07:02 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f82d88b95bcd3c8804bbdc63dbc1601170099a43a278188151f310f43533eac6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125653695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f72cfff79518f8f68b99d313d1610bbf91ef8f2775db84bf4fd44b30d56c870`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 25 Feb 2022 17:40:05 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:40:05 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:40:06 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:40:07 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:40:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:40:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:40:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:40:39 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:40:41 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:40:42 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:40:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:40:43 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:40:44 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf563ddfeccb077f605d11cb85db1f63dde8f511a61ac8c6b9068a3ceb696c5f`  
		Last Modified: Fri, 25 Feb 2022 17:46:13 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018598e8609f71798ea3313231b403bac97cb7a512e2bbff25f4e842ca9369c1`  
		Last Modified: Fri, 25 Feb 2022 17:46:27 GMT  
		Size: 87.6 MB (87574287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a5af72a81bd3494765615960a78d9a9b2bed0209154826d8a8032c730ceb10`  
		Last Modified: Fri, 25 Feb 2022 17:46:13 GMT  
		Size: 3.5 KB (3458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b1ccae977bfbeba1ccdf69a8f33ba095abc7a765d0068d195decdb9f2782cd`  
		Last Modified: Fri, 25 Feb 2022 17:46:13 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:40af03fb20c513533052ace03ed7a22e6388155af56677841aae040401c1b987
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127724127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d230b13c83f22c7fdc3637bf5e2e088b2a74a7eadf8151e0be308f8c07043e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 25 Feb 2022 17:41:48 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:41:49 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 25 Feb 2022 17:41:49 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:41:50 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 25 Feb 2022 17:41:50 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:41:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:18 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:22 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:23 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:23 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:23 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fc756bd7cc38827f64e2e9271c3a39e72cb00a329f75cf8d122bbc8d3df32a`  
		Last Modified: Fri, 25 Feb 2022 17:44:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf11b0e320f1600632a2c68dacfadf3ebf1d1f4d2fa617c961143de2badf2924`  
		Last Modified: Fri, 25 Feb 2022 17:45:06 GMT  
		Size: 89.8 MB (89779518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d51d433e94e8e372d5aacaeb38bdfebd01d572ca4439ee1b924422426f9559`  
		Last Modified: Fri, 25 Feb 2022 17:44:53 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c583ef5d28b7f43d39033283bdbb71b3ae4caa93a2b99ef45cc76c23d43ec4`  
		Last Modified: Fri, 25 Feb 2022 17:44:53 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:9e1b5f318c0255eae6bb0877b0762c560cde9f7e6186f673060189761202615a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:0fed5d91ed5beb07acfb64b268e29d4c958b2692cba3911c596d6021537e5149
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539871f8c20e7bf54159322bfe2b3c25eddb9f6ff61074c1ceeb42c9c81d96d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:45:03 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 03:45:04 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 19:01:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:01:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:02:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:02:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:02:12 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:02:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caac2a47a26c1d5ac110c8c8160d78c46633c515fabc02aeead42a929abb3f34`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d95be4fc3ed23b3da3e0b23d8207ff984583950c9f475029a113d470656273`  
		Last Modified: Fri, 25 Feb 2022 19:07:50 GMT  
		Size: 88.7 MB (88742109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1a87df3e4e40283a0f746897cbb88bfbd00077e0fa0548901288ab4bf7eee`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f323680a6eb6da7bb7518c7bc1e4ea7ed5ee8ae6d9743a0ab57b622438a3b788`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:63aaeb42ea87e3fcd3dc9b95d351db22517700c92df3361c2dfc02a9e5a80b9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125723761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ffdf1c8b8c51c02922ad33ef21d0d10f9b90be60cf34707f4ec8d44b6cd03e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:41:18 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 04:41:19 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:40:56 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:40:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:41:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:41:27 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:41:29 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:41:30 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:41:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:41:31 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:41:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d5701620936a9434a752e612b26e7ef401d732951312b4cb3ba8e0d56624b6`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a445807beccaa6654d95ccc8bb6a1200f1e1254b7dbace6227db6d2ddcdcf6`  
		Last Modified: Fri, 25 Feb 2022 17:46:58 GMT  
		Size: 87.6 MB (87644355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c712675c67566e4c76372be2b231f84dc1b13f6085a0f37c58638c4468f0cac`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea1c89bb7bfd6f10e08bb4a0e0b25a8c7c515a62ce859975be7258b7bef85ed`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:26365cfc20ce97ce9359b32d5774b0cd623e503cd1dc0a5ddbc065b92fa9e70a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137783748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737496717e740b26172016c9c63dbeb5ae8ee2a178eb689b4f8a4c9176d37b99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:14:03 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 06:14:05 GMT
ENV MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 06:14:07 GMT
ARG MARIADB_VERSION=1:10.6.5+maria~focal
# Wed, 02 Feb 2022 06:14:08 GMT
ENV MARIADB_VERSION=1:10.6.5+maria~focal
# Wed, 02 Feb 2022 06:14:11 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:14:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:16:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:17:15 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:17:18 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:17:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:17:28 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:17:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4683b2a4076da23a58c3d55ec3193591331e38c1da0cd871cb108e31c76984ec`  
		Last Modified: Wed, 02 Feb 2022 06:39:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cedf38ea121b3c6203ec8682b97afed76dc9815da29af531bf48951ecbed21`  
		Last Modified: Wed, 02 Feb 2022 06:39:57 GMT  
		Size: 91.6 MB (91579209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca079698384d698aa1ec8a2a18c8458fbed546951d84d331a3d168d4dd4acba`  
		Last Modified: Wed, 02 Feb 2022 06:39:39 GMT  
		Size: 5.6 KB (5626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; s390x

```console
$ docker pull mariadb@sha256:86ecdcd726c86e5fdfd4a6e9d0806aa37120a54429b66fd9c4e917abc4fdc2fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127759644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c3482b60cba3773e4a8f8e0d1cdc804d03bb9b8e394a4cec25ab7f053d8b0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:01:20 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 02:01:20 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:42:33 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:42:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:58 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702f91bfef0abb95f814177f9a921283357b4afaa60cdb435acb8fe7a1402906`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543833eab2dd4901ece63b421429338ce5cca212daecd891f1ee2712a30b103`  
		Last Modified: Fri, 25 Feb 2022 17:45:35 GMT  
		Size: 89.8 MB (89815037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097c2f2236be70639eba7442cd4ceacf28eb6da74d1e88f4bef031bc88dd2150`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c175ac6918dcd13672765a8d1719eec85eeeca8fe4dffe912f427f6499d8d7`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 6.6 KB (6597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:9e1b5f318c0255eae6bb0877b0762c560cde9f7e6186f673060189761202615a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:0fed5d91ed5beb07acfb64b268e29d4c958b2692cba3911c596d6021537e5149
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128668144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:539871f8c20e7bf54159322bfe2b3c25eddb9f6ff61074c1ceeb42c9c81d96d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 03:44:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 03:44:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:10 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 03:44:22 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 03:44:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 03:44:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 03:44:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 03:45:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 03:45:03 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 03:45:04 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 19:01:39 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 19:01:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 19:01:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 19:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 19:02:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 19:02:11 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 19:02:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 19:02:12 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 19:02:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bcb14c13a16d41b62e37e326b8a6f8c624abc25a69c124f4adc0efe20cd699`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c56760f8795a481e78e45a17a5be161f3e783bc3706500c78438d786664145`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 5.5 MB (5488714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95000a218fc379d12546e703c2c5053c762fa18cd2b4f9bdbd18262de3ab830`  
		Last Modified: Wed, 02 Feb 2022 03:50:45 GMT  
		Size: 3.6 MB (3585297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765d76e68d91020e9f23c79d526959e31827ebb8beaa3c2dbdab96e0b3fcb49`  
		Last Modified: Wed, 02 Feb 2022 03:50:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6945738f085b358ec9b3e38bcdd7791eec1d2a390d686f16c498dc512b39cd8`  
		Last Modified: Wed, 02 Feb 2022 03:50:43 GMT  
		Size: 2.3 MB (2273154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62787b7c58c5b4583c32aae1c05a7754bbe015bcc7befeadb18724d1d30b880f`  
		Last Modified: Wed, 02 Feb 2022 03:50:42 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caac2a47a26c1d5ac110c8c8160d78c46633c515fabc02aeead42a929abb3f34`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d95be4fc3ed23b3da3e0b23d8207ff984583950c9f475029a113d470656273`  
		Last Modified: Fri, 25 Feb 2022 19:07:50 GMT  
		Size: 88.7 MB (88742109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1a87df3e4e40283a0f746897cbb88bfbd00077e0fa0548901288ab4bf7eee`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 3.5 KB (3456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f323680a6eb6da7bb7518c7bc1e4ea7ed5ee8ae6d9743a0ab57b622438a3b788`  
		Last Modified: Fri, 25 Feb 2022 19:07:35 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:63aaeb42ea87e3fcd3dc9b95d351db22517700c92df3361c2dfc02a9e5a80b9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125723761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ffdf1c8b8c51c02922ad33ef21d0d10f9b90be60cf34707f4ec8d44b6cd03e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 04:39:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 04:40:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 04:40:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 04:40:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 04:40:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 04:40:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 04:41:17 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 04:41:18 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 04:41:19 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:40:56 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:57 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:40:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:40:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:41:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:41:27 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:41:29 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:41:30 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:41:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:41:31 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:41:32 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f406123c735827ddca5013c4dbaec303a0bbde59e31c312fe60c4a3c4eeef62c`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414755d47c502f9964427595a679ddd698eff61c209060f6955a264d4ee98981`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 5.3 MB (5320804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72e3f9adedebed74ad9cc9b32baa8e4bdd52883d9faff9419213a4b6a5e82a`  
		Last Modified: Wed, 02 Feb 2022 04:57:34 GMT  
		Size: 3.4 MB (3370594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b1182692e22e0260cdfb1a4f2257ae7d2dcccc416216bc53eec22a1d5a48`  
		Last Modified: Wed, 02 Feb 2022 04:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620b0eb464ebca108fe2b78540a25bc563ea53b8c917bb9174e44344bff9775`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.2 MB (2203676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c610e5ec0f6e73427891b2add972f5779ba9e99583f0a6c4c657d8532eda6c`  
		Last Modified: Wed, 02 Feb 2022 04:57:31 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d5701620936a9434a752e612b26e7ef401d732951312b4cb3ba8e0d56624b6`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a445807beccaa6654d95ccc8bb6a1200f1e1254b7dbace6227db6d2ddcdcf6`  
		Last Modified: Fri, 25 Feb 2022 17:46:58 GMT  
		Size: 87.6 MB (87644355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c712675c67566e4c76372be2b231f84dc1b13f6085a0f37c58638c4468f0cac`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea1c89bb7bfd6f10e08bb4a0e0b25a8c7c515a62ce859975be7258b7bef85ed`  
		Last Modified: Fri, 25 Feb 2022 17:46:45 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:26365cfc20ce97ce9359b32d5774b0cd623e503cd1dc0a5ddbc065b92fa9e70a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137783748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737496717e740b26172016c9c63dbeb5ae8ee2a178eb689b4f8a4c9176d37b99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 06:07:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 06:08:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:08:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 06:09:21 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 06:09:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 06:09:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 06:09:55 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 06:10:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 06:14:03 GMT
ARG MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 06:14:05 GMT
ENV MARIADB_MAJOR=10.6
# Wed, 02 Feb 2022 06:14:07 GMT
ARG MARIADB_VERSION=1:10.6.5+maria~focal
# Wed, 02 Feb 2022 06:14:08 GMT
ENV MARIADB_VERSION=1:10.6.5+maria~focal
# Wed, 02 Feb 2022 06:14:11 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
# Wed, 02 Feb 2022 06:14:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Feb 2022 06:16:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Feb 2022 06:17:15 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Feb 2022 06:17:18 GMT
COPY file:3d431099953246ba9f86475bec3d0dd982f00a61aadadc1bc6d8c1083ec64129 in /usr/local/bin/ 
# Wed, 02 Feb 2022 06:17:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 06:17:28 GMT
EXPOSE 3306
# Wed, 02 Feb 2022 06:17:31 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa6ddf04a6d9ff5571f3581411a5c5599f359efc06218aa8d7c98b19a55901`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ae472154410dbc918378510614e56d08dd8a080b560ff9c32dda5245513274`  
		Last Modified: Wed, 02 Feb 2022 06:39:05 GMT  
		Size: 6.7 MB (6667616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e257a32b5e76c486ebf42a085bb256e66387304f2229a5ea755f81fd4ff043`  
		Last Modified: Wed, 02 Feb 2022 06:39:04 GMT  
		Size: 3.7 MB (3672907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ba19c6c72ddf1ef6540af7465f5ebce217aa9ae4262681c6f8dab092d1c4f2`  
		Last Modified: Wed, 02 Feb 2022 06:39:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a1d4520ce5fb6b4de48cceee5ec288b0d16ed237ac7a5803a60e47a5b30485`  
		Last Modified: Wed, 02 Feb 2022 06:39:01 GMT  
		Size: 2.6 MB (2568961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e484cec9b927076854980caeef8520dfe1aa90b9caf1af6321de484c1afd41`  
		Last Modified: Wed, 02 Feb 2022 06:39:00 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4683b2a4076da23a58c3d55ec3193591331e38c1da0cd871cb108e31c76984ec`  
		Last Modified: Wed, 02 Feb 2022 06:39:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cedf38ea121b3c6203ec8682b97afed76dc9815da29af531bf48951ecbed21`  
		Last Modified: Wed, 02 Feb 2022 06:39:57 GMT  
		Size: 91.6 MB (91579209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca079698384d698aa1ec8a2a18c8458fbed546951d84d331a3d168d4dd4acba`  
		Last Modified: Wed, 02 Feb 2022 06:39:39 GMT  
		Size: 5.6 KB (5626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:86ecdcd726c86e5fdfd4a6e9d0806aa37120a54429b66fd9c4e917abc4fdc2fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127759644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c3482b60cba3773e4a8f8e0d1cdc804d03bb9b8e394a4cec25ab7f053d8b0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:00:15 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Feb 2022 02:00:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Feb 2022 02:00:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Feb 2022 02:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Feb 2022 02:00:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 02:00:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Feb 2022 02:01:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Feb 2022 02:01:20 GMT
ARG MARIADB_MAJOR=10.7
# Wed, 02 Feb 2022 02:01:20 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 25 Feb 2022 17:42:33 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 25 Feb 2022 17:42:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 25 Feb 2022 17:42:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 25 Feb 2022 17:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 25 Feb 2022 17:42:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:f693e5845f70db80415072fbc1b9ad23eb585c105d71de03f85effee169e3220 in /usr/local/bin/healthcheck.sh 
# Fri, 25 Feb 2022 17:42:58 GMT
COPY file:d5d79d09980467bc2d89c305ca6c877b5500a08d8bfc8e1accc338acff89339f in /usr/local/bin/ 
# Fri, 25 Feb 2022 17:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Feb 2022 17:42:58 GMT
EXPOSE 3306
# Fri, 25 Feb 2022 17:42:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efba31bb782a719396206842603ef1b2a8a771ab834a5eceff66d64f0a5918f`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54055a30f227d69198e91da1931c1ee5d7effcbc8f0ad640a2dbb2b5ba57f7`  
		Last Modified: Wed, 02 Feb 2022 02:04:00 GMT  
		Size: 5.4 MB (5380988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1175de9b14ef6cc481f92baa7df6265e3348404e267fd8607ff1a48cd81f9791`  
		Last Modified: Wed, 02 Feb 2022 02:04:02 GMT  
		Size: 3.2 MB (3244533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8905d7a3550001eeac1668b17f2089d9dfe90316c19d635333e81d4a3f70dbe0`  
		Last Modified: Wed, 02 Feb 2022 02:03:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27deea83714266cb24dd1fe4acbbfa21514b978790242c8b83cc5c85eae85472`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.2 MB (2185574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b06a0b2eb1cb2dea04f21477e6c1ebead902b9d5db32337e092dcfb65bce74`  
		Last Modified: Wed, 02 Feb 2022 02:03:58 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702f91bfef0abb95f814177f9a921283357b4afaa60cdb435acb8fe7a1402906`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b543833eab2dd4901ece63b421429338ce5cca212daecd891f1ee2712a30b103`  
		Last Modified: Fri, 25 Feb 2022 17:45:35 GMT  
		Size: 89.8 MB (89815037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097c2f2236be70639eba7442cd4ceacf28eb6da74d1e88f4bef031bc88dd2150`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 3.5 KB (3459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c175ac6918dcd13672765a8d1719eec85eeeca8fe4dffe912f427f6499d8d7`  
		Last Modified: Fri, 25 Feb 2022 17:45:23 GMT  
		Size: 6.6 KB (6597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
