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
