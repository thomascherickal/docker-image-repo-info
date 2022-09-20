<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10-jammy`](#mariadb10-jammy)
-	[`mariadb:10.10-rc`](#mariadb1010-rc)
-	[`mariadb:10.10-rc-jammy`](#mariadb1010-rc-jammy)
-	[`mariadb:10.10.1-rc`](#mariadb10101-rc)
-	[`mariadb:10.10.1-rc-jammy`](#mariadb10101-rc-jammy)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.3.36`](#mariadb10336)
-	[`mariadb:10.3.36-focal`](#mariadb10336-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.4.26`](#mariadb10426)
-	[`mariadb:10.4.26-focal`](#mariadb10426-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10.5.17`](#mariadb10517)
-	[`mariadb:10.5.17-focal`](#mariadb10517-focal)
-	[`mariadb:10.6`](#mariadb106)
-	[`mariadb:10.6-focal`](#mariadb106-focal)
-	[`mariadb:10.6.10`](#mariadb10610)
-	[`mariadb:10.6.10-focal`](#mariadb10610-focal)
-	[`mariadb:10.7`](#mariadb107)
-	[`mariadb:10.7-focal`](#mariadb107-focal)
-	[`mariadb:10.7.6`](#mariadb1076)
-	[`mariadb:10.7.6-focal`](#mariadb1076-focal)
-	[`mariadb:10.8`](#mariadb108)
-	[`mariadb:10.8-jammy`](#mariadb108-jammy)
-	[`mariadb:10.8.5`](#mariadb1085)
-	[`mariadb:10.8.5-jammy`](#mariadb1085-jammy)
-	[`mariadb:10.9`](#mariadb109)
-	[`mariadb:10.9-jammy`](#mariadb109-jammy)
-	[`mariadb:10.9.3`](#mariadb1093)
-	[`mariadb:10.9.3-jammy`](#mariadb1093-jammy)
-	[`mariadb:jammy`](#mariadbjammy)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:ca04948aca834499f728692520eff82917de1d768b47751ba4dd0fc5f261c8e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:7e613e248abdf4604776d6ace8eba9998b61b44f3c6cfd7121939c2fc3f1a7d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (124013572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c284e5e829612878511aa9fc0c383708c5a68f2167fa77a515bc2e4b2a35bf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:41:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:42:07 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:07 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:42:19 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:42:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:42:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:28 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:42:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:43:20 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 03:43:20 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 03:43:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 03:43:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:43:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:43:42 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:43:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:43:42 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:43:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:43:42 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:43:42 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf944e49ffa85996da499d5d92c328463b711fd3a1672b809e2824a964da9fb`  
		Last Modified: Fri, 02 Sep 2022 03:48:07 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020ff2b6bb0b679bc28ad3ec3d451993a1ef2282c86f87ca148774d73593a1cc`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 3.8 MB (3765427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977397ae9bc646b6dcf2321014794f535cb5a74110c608b1d1c0986ee1eb1424`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.0 MB (1992954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361cf449d40803e89980d56903e81945ce9fa372a686ea76f4a9c7a646a8337`  
		Last Modified: Fri, 02 Sep 2022 03:48:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d26195015760a28953bf9d2ad8603a66f8508da28d9878f972ddf137a5b34d`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.3 MB (2281503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a47dd94359e3cf2394add8b9de63828e53d9d2195aa09d903a5e2143e6a9c`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4132d19a681ab040d5709b46847ab664104c652bf06ef4a02a0b81d909b57979`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701416dc7e3dc54762a773a56a3140235bcd7c031e29891270df8d8156ac566`  
		Last Modified: Fri, 02 Sep 2022 03:48:43 GMT  
		Size: 85.5 MB (85532069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e314a661679bf4986516e7a5521b2ced57b07332a1bee31fdc83146474893a4`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efce0fc30145a5908ba6bf7fd4c4b33fd9d54e593bff96c19842055866bee692`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b27d6a2d4a982fb67a724692fd8edd42e1bfe20dd6d2a73b2fb0eb16c27ad7d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102629742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ecf4f48e2978426dbcc04c56a89f22f76339b1ac791bc5baf9052cb4b99890`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:25:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:26:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:01 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:26:17 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:26:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:26:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:26 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:26:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:27:16 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 05:27:17 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 05:27:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 05:27:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:27:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:27:41 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:27:43 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:27:44 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:27:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:27:45 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:27:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0749552ddbb27b679c4c784814a6bc9cff4dea894b4c50ff08211ac33d7141`  
		Last Modified: Fri, 02 Sep 2022 05:33:56 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f3be11a3a90d15ce271dbf8b58dc49944d979b4199b6a9810b17688f071274`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 3.6 MB (3593224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c93d9284a3d0f05825c9fdc3591a7d7d3ae34f1ae103b4ff077a235d40e0f`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 1.9 MB (1898967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232f4136dd4f7f7c1b1de60c1ce430dfdb5d873cdc0e8cf41ac08e1ece7077c2`  
		Last Modified: Fri, 02 Sep 2022 05:33:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ccd89de31befb378b3fd447ebd5efc4fc67e5969c98f28f3df064a191ec01`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 2.2 MB (2194638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea239af7d9b117acb387a6885623fe9b3dd8df83c1e1cd42c1e418f41e14ef3f`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b306f626891fb340fada4bee82bca7350cea48d4b7d9417c8e16d70b607625`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f977adfc1f0b0065e437818c0d56a7fbea2e66cc2c20fcffb22eb2c726a9d32a`  
		Last Modified: Fri, 02 Sep 2022 05:34:31 GMT  
		Size: 66.5 MB (66546741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c63d31682849e6f78d30d0f7433c748e8581611ada5daf827d30785d2918fd2`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d7766f9fa328aaecc5edea92a920254bf6c7d03d0155d4bbc0b2fced86eded`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:efc520a5969afe22458ec081d2591e6c530af4bdc71f4cb66a755645faff34a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117027115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6dac49f7b083a7406a56adae7166704f912cc7c1676485947393adb8952ad3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:52:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:53:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:53:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:53:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:53:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:55:03 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 04:55:03 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 04:55:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 04:55:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:55:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:55:46 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:55:47 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:55:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:55:47 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:55:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55324944c013f5e152ef0fad27126a86f0a45cfff228ed5d376984c8bcb18dbc`  
		Last Modified: Fri, 02 Sep 2022 05:04:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc5813595f57876629a096fc5630c832e5d23f1a6f8c52b86f94b395dd72973`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 4.5 MB (4503005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53136ad37739b4c4b6d5c9c41623f06a89e1c954299e6487b758572c2129b6`  
		Last Modified: Fri, 02 Sep 2022 05:04:41 GMT  
		Size: 1.9 MB (1922006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e9deaa9bc92d6868ca60db4ace55d593c6da8f7dd776648377d6df75bbcdb2`  
		Last Modified: Fri, 02 Sep 2022 05:04:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88549712edded06fae8bfa5c56fae89c47664fc83e5b4a957c2c2764649ebff`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 2.4 MB (2389323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a4751f2b2dee4c43d237fe7b4ce6e1273b2374fcce6496c681cb525e8d26c1`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105f46c3085029c3a9f300164ffa8751b280f2ac336393e07ca596d6f1475929`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997e1406175b8de4067c34e21e14c3e22d70e65d699abfb60d8dfd481f2ef6be`  
		Last Modified: Fri, 02 Sep 2022 05:05:37 GMT  
		Size: 72.5 MB (72476684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66144ed93c4b6752c2c1059ed5ab44b752cc2444db93c44745a7c41c644be878`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39015c23b5aa07433c0d517088d4fb65a3b8e8d59ae9d235e1edc1661971bfb1`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; s390x

```console
$ docker pull mariadb@sha256:6f4ec55b4c6a791b54f9a18f4f744b8cd3526fdfd9be7d238370ce93fecc9b8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105124376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66ac2973c068da3f5b39dcb1713654443f0ccd0cf7e315dab0de330e787d8c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:18:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:18:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:18:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:18:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:32 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:18:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:19:29 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 02:19:29 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 02:19:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 02:19:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:19:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:19:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:19:50 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:19:50 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:19:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:19:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a83a742f8905e65d86bab1137abea13cf130c3c52de601dd27fc4c4188ad7`  
		Last Modified: Fri, 02 Sep 2022 02:23:46 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0074f95048477359d16a331130ff329c74b549bcc5d7a97cd5559fcfe9c7464`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 3.7 MB (3674479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792e98156ec6717f9a09ef69964b1441fc52ea8407babf26638a445cfbca24a7`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.0 MB (1956114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f52d5f8a1d48c335871d777bb6305d30ca6e0d35472d729f97839e5118e1ed`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b51775573dc421f5d01c30c0385676817ad4cd3ed88f8c69fdfe498f57a5b39`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.2 MB (2200620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c5f2dd2c4f8a5fcba9a6bd048360e2483d370947a8e8499b83147d0878d31d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4005206c1b7f520588d957202113c82375fa4ac4b297a19265f0fc8408f6a082`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56247b961b3a212d383dc7a9d8148dfccfbcc139deb5f0c7718cac610d4707e2`  
		Last Modified: Fri, 02 Sep 2022 02:24:16 GMT  
		Size: 68.6 MB (68635084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a147a6bdb02d471ccfe5c14f82e463b195033f170feccb02e1db2bb128b051a5`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318ac1fb7ba29d893d6d9bb95215957152ae3ea476a5b7325b44532655c7c37d`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-jammy`

```console
$ docker pull mariadb@sha256:ca04948aca834499f728692520eff82917de1d768b47751ba4dd0fc5f261c8e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:7e613e248abdf4604776d6ace8eba9998b61b44f3c6cfd7121939c2fc3f1a7d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (124013572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c284e5e829612878511aa9fc0c383708c5a68f2167fa77a515bc2e4b2a35bf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:41:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:42:07 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:07 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:42:19 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:42:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:42:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:28 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:42:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:43:20 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 03:43:20 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 03:43:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 03:43:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:43:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:43:42 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:43:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:43:42 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:43:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:43:42 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:43:42 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf944e49ffa85996da499d5d92c328463b711fd3a1672b809e2824a964da9fb`  
		Last Modified: Fri, 02 Sep 2022 03:48:07 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020ff2b6bb0b679bc28ad3ec3d451993a1ef2282c86f87ca148774d73593a1cc`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 3.8 MB (3765427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977397ae9bc646b6dcf2321014794f535cb5a74110c608b1d1c0986ee1eb1424`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.0 MB (1992954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361cf449d40803e89980d56903e81945ce9fa372a686ea76f4a9c7a646a8337`  
		Last Modified: Fri, 02 Sep 2022 03:48:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d26195015760a28953bf9d2ad8603a66f8508da28d9878f972ddf137a5b34d`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.3 MB (2281503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a47dd94359e3cf2394add8b9de63828e53d9d2195aa09d903a5e2143e6a9c`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4132d19a681ab040d5709b46847ab664104c652bf06ef4a02a0b81d909b57979`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701416dc7e3dc54762a773a56a3140235bcd7c031e29891270df8d8156ac566`  
		Last Modified: Fri, 02 Sep 2022 03:48:43 GMT  
		Size: 85.5 MB (85532069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e314a661679bf4986516e7a5521b2ced57b07332a1bee31fdc83146474893a4`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efce0fc30145a5908ba6bf7fd4c4b33fd9d54e593bff96c19842055866bee692`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b27d6a2d4a982fb67a724692fd8edd42e1bfe20dd6d2a73b2fb0eb16c27ad7d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102629742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ecf4f48e2978426dbcc04c56a89f22f76339b1ac791bc5baf9052cb4b99890`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:25:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:26:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:01 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:26:17 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:26:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:26:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:26 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:26:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:27:16 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 05:27:17 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 05:27:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 05:27:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:27:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:27:41 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:27:43 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:27:44 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:27:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:27:45 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:27:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0749552ddbb27b679c4c784814a6bc9cff4dea894b4c50ff08211ac33d7141`  
		Last Modified: Fri, 02 Sep 2022 05:33:56 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f3be11a3a90d15ce271dbf8b58dc49944d979b4199b6a9810b17688f071274`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 3.6 MB (3593224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c93d9284a3d0f05825c9fdc3591a7d7d3ae34f1ae103b4ff077a235d40e0f`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 1.9 MB (1898967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232f4136dd4f7f7c1b1de60c1ce430dfdb5d873cdc0e8cf41ac08e1ece7077c2`  
		Last Modified: Fri, 02 Sep 2022 05:33:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ccd89de31befb378b3fd447ebd5efc4fc67e5969c98f28f3df064a191ec01`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 2.2 MB (2194638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea239af7d9b117acb387a6885623fe9b3dd8df83c1e1cd42c1e418f41e14ef3f`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b306f626891fb340fada4bee82bca7350cea48d4b7d9417c8e16d70b607625`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f977adfc1f0b0065e437818c0d56a7fbea2e66cc2c20fcffb22eb2c726a9d32a`  
		Last Modified: Fri, 02 Sep 2022 05:34:31 GMT  
		Size: 66.5 MB (66546741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c63d31682849e6f78d30d0f7433c748e8581611ada5daf827d30785d2918fd2`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d7766f9fa328aaecc5edea92a920254bf6c7d03d0155d4bbc0b2fced86eded`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:efc520a5969afe22458ec081d2591e6c530af4bdc71f4cb66a755645faff34a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117027115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6dac49f7b083a7406a56adae7166704f912cc7c1676485947393adb8952ad3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:52:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:53:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:53:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:53:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:53:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:55:03 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 04:55:03 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 04:55:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 04:55:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:55:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:55:46 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:55:47 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:55:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:55:47 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:55:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55324944c013f5e152ef0fad27126a86f0a45cfff228ed5d376984c8bcb18dbc`  
		Last Modified: Fri, 02 Sep 2022 05:04:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc5813595f57876629a096fc5630c832e5d23f1a6f8c52b86f94b395dd72973`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 4.5 MB (4503005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53136ad37739b4c4b6d5c9c41623f06a89e1c954299e6487b758572c2129b6`  
		Last Modified: Fri, 02 Sep 2022 05:04:41 GMT  
		Size: 1.9 MB (1922006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e9deaa9bc92d6868ca60db4ace55d593c6da8f7dd776648377d6df75bbcdb2`  
		Last Modified: Fri, 02 Sep 2022 05:04:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88549712edded06fae8bfa5c56fae89c47664fc83e5b4a957c2c2764649ebff`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 2.4 MB (2389323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a4751f2b2dee4c43d237fe7b4ce6e1273b2374fcce6496c681cb525e8d26c1`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105f46c3085029c3a9f300164ffa8751b280f2ac336393e07ca596d6f1475929`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997e1406175b8de4067c34e21e14c3e22d70e65d699abfb60d8dfd481f2ef6be`  
		Last Modified: Fri, 02 Sep 2022 05:05:37 GMT  
		Size: 72.5 MB (72476684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66144ed93c4b6752c2c1059ed5ab44b752cc2444db93c44745a7c41c644be878`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39015c23b5aa07433c0d517088d4fb65a3b8e8d59ae9d235e1edc1661971bfb1`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:6f4ec55b4c6a791b54f9a18f4f744b8cd3526fdfd9be7d238370ce93fecc9b8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105124376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66ac2973c068da3f5b39dcb1713654443f0ccd0cf7e315dab0de330e787d8c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:18:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:18:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:18:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:18:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:32 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:18:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:19:29 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 02:19:29 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 02:19:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 02:19:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:19:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:19:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:19:50 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:19:50 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:19:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:19:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a83a742f8905e65d86bab1137abea13cf130c3c52de601dd27fc4c4188ad7`  
		Last Modified: Fri, 02 Sep 2022 02:23:46 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0074f95048477359d16a331130ff329c74b549bcc5d7a97cd5559fcfe9c7464`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 3.7 MB (3674479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792e98156ec6717f9a09ef69964b1441fc52ea8407babf26638a445cfbca24a7`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.0 MB (1956114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f52d5f8a1d48c335871d777bb6305d30ca6e0d35472d729f97839e5118e1ed`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b51775573dc421f5d01c30c0385676817ad4cd3ed88f8c69fdfe498f57a5b39`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.2 MB (2200620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c5f2dd2c4f8a5fcba9a6bd048360e2483d370947a8e8499b83147d0878d31d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4005206c1b7f520588d957202113c82375fa4ac4b297a19265f0fc8408f6a082`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56247b961b3a212d383dc7a9d8148dfccfbcc139deb5f0c7718cac610d4707e2`  
		Last Modified: Fri, 02 Sep 2022 02:24:16 GMT  
		Size: 68.6 MB (68635084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a147a6bdb02d471ccfe5c14f82e463b195033f170feccb02e1db2bb128b051a5`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318ac1fb7ba29d893d6d9bb95215957152ae3ea476a5b7325b44532655c7c37d`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10-rc`

```console
$ docker pull mariadb@sha256:f72a0f8c8ad1ac903cb22aebd4168ad92be60e01c354c256ded3a3119c26c6a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.10-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:63a176cd8b86aaabd2db0384b046905ff8cbb9d666bfd258c927a8c4c0998b4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127866498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44fe8cc220208582fe1ebab8a861d40bfff15de448edd873a4230179b92d589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:41:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:42:07 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:07 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:42:19 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:42:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:42:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:28 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:42:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:42:29 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 03:42:29 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 03:42:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 03:42:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:43:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:43:09 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:43:10 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:43:10 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:43:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:43:10 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:43:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf944e49ffa85996da499d5d92c328463b711fd3a1672b809e2824a964da9fb`  
		Last Modified: Fri, 02 Sep 2022 03:48:07 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020ff2b6bb0b679bc28ad3ec3d451993a1ef2282c86f87ca148774d73593a1cc`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 3.8 MB (3765427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977397ae9bc646b6dcf2321014794f535cb5a74110c608b1d1c0986ee1eb1424`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.0 MB (1992954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361cf449d40803e89980d56903e81945ce9fa372a686ea76f4a9c7a646a8337`  
		Last Modified: Fri, 02 Sep 2022 03:48:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d26195015760a28953bf9d2ad8603a66f8508da28d9878f972ddf137a5b34d`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.3 MB (2281503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a47dd94359e3cf2394add8b9de63828e53d9d2195aa09d903a5e2143e6a9c`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4454d55acc28f5aad3988b76ee8e6da1d5de3e5aef12c04c4239a638865f2f40`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3389f250985a8732f316319f8050f3167a3b01d1900fd15ab12b1dec634a3aaf`  
		Last Modified: Fri, 02 Sep 2022 03:48:16 GMT  
		Size: 89.4 MB (89384994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0a7c94b05b97059fffee613c830da401a0677043d70d6761c38315b1a3a6f`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe23ebdaeee86b655dbf66e2182ed96b07b7ad17e39588810f25b0c9e466200`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0e3e613b5017436210b9e7e64451d773da684e512216d3d2c21015ed68a2c5d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104418493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e70cf3556ea55edfdf52779198b666e0f4fd90f728a1b1fbb0bef26d567a51fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:25:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:26:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:01 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:26:17 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:26:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:26:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:26 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:26:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:26:29 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 05:26:30 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 05:26:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 05:26:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:26:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:26:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:26:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:26:57 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:26:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:26:58 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:26:59 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0749552ddbb27b679c4c784814a6bc9cff4dea894b4c50ff08211ac33d7141`  
		Last Modified: Fri, 02 Sep 2022 05:33:56 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f3be11a3a90d15ce271dbf8b58dc49944d979b4199b6a9810b17688f071274`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 3.6 MB (3593224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c93d9284a3d0f05825c9fdc3591a7d7d3ae34f1ae103b4ff077a235d40e0f`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 1.9 MB (1898967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232f4136dd4f7f7c1b1de60c1ce430dfdb5d873cdc0e8cf41ac08e1ece7077c2`  
		Last Modified: Fri, 02 Sep 2022 05:33:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ccd89de31befb378b3fd447ebd5efc4fc67e5969c98f28f3df064a191ec01`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 2.2 MB (2194638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea239af7d9b117acb387a6885623fe9b3dd8df83c1e1cd42c1e418f41e14ef3f`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e8fc052147b1386b60399b89c6da423b0c2c9ef5ff51eaeec7c9e1ab2ab1ab`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1099e03734aa64cc9d72cf94b2cd79bc2b1b3e03f10f59620d337fe592bd71ad`  
		Last Modified: Fri, 02 Sep 2022 05:34:02 GMT  
		Size: 68.3 MB (68335490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9cc8c194b8295ec9a3f0186c6c6e8d3e17937321cb3de72ee52fe0987c2c04`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b5bd276d9535ea2beb13f69884e0294357647599bc8564038288fdade3ca7a`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:80bfb3d61afd180f1c85e43004b517daa2b4992b852924b74491e630243cb173
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118875231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bc7d70001decd3e6eb10f85a299f882832b39e5a37e197c4ac115bc05e4c49d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:52:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:53:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:53:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:53:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:53:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:53:46 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 04:53:46 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 04:53:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 04:53:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:54:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:54:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:54:46 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:54:46 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:54:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:54:47 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:54:47 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55324944c013f5e152ef0fad27126a86f0a45cfff228ed5d376984c8bcb18dbc`  
		Last Modified: Fri, 02 Sep 2022 05:04:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc5813595f57876629a096fc5630c832e5d23f1a6f8c52b86f94b395dd72973`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 4.5 MB (4503005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53136ad37739b4c4b6d5c9c41623f06a89e1c954299e6487b758572c2129b6`  
		Last Modified: Fri, 02 Sep 2022 05:04:41 GMT  
		Size: 1.9 MB (1922006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e9deaa9bc92d6868ca60db4ace55d593c6da8f7dd776648377d6df75bbcdb2`  
		Last Modified: Fri, 02 Sep 2022 05:04:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88549712edded06fae8bfa5c56fae89c47664fc83e5b4a957c2c2764649ebff`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 2.4 MB (2389323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a4751f2b2dee4c43d237fe7b4ce6e1273b2374fcce6496c681cb525e8d26c1`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da29ffbb8b6b8b4238f95c37d07b8082d6a732ac3e34c6fa2d976bbf52c403a`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c258c128927113436cbb111e01ad2be73cf5a0063faa7bb9ed992acbaa0dbe6e`  
		Last Modified: Fri, 02 Sep 2022 05:04:57 GMT  
		Size: 74.3 MB (74324794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d808802090330fb48fd19eca992270663ebbc0ea0dcf4a9bbbf158a6b49b0c`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d981de12d517df114c59bf23dedf64803a95ace763e096e8c46cb289d32234e`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:72ed28f1fdf56555c9f08785e409d89126035e7cf2193f571ce79263d1f0ff11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107303124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf87bed09602ce288f39d2b9016eb3f45bf99750c81558eae73a456fcb31081`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:18:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:18:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:18:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:18:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:32 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:18:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:18:34 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 02:18:34 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 02:18:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 02:18:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:19:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:19:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:19:11 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:19:11 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:19:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:19:12 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:19:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a83a742f8905e65d86bab1137abea13cf130c3c52de601dd27fc4c4188ad7`  
		Last Modified: Fri, 02 Sep 2022 02:23:46 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0074f95048477359d16a331130ff329c74b549bcc5d7a97cd5559fcfe9c7464`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 3.7 MB (3674479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792e98156ec6717f9a09ef69964b1441fc52ea8407babf26638a445cfbca24a7`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.0 MB (1956114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f52d5f8a1d48c335871d777bb6305d30ca6e0d35472d729f97839e5118e1ed`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b51775573dc421f5d01c30c0385676817ad4cd3ed88f8c69fdfe498f57a5b39`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.2 MB (2200620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c5f2dd2c4f8a5fcba9a6bd048360e2483d370947a8e8499b83147d0878d31d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9a9a0e4520a2aec75826e0af747ef46ef7f18324b92863d494cee07d764d84`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de990102574350bfef752f732153cf65ee620d5ef5cf360ae047cabe48ed98fc`  
		Last Modified: Fri, 02 Sep 2022 02:23:53 GMT  
		Size: 70.8 MB (70813831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2807fd8127e4f41277439d2c66a230cddace3cb032721f829f176a52902e2da5`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a773b0a90f861f259a602d5363184274d18cd5ec9af524ced82a6c52677b87d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10-rc-jammy`

```console
$ docker pull mariadb@sha256:f72a0f8c8ad1ac903cb22aebd4168ad92be60e01c354c256ded3a3119c26c6a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.10-rc-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:63a176cd8b86aaabd2db0384b046905ff8cbb9d666bfd258c927a8c4c0998b4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127866498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44fe8cc220208582fe1ebab8a861d40bfff15de448edd873a4230179b92d589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:41:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:42:07 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:07 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:42:19 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:42:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:42:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:28 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:42:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:42:29 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 03:42:29 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 03:42:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 03:42:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:43:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:43:09 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:43:10 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:43:10 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:43:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:43:10 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:43:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf944e49ffa85996da499d5d92c328463b711fd3a1672b809e2824a964da9fb`  
		Last Modified: Fri, 02 Sep 2022 03:48:07 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020ff2b6bb0b679bc28ad3ec3d451993a1ef2282c86f87ca148774d73593a1cc`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 3.8 MB (3765427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977397ae9bc646b6dcf2321014794f535cb5a74110c608b1d1c0986ee1eb1424`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.0 MB (1992954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361cf449d40803e89980d56903e81945ce9fa372a686ea76f4a9c7a646a8337`  
		Last Modified: Fri, 02 Sep 2022 03:48:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d26195015760a28953bf9d2ad8603a66f8508da28d9878f972ddf137a5b34d`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.3 MB (2281503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a47dd94359e3cf2394add8b9de63828e53d9d2195aa09d903a5e2143e6a9c`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4454d55acc28f5aad3988b76ee8e6da1d5de3e5aef12c04c4239a638865f2f40`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3389f250985a8732f316319f8050f3167a3b01d1900fd15ab12b1dec634a3aaf`  
		Last Modified: Fri, 02 Sep 2022 03:48:16 GMT  
		Size: 89.4 MB (89384994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0a7c94b05b97059fffee613c830da401a0677043d70d6761c38315b1a3a6f`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe23ebdaeee86b655dbf66e2182ed96b07b7ad17e39588810f25b0c9e466200`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-rc-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0e3e613b5017436210b9e7e64451d773da684e512216d3d2c21015ed68a2c5d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104418493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e70cf3556ea55edfdf52779198b666e0f4fd90f728a1b1fbb0bef26d567a51fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:25:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:26:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:01 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:26:17 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:26:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:26:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:26 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:26:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:26:29 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 05:26:30 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 05:26:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 05:26:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:26:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:26:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:26:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:26:57 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:26:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:26:58 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:26:59 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0749552ddbb27b679c4c784814a6bc9cff4dea894b4c50ff08211ac33d7141`  
		Last Modified: Fri, 02 Sep 2022 05:33:56 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f3be11a3a90d15ce271dbf8b58dc49944d979b4199b6a9810b17688f071274`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 3.6 MB (3593224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c93d9284a3d0f05825c9fdc3591a7d7d3ae34f1ae103b4ff077a235d40e0f`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 1.9 MB (1898967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232f4136dd4f7f7c1b1de60c1ce430dfdb5d873cdc0e8cf41ac08e1ece7077c2`  
		Last Modified: Fri, 02 Sep 2022 05:33:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ccd89de31befb378b3fd447ebd5efc4fc67e5969c98f28f3df064a191ec01`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 2.2 MB (2194638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea239af7d9b117acb387a6885623fe9b3dd8df83c1e1cd42c1e418f41e14ef3f`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e8fc052147b1386b60399b89c6da423b0c2c9ef5ff51eaeec7c9e1ab2ab1ab`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1099e03734aa64cc9d72cf94b2cd79bc2b1b3e03f10f59620d337fe592bd71ad`  
		Last Modified: Fri, 02 Sep 2022 05:34:02 GMT  
		Size: 68.3 MB (68335490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9cc8c194b8295ec9a3f0186c6c6e8d3e17937321cb3de72ee52fe0987c2c04`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b5bd276d9535ea2beb13f69884e0294357647599bc8564038288fdade3ca7a`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-rc-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:80bfb3d61afd180f1c85e43004b517daa2b4992b852924b74491e630243cb173
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118875231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bc7d70001decd3e6eb10f85a299f882832b39e5a37e197c4ac115bc05e4c49d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:52:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:53:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:53:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:53:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:53:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:53:46 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 04:53:46 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 04:53:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 04:53:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:54:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:54:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:54:46 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:54:46 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:54:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:54:47 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:54:47 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55324944c013f5e152ef0fad27126a86f0a45cfff228ed5d376984c8bcb18dbc`  
		Last Modified: Fri, 02 Sep 2022 05:04:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc5813595f57876629a096fc5630c832e5d23f1a6f8c52b86f94b395dd72973`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 4.5 MB (4503005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53136ad37739b4c4b6d5c9c41623f06a89e1c954299e6487b758572c2129b6`  
		Last Modified: Fri, 02 Sep 2022 05:04:41 GMT  
		Size: 1.9 MB (1922006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e9deaa9bc92d6868ca60db4ace55d593c6da8f7dd776648377d6df75bbcdb2`  
		Last Modified: Fri, 02 Sep 2022 05:04:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88549712edded06fae8bfa5c56fae89c47664fc83e5b4a957c2c2764649ebff`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 2.4 MB (2389323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a4751f2b2dee4c43d237fe7b4ce6e1273b2374fcce6496c681cb525e8d26c1`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da29ffbb8b6b8b4238f95c37d07b8082d6a732ac3e34c6fa2d976bbf52c403a`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c258c128927113436cbb111e01ad2be73cf5a0063faa7bb9ed992acbaa0dbe6e`  
		Last Modified: Fri, 02 Sep 2022 05:04:57 GMT  
		Size: 74.3 MB (74324794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d808802090330fb48fd19eca992270663ebbc0ea0dcf4a9bbbf158a6b49b0c`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d981de12d517df114c59bf23dedf64803a95ace763e096e8c46cb289d32234e`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10-rc-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:72ed28f1fdf56555c9f08785e409d89126035e7cf2193f571ce79263d1f0ff11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107303124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf87bed09602ce288f39d2b9016eb3f45bf99750c81558eae73a456fcb31081`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:18:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:18:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:18:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:18:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:32 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:18:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:18:34 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 02:18:34 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 02:18:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 02:18:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:19:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:19:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:19:11 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:19:11 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:19:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:19:12 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:19:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a83a742f8905e65d86bab1137abea13cf130c3c52de601dd27fc4c4188ad7`  
		Last Modified: Fri, 02 Sep 2022 02:23:46 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0074f95048477359d16a331130ff329c74b549bcc5d7a97cd5559fcfe9c7464`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 3.7 MB (3674479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792e98156ec6717f9a09ef69964b1441fc52ea8407babf26638a445cfbca24a7`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.0 MB (1956114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f52d5f8a1d48c335871d777bb6305d30ca6e0d35472d729f97839e5118e1ed`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b51775573dc421f5d01c30c0385676817ad4cd3ed88f8c69fdfe498f57a5b39`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.2 MB (2200620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c5f2dd2c4f8a5fcba9a6bd048360e2483d370947a8e8499b83147d0878d31d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9a9a0e4520a2aec75826e0af747ef46ef7f18324b92863d494cee07d764d84`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de990102574350bfef752f732153cf65ee620d5ef5cf360ae047cabe48ed98fc`  
		Last Modified: Fri, 02 Sep 2022 02:23:53 GMT  
		Size: 70.8 MB (70813831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2807fd8127e4f41277439d2c66a230cddace3cb032721f829f176a52902e2da5`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a773b0a90f861f259a602d5363184274d18cd5ec9af524ced82a6c52677b87d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10.1-rc`

```console
$ docker pull mariadb@sha256:f72a0f8c8ad1ac903cb22aebd4168ad92be60e01c354c256ded3a3119c26c6a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.10.1-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:63a176cd8b86aaabd2db0384b046905ff8cbb9d666bfd258c927a8c4c0998b4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127866498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44fe8cc220208582fe1ebab8a861d40bfff15de448edd873a4230179b92d589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:41:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:42:07 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:07 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:42:19 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:42:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:42:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:28 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:42:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:42:29 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 03:42:29 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 03:42:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 03:42:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:43:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:43:09 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:43:10 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:43:10 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:43:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:43:10 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:43:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf944e49ffa85996da499d5d92c328463b711fd3a1672b809e2824a964da9fb`  
		Last Modified: Fri, 02 Sep 2022 03:48:07 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020ff2b6bb0b679bc28ad3ec3d451993a1ef2282c86f87ca148774d73593a1cc`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 3.8 MB (3765427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977397ae9bc646b6dcf2321014794f535cb5a74110c608b1d1c0986ee1eb1424`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.0 MB (1992954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361cf449d40803e89980d56903e81945ce9fa372a686ea76f4a9c7a646a8337`  
		Last Modified: Fri, 02 Sep 2022 03:48:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d26195015760a28953bf9d2ad8603a66f8508da28d9878f972ddf137a5b34d`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.3 MB (2281503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a47dd94359e3cf2394add8b9de63828e53d9d2195aa09d903a5e2143e6a9c`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4454d55acc28f5aad3988b76ee8e6da1d5de3e5aef12c04c4239a638865f2f40`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3389f250985a8732f316319f8050f3167a3b01d1900fd15ab12b1dec634a3aaf`  
		Last Modified: Fri, 02 Sep 2022 03:48:16 GMT  
		Size: 89.4 MB (89384994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0a7c94b05b97059fffee613c830da401a0677043d70d6761c38315b1a3a6f`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe23ebdaeee86b655dbf66e2182ed96b07b7ad17e39588810f25b0c9e466200`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.1-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0e3e613b5017436210b9e7e64451d773da684e512216d3d2c21015ed68a2c5d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104418493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e70cf3556ea55edfdf52779198b666e0f4fd90f728a1b1fbb0bef26d567a51fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:25:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:26:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:01 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:26:17 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:26:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:26:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:26 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:26:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:26:29 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 05:26:30 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 05:26:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 05:26:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:26:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:26:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:26:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:26:57 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:26:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:26:58 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:26:59 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0749552ddbb27b679c4c784814a6bc9cff4dea894b4c50ff08211ac33d7141`  
		Last Modified: Fri, 02 Sep 2022 05:33:56 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f3be11a3a90d15ce271dbf8b58dc49944d979b4199b6a9810b17688f071274`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 3.6 MB (3593224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c93d9284a3d0f05825c9fdc3591a7d7d3ae34f1ae103b4ff077a235d40e0f`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 1.9 MB (1898967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232f4136dd4f7f7c1b1de60c1ce430dfdb5d873cdc0e8cf41ac08e1ece7077c2`  
		Last Modified: Fri, 02 Sep 2022 05:33:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ccd89de31befb378b3fd447ebd5efc4fc67e5969c98f28f3df064a191ec01`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 2.2 MB (2194638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea239af7d9b117acb387a6885623fe9b3dd8df83c1e1cd42c1e418f41e14ef3f`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e8fc052147b1386b60399b89c6da423b0c2c9ef5ff51eaeec7c9e1ab2ab1ab`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1099e03734aa64cc9d72cf94b2cd79bc2b1b3e03f10f59620d337fe592bd71ad`  
		Last Modified: Fri, 02 Sep 2022 05:34:02 GMT  
		Size: 68.3 MB (68335490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9cc8c194b8295ec9a3f0186c6c6e8d3e17937321cb3de72ee52fe0987c2c04`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b5bd276d9535ea2beb13f69884e0294357647599bc8564038288fdade3ca7a`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.1-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:80bfb3d61afd180f1c85e43004b517daa2b4992b852924b74491e630243cb173
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118875231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bc7d70001decd3e6eb10f85a299f882832b39e5a37e197c4ac115bc05e4c49d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:52:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:53:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:53:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:53:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:53:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:53:46 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 04:53:46 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 04:53:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 04:53:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:54:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:54:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:54:46 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:54:46 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:54:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:54:47 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:54:47 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55324944c013f5e152ef0fad27126a86f0a45cfff228ed5d376984c8bcb18dbc`  
		Last Modified: Fri, 02 Sep 2022 05:04:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc5813595f57876629a096fc5630c832e5d23f1a6f8c52b86f94b395dd72973`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 4.5 MB (4503005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53136ad37739b4c4b6d5c9c41623f06a89e1c954299e6487b758572c2129b6`  
		Last Modified: Fri, 02 Sep 2022 05:04:41 GMT  
		Size: 1.9 MB (1922006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e9deaa9bc92d6868ca60db4ace55d593c6da8f7dd776648377d6df75bbcdb2`  
		Last Modified: Fri, 02 Sep 2022 05:04:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88549712edded06fae8bfa5c56fae89c47664fc83e5b4a957c2c2764649ebff`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 2.4 MB (2389323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a4751f2b2dee4c43d237fe7b4ce6e1273b2374fcce6496c681cb525e8d26c1`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da29ffbb8b6b8b4238f95c37d07b8082d6a732ac3e34c6fa2d976bbf52c403a`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c258c128927113436cbb111e01ad2be73cf5a0063faa7bb9ed992acbaa0dbe6e`  
		Last Modified: Fri, 02 Sep 2022 05:04:57 GMT  
		Size: 74.3 MB (74324794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d808802090330fb48fd19eca992270663ebbc0ea0dcf4a9bbbf158a6b49b0c`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d981de12d517df114c59bf23dedf64803a95ace763e096e8c46cb289d32234e`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.1-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:72ed28f1fdf56555c9f08785e409d89126035e7cf2193f571ce79263d1f0ff11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107303124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf87bed09602ce288f39d2b9016eb3f45bf99750c81558eae73a456fcb31081`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:18:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:18:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:18:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:18:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:32 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:18:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:18:34 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 02:18:34 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 02:18:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 02:18:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:19:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:19:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:19:11 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:19:11 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:19:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:19:12 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:19:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a83a742f8905e65d86bab1137abea13cf130c3c52de601dd27fc4c4188ad7`  
		Last Modified: Fri, 02 Sep 2022 02:23:46 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0074f95048477359d16a331130ff329c74b549bcc5d7a97cd5559fcfe9c7464`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 3.7 MB (3674479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792e98156ec6717f9a09ef69964b1441fc52ea8407babf26638a445cfbca24a7`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.0 MB (1956114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f52d5f8a1d48c335871d777bb6305d30ca6e0d35472d729f97839e5118e1ed`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b51775573dc421f5d01c30c0385676817ad4cd3ed88f8c69fdfe498f57a5b39`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.2 MB (2200620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c5f2dd2c4f8a5fcba9a6bd048360e2483d370947a8e8499b83147d0878d31d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9a9a0e4520a2aec75826e0af747ef46ef7f18324b92863d494cee07d764d84`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de990102574350bfef752f732153cf65ee620d5ef5cf360ae047cabe48ed98fc`  
		Last Modified: Fri, 02 Sep 2022 02:23:53 GMT  
		Size: 70.8 MB (70813831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2807fd8127e4f41277439d2c66a230cddace3cb032721f829f176a52902e2da5`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a773b0a90f861f259a602d5363184274d18cd5ec9af524ced82a6c52677b87d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.10.1-rc-jammy`

```console
$ docker pull mariadb@sha256:f72a0f8c8ad1ac903cb22aebd4168ad92be60e01c354c256ded3a3119c26c6a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.10.1-rc-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:63a176cd8b86aaabd2db0384b046905ff8cbb9d666bfd258c927a8c4c0998b4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127866498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b44fe8cc220208582fe1ebab8a861d40bfff15de448edd873a4230179b92d589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:41:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:42:07 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:07 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:42:19 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:42:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:42:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:28 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:42:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:42:29 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 03:42:29 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 03:42:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 03:42:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:43:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:43:09 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:43:10 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:43:10 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:43:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:43:10 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:43:10 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf944e49ffa85996da499d5d92c328463b711fd3a1672b809e2824a964da9fb`  
		Last Modified: Fri, 02 Sep 2022 03:48:07 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020ff2b6bb0b679bc28ad3ec3d451993a1ef2282c86f87ca148774d73593a1cc`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 3.8 MB (3765427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977397ae9bc646b6dcf2321014794f535cb5a74110c608b1d1c0986ee1eb1424`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.0 MB (1992954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361cf449d40803e89980d56903e81945ce9fa372a686ea76f4a9c7a646a8337`  
		Last Modified: Fri, 02 Sep 2022 03:48:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d26195015760a28953bf9d2ad8603a66f8508da28d9878f972ddf137a5b34d`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.3 MB (2281503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a47dd94359e3cf2394add8b9de63828e53d9d2195aa09d903a5e2143e6a9c`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4454d55acc28f5aad3988b76ee8e6da1d5de3e5aef12c04c4239a638865f2f40`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3389f250985a8732f316319f8050f3167a3b01d1900fd15ab12b1dec634a3aaf`  
		Last Modified: Fri, 02 Sep 2022 03:48:16 GMT  
		Size: 89.4 MB (89384994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe0a7c94b05b97059fffee613c830da401a0677043d70d6761c38315b1a3a6f`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe23ebdaeee86b655dbf66e2182ed96b07b7ad17e39588810f25b0c9e466200`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.1-rc-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0e3e613b5017436210b9e7e64451d773da684e512216d3d2c21015ed68a2c5d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104418493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e70cf3556ea55edfdf52779198b666e0f4fd90f728a1b1fbb0bef26d567a51fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:25:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:26:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:01 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:26:17 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:26:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:26:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:26 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:26:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:26:29 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 05:26:30 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 05:26:31 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 05:26:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:26:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:26:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:26:56 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:26:57 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:26:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:26:58 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:26:59 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0749552ddbb27b679c4c784814a6bc9cff4dea894b4c50ff08211ac33d7141`  
		Last Modified: Fri, 02 Sep 2022 05:33:56 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f3be11a3a90d15ce271dbf8b58dc49944d979b4199b6a9810b17688f071274`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 3.6 MB (3593224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c93d9284a3d0f05825c9fdc3591a7d7d3ae34f1ae103b4ff077a235d40e0f`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 1.9 MB (1898967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232f4136dd4f7f7c1b1de60c1ce430dfdb5d873cdc0e8cf41ac08e1ece7077c2`  
		Last Modified: Fri, 02 Sep 2022 05:33:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ccd89de31befb378b3fd447ebd5efc4fc67e5969c98f28f3df064a191ec01`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 2.2 MB (2194638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea239af7d9b117acb387a6885623fe9b3dd8df83c1e1cd42c1e418f41e14ef3f`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e8fc052147b1386b60399b89c6da423b0c2c9ef5ff51eaeec7c9e1ab2ab1ab`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1099e03734aa64cc9d72cf94b2cd79bc2b1b3e03f10f59620d337fe592bd71ad`  
		Last Modified: Fri, 02 Sep 2022 05:34:02 GMT  
		Size: 68.3 MB (68335490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9cc8c194b8295ec9a3f0186c6c6e8d3e17937321cb3de72ee52fe0987c2c04`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b5bd276d9535ea2beb13f69884e0294357647599bc8564038288fdade3ca7a`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.1-rc-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:80bfb3d61afd180f1c85e43004b517daa2b4992b852924b74491e630243cb173
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118875231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bc7d70001decd3e6eb10f85a299f882832b39e5a37e197c4ac115bc05e4c49d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:52:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:53:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:53:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:53:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:53:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:53:46 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 04:53:46 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 04:53:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 04:53:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:54:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:54:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:54:46 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:54:46 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:54:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:54:47 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:54:47 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55324944c013f5e152ef0fad27126a86f0a45cfff228ed5d376984c8bcb18dbc`  
		Last Modified: Fri, 02 Sep 2022 05:04:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc5813595f57876629a096fc5630c832e5d23f1a6f8c52b86f94b395dd72973`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 4.5 MB (4503005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53136ad37739b4c4b6d5c9c41623f06a89e1c954299e6487b758572c2129b6`  
		Last Modified: Fri, 02 Sep 2022 05:04:41 GMT  
		Size: 1.9 MB (1922006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e9deaa9bc92d6868ca60db4ace55d593c6da8f7dd776648377d6df75bbcdb2`  
		Last Modified: Fri, 02 Sep 2022 05:04:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88549712edded06fae8bfa5c56fae89c47664fc83e5b4a957c2c2764649ebff`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 2.4 MB (2389323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a4751f2b2dee4c43d237fe7b4ce6e1273b2374fcce6496c681cb525e8d26c1`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da29ffbb8b6b8b4238f95c37d07b8082d6a732ac3e34c6fa2d976bbf52c403a`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c258c128927113436cbb111e01ad2be73cf5a0063faa7bb9ed992acbaa0dbe6e`  
		Last Modified: Fri, 02 Sep 2022 05:04:57 GMT  
		Size: 74.3 MB (74324794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d808802090330fb48fd19eca992270663ebbc0ea0dcf4a9bbbf158a6b49b0c`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d981de12d517df114c59bf23dedf64803a95ace763e096e8c46cb289d32234e`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.10.1-rc-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:72ed28f1fdf56555c9f08785e409d89126035e7cf2193f571ce79263d1f0ff11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107303124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf87bed09602ce288f39d2b9016eb3f45bf99750c81558eae73a456fcb31081`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:18:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:18:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:18:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:18:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:32 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:18:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:18:34 GMT
ARG MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 02:18:34 GMT
ENV MARIADB_VERSION=1:10.10.1+maria~ubu2204
# Fri, 02 Sep 2022 02:18:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 02:18:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:19:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.10.1/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:19:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:19:11 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:19:11 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:19:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:19:12 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:19:12 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a83a742f8905e65d86bab1137abea13cf130c3c52de601dd27fc4c4188ad7`  
		Last Modified: Fri, 02 Sep 2022 02:23:46 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0074f95048477359d16a331130ff329c74b549bcc5d7a97cd5559fcfe9c7464`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 3.7 MB (3674479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792e98156ec6717f9a09ef69964b1441fc52ea8407babf26638a445cfbca24a7`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.0 MB (1956114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f52d5f8a1d48c335871d777bb6305d30ca6e0d35472d729f97839e5118e1ed`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b51775573dc421f5d01c30c0385676817ad4cd3ed88f8c69fdfe498f57a5b39`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.2 MB (2200620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c5f2dd2c4f8a5fcba9a6bd048360e2483d370947a8e8499b83147d0878d31d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9a9a0e4520a2aec75826e0af747ef46ef7f18324b92863d494cee07d764d84`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de990102574350bfef752f732153cf65ee620d5ef5cf360ae047cabe48ed98fc`  
		Last Modified: Fri, 02 Sep 2022 02:23:53 GMT  
		Size: 70.8 MB (70813831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2807fd8127e4f41277439d2c66a230cddace3cb032721f829f176a52902e2da5`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a773b0a90f861f259a602d5363184274d18cd5ec9af524ced82a6c52677b87d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:c769235db77fff4b6dc1eccb32cfc51b40b686a450bf12e6eecfe5df01c916e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:db3e7050a150772c34a27c65d8acfd466be8a2c8e26f26c28171f99007d53e49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120221063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2978a6a1eaf7fe4a0fbaca9a7c7599c25866852f7712958afe0edb2af83fef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:46:54 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 03:46:54 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 03:46:54 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 03:46:54 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 03:46:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:46:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:47:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:47:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:47:23 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:47:23 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:47:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 03:47:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:47:24 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:47:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc9da0995737ce94984fdbb5230dab10aac34f44581c04fc5fdb29d85711df5`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fd6ada2b2c203f950ba3a0ec980d7e6df86bb73bf7bb2dac275d18cc56be78`  
		Last Modified: Fri, 02 Sep 2022 03:51:49 GMT  
		Size: 80.3 MB (80306752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaa8398274c59fb7ec4d0624428cd9e56b7c986b3d4a624dd262344f9dbd8ae`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd4bd4ac7cf287cbc3afd119ee87da8b2ccc2dd7612a53aa89aacec4d1cb57`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938a2e87683b82a6b4af90e1d96d30d974372b94b88ded49998d45f07392305d`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:fb5502f285c9f8797f34c8f83fc3dac1bbea641b3a4526dd3d25e6bef88aa15f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117719627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a5c3993e86e23861683c05907f305fb413577451f92b8c0f4a1fadb63fc266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:32:01 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:32:01 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:32:02 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:32:03 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:32:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:32:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:32:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:32:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:32:34 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:32:35 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:32:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:32:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:32:37 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:32:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85e8fffea2104a54258086d7d062df6c19a23d6acd7f27bb721dd6d3a78d0ff`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a214017dcc58f16a030935e2eccc2388a96cf26505df14a08539afb7033a37e`  
		Last Modified: Fri, 02 Sep 2022 05:37:51 GMT  
		Size: 79.6 MB (79637211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684491e96984ea6bd53e18f3416adf5064baf60998bcf2f54396ff77747d0bcc`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37364f0f04f22d7f0997b915eecf9630a9ea4ae286ff35deb66db9866ef86025`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe600e61a068e3cbda5aa6a828118808a9964f7d575d2ee5caec1d5c63c4217`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:989c9a03246abd5c62326cd2c9f08ccf202ecc64d1ac4b062589d2b9567a4661
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131106416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f310cded24290e61deb238766c4bc795e514ca9213a11164359c5f174005d6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:02:07 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:02:07 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:02:07 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:02:08 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:02:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:02:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:03:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:03:02 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:03:02 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:03:04 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:03:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0e365a17cba280f5ea94402d76b1204fa3b9739a019b5a29ae3350d2e7eae0`  
		Last Modified: Fri, 02 Sep 2022 05:10:01 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931d60e7c59cd1abd61964c967a05cc09cd3434ced8572806c041be1357721a7`  
		Last Modified: Fri, 02 Sep 2022 05:10:23 GMT  
		Size: 84.9 MB (84907762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80364b61c0d25a8e15f72fb0033481ee0cab504961675bc0b6037ef6289b8dbc`  
		Last Modified: Fri, 02 Sep 2022 05:10:00 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3082715d12ba9b85147ccbf83e5fadd56ec54ea32f0a1722bea0a077344ae72e`  
		Last Modified: Fri, 02 Sep 2022 05:10:00 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fbcf13742cae6290880f88bd94fd18e1d4726da8085546ffdb88f21fc46c99`  
		Last Modified: Fri, 02 Sep 2022 05:10:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:c769235db77fff4b6dc1eccb32cfc51b40b686a450bf12e6eecfe5df01c916e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:db3e7050a150772c34a27c65d8acfd466be8a2c8e26f26c28171f99007d53e49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120221063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2978a6a1eaf7fe4a0fbaca9a7c7599c25866852f7712958afe0edb2af83fef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:46:54 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 03:46:54 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 03:46:54 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 03:46:54 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 03:46:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:46:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:47:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:47:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:47:23 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:47:23 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:47:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 03:47:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:47:24 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:47:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc9da0995737ce94984fdbb5230dab10aac34f44581c04fc5fdb29d85711df5`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fd6ada2b2c203f950ba3a0ec980d7e6df86bb73bf7bb2dac275d18cc56be78`  
		Last Modified: Fri, 02 Sep 2022 03:51:49 GMT  
		Size: 80.3 MB (80306752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaa8398274c59fb7ec4d0624428cd9e56b7c986b3d4a624dd262344f9dbd8ae`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd4bd4ac7cf287cbc3afd119ee87da8b2ccc2dd7612a53aa89aacec4d1cb57`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938a2e87683b82a6b4af90e1d96d30d974372b94b88ded49998d45f07392305d`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:fb5502f285c9f8797f34c8f83fc3dac1bbea641b3a4526dd3d25e6bef88aa15f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117719627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a5c3993e86e23861683c05907f305fb413577451f92b8c0f4a1fadb63fc266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:32:01 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:32:01 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:32:02 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:32:03 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:32:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:32:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:32:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:32:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:32:34 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:32:35 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:32:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:32:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:32:37 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:32:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85e8fffea2104a54258086d7d062df6c19a23d6acd7f27bb721dd6d3a78d0ff`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a214017dcc58f16a030935e2eccc2388a96cf26505df14a08539afb7033a37e`  
		Last Modified: Fri, 02 Sep 2022 05:37:51 GMT  
		Size: 79.6 MB (79637211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684491e96984ea6bd53e18f3416adf5064baf60998bcf2f54396ff77747d0bcc`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37364f0f04f22d7f0997b915eecf9630a9ea4ae286ff35deb66db9866ef86025`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe600e61a068e3cbda5aa6a828118808a9964f7d575d2ee5caec1d5c63c4217`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:989c9a03246abd5c62326cd2c9f08ccf202ecc64d1ac4b062589d2b9567a4661
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131106416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f310cded24290e61deb238766c4bc795e514ca9213a11164359c5f174005d6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:02:07 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:02:07 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:02:07 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:02:08 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:02:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:02:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:03:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:03:02 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:03:02 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:03:04 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:03:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0e365a17cba280f5ea94402d76b1204fa3b9739a019b5a29ae3350d2e7eae0`  
		Last Modified: Fri, 02 Sep 2022 05:10:01 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931d60e7c59cd1abd61964c967a05cc09cd3434ced8572806c041be1357721a7`  
		Last Modified: Fri, 02 Sep 2022 05:10:23 GMT  
		Size: 84.9 MB (84907762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80364b61c0d25a8e15f72fb0033481ee0cab504961675bc0b6037ef6289b8dbc`  
		Last Modified: Fri, 02 Sep 2022 05:10:00 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3082715d12ba9b85147ccbf83e5fadd56ec54ea32f0a1722bea0a077344ae72e`  
		Last Modified: Fri, 02 Sep 2022 05:10:00 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fbcf13742cae6290880f88bd94fd18e1d4726da8085546ffdb88f21fc46c99`  
		Last Modified: Fri, 02 Sep 2022 05:10:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.36`

```console
$ docker pull mariadb@sha256:c769235db77fff4b6dc1eccb32cfc51b40b686a450bf12e6eecfe5df01c916e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.36` - linux; amd64

```console
$ docker pull mariadb@sha256:db3e7050a150772c34a27c65d8acfd466be8a2c8e26f26c28171f99007d53e49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120221063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2978a6a1eaf7fe4a0fbaca9a7c7599c25866852f7712958afe0edb2af83fef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:46:54 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 03:46:54 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 03:46:54 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 03:46:54 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 03:46:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:46:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:47:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:47:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:47:23 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:47:23 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:47:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 03:47:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:47:24 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:47:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc9da0995737ce94984fdbb5230dab10aac34f44581c04fc5fdb29d85711df5`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fd6ada2b2c203f950ba3a0ec980d7e6df86bb73bf7bb2dac275d18cc56be78`  
		Last Modified: Fri, 02 Sep 2022 03:51:49 GMT  
		Size: 80.3 MB (80306752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaa8398274c59fb7ec4d0624428cd9e56b7c986b3d4a624dd262344f9dbd8ae`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd4bd4ac7cf287cbc3afd119ee87da8b2ccc2dd7612a53aa89aacec4d1cb57`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938a2e87683b82a6b4af90e1d96d30d974372b94b88ded49998d45f07392305d`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.36` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:fb5502f285c9f8797f34c8f83fc3dac1bbea641b3a4526dd3d25e6bef88aa15f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117719627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a5c3993e86e23861683c05907f305fb413577451f92b8c0f4a1fadb63fc266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:32:01 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:32:01 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:32:02 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:32:03 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:32:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:32:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:32:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:32:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:32:34 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:32:35 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:32:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:32:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:32:37 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:32:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85e8fffea2104a54258086d7d062df6c19a23d6acd7f27bb721dd6d3a78d0ff`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a214017dcc58f16a030935e2eccc2388a96cf26505df14a08539afb7033a37e`  
		Last Modified: Fri, 02 Sep 2022 05:37:51 GMT  
		Size: 79.6 MB (79637211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684491e96984ea6bd53e18f3416adf5064baf60998bcf2f54396ff77747d0bcc`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37364f0f04f22d7f0997b915eecf9630a9ea4ae286ff35deb66db9866ef86025`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe600e61a068e3cbda5aa6a828118808a9964f7d575d2ee5caec1d5c63c4217`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.36` - linux; ppc64le

```console
$ docker pull mariadb@sha256:989c9a03246abd5c62326cd2c9f08ccf202ecc64d1ac4b062589d2b9567a4661
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131106416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f310cded24290e61deb238766c4bc795e514ca9213a11164359c5f174005d6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:02:07 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:02:07 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:02:07 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:02:08 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:02:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:02:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:03:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:03:02 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:03:02 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:03:04 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:03:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0e365a17cba280f5ea94402d76b1204fa3b9739a019b5a29ae3350d2e7eae0`  
		Last Modified: Fri, 02 Sep 2022 05:10:01 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931d60e7c59cd1abd61964c967a05cc09cd3434ced8572806c041be1357721a7`  
		Last Modified: Fri, 02 Sep 2022 05:10:23 GMT  
		Size: 84.9 MB (84907762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80364b61c0d25a8e15f72fb0033481ee0cab504961675bc0b6037ef6289b8dbc`  
		Last Modified: Fri, 02 Sep 2022 05:10:00 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3082715d12ba9b85147ccbf83e5fadd56ec54ea32f0a1722bea0a077344ae72e`  
		Last Modified: Fri, 02 Sep 2022 05:10:00 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fbcf13742cae6290880f88bd94fd18e1d4726da8085546ffdb88f21fc46c99`  
		Last Modified: Fri, 02 Sep 2022 05:10:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.36-focal`

```console
$ docker pull mariadb@sha256:c769235db77fff4b6dc1eccb32cfc51b40b686a450bf12e6eecfe5df01c916e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.36-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:db3e7050a150772c34a27c65d8acfd466be8a2c8e26f26c28171f99007d53e49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120221063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2978a6a1eaf7fe4a0fbaca9a7c7599c25866852f7712958afe0edb2af83fef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:46:54 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 03:46:54 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 03:46:54 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 03:46:54 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 03:46:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:46:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:47:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:47:23 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:47:23 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:47:23 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:47:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 03:47:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:47:24 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:47:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc9da0995737ce94984fdbb5230dab10aac34f44581c04fc5fdb29d85711df5`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fd6ada2b2c203f950ba3a0ec980d7e6df86bb73bf7bb2dac275d18cc56be78`  
		Last Modified: Fri, 02 Sep 2022 03:51:49 GMT  
		Size: 80.3 MB (80306752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaa8398274c59fb7ec4d0624428cd9e56b7c986b3d4a624dd262344f9dbd8ae`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd4bd4ac7cf287cbc3afd119ee87da8b2ccc2dd7612a53aa89aacec4d1cb57`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938a2e87683b82a6b4af90e1d96d30d974372b94b88ded49998d45f07392305d`  
		Last Modified: Fri, 02 Sep 2022 03:51:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.36-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:fb5502f285c9f8797f34c8f83fc3dac1bbea641b3a4526dd3d25e6bef88aa15f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117719627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a5c3993e86e23861683c05907f305fb413577451f92b8c0f4a1fadb63fc266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:32:01 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:32:01 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:32:02 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:32:03 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:32:04 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:32:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:32:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:32:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:32:34 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:32:35 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:32:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:32:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:32:37 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:32:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85e8fffea2104a54258086d7d062df6c19a23d6acd7f27bb721dd6d3a78d0ff`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a214017dcc58f16a030935e2eccc2388a96cf26505df14a08539afb7033a37e`  
		Last Modified: Fri, 02 Sep 2022 05:37:51 GMT  
		Size: 79.6 MB (79637211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684491e96984ea6bd53e18f3416adf5064baf60998bcf2f54396ff77747d0bcc`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37364f0f04f22d7f0997b915eecf9630a9ea4ae286ff35deb66db9866ef86025`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe600e61a068e3cbda5aa6a828118808a9964f7d575d2ee5caec1d5c63c4217`  
		Last Modified: Fri, 02 Sep 2022 05:37:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.36-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:989c9a03246abd5c62326cd2c9f08ccf202ecc64d1ac4b062589d2b9567a4661
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131106416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f310cded24290e61deb238766c4bc795e514ca9213a11164359c5f174005d6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:02:07 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:02:07 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 02 Sep 2022 05:02:07 GMT
ARG MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:02:08 GMT
ENV MARIADB_VERSION=1:10.3.36+maria~ubu2004
# Fri, 02 Sep 2022 05:02:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:02:10 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:02:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:03:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:03:02 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:03:02 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:03:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.36/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:03:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:03:04 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:03:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0e365a17cba280f5ea94402d76b1204fa3b9739a019b5a29ae3350d2e7eae0`  
		Last Modified: Fri, 02 Sep 2022 05:10:01 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931d60e7c59cd1abd61964c967a05cc09cd3434ced8572806c041be1357721a7`  
		Last Modified: Fri, 02 Sep 2022 05:10:23 GMT  
		Size: 84.9 MB (84907762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80364b61c0d25a8e15f72fb0033481ee0cab504961675bc0b6037ef6289b8dbc`  
		Last Modified: Fri, 02 Sep 2022 05:10:00 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3082715d12ba9b85147ccbf83e5fadd56ec54ea32f0a1722bea0a077344ae72e`  
		Last Modified: Fri, 02 Sep 2022 05:10:00 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fbcf13742cae6290880f88bd94fd18e1d4726da8085546ffdb88f21fc46c99`  
		Last Modified: Fri, 02 Sep 2022 05:10:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:1e90e1aae83341869c9938f9df91e140d07df6e87acf9fc958f29f9d71d582e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:5d2aa8c7effe3db2cd2338cc892852c247f26b5ee016372011bb4a906bfac2fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125832212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801fdf0164b268eccd799a793913b7664b7f64ed43a852d97f9daa3bfcca897b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:46:25 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 03:46:25 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 03:46:25 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 03:46:25 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 03:46:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:46:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:46:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:46:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:46:50 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:46:50 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:46:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 03:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:46:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:46:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d194f12d3188cb6b7a11bde77791bbd35326da766a493465b142f98abc3caa`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fb7e8252943bfc6428758bdb8db56078cb61413b90658bef225022398a6c91`  
		Last Modified: Fri, 02 Sep 2022 03:51:21 GMT  
		Size: 85.9 MB (85917901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff39f4020c49372580edeb910dc65d7018e3fd41f3ac7747b76a2c3f146ef85`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5bd8a470bef766b74cdda1f8b8957427767298b4ec30701532008832602b53`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c24d2dc91cbb8ab7b21104ca6bc0678ce2a75602ee92e5112502f60b82e03e`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:024fed356afa64de41a956f6e776f6bd4153cd5942fb998666eeae5c5c5d9ecf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123210931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b620220f60ff7959c4ef01f7e8f924e366c6030a99f6199d7e5e499ab404b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:31:17 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:31:18 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:31:19 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:31:20 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:31:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:31:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:31:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:31:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:31:48 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:31:49 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:31:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:31:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:31:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:31:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6380fc1f620ea4d1844db54f67020beef6fcb7bdbf1d91fc82dc9dcfba62ee`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87fc1eae5da293ad72b1e887673101bc88b41da34be266e0cb9ffb925b1cd9e`  
		Last Modified: Fri, 02 Sep 2022 05:37:20 GMT  
		Size: 85.1 MB (85128514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c839d061ae3488844d609e2d33783651ac4f61a1ac2a3ab91e5843ffb46c09`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7ad044b07820a01e4f3d7d005bcc5b85daddee7d33023b78e2b70415e93c39`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb528ea63c8052a53adc17b551adf2d399599d826dc846e12e6f7fdbd043da0`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:03a7284ae289837f4fd263f9c428e9e88b2abf1618c64852f54ba1c07d315fb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136711917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0768ad7800fcff93488beec5327c571ca074cf12db86ed40c84fdc46d30a6fad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:01:06 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:01:08 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:01:09 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:01:09 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:01:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:01:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:01:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:01:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:01:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:01:58 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:01:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:01:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:02:00 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:02:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d30000abbc2f6df020005bbf80afa1517e668ffdb9b1f07fb3b8db7872f7dc`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227b438f458701243e917f16e8e93a71929afda708311e6df3b341ee34677393`  
		Last Modified: Fri, 02 Sep 2022 05:09:40 GMT  
		Size: 90.5 MB (90513260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653986903ee5b2beafc174987abe4b92d51d671d1d0332ff0ae8ac010fad4ab9`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb46793d402c50e96f68ead706d3d8038b1b7148d104abfc504d1d07d673d7e`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cf86fd9242bf89650b9e6d3c3886fdf647a3dca1bebb9c4ed2882c7cb90227`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:1e90e1aae83341869c9938f9df91e140d07df6e87acf9fc958f29f9d71d582e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:5d2aa8c7effe3db2cd2338cc892852c247f26b5ee016372011bb4a906bfac2fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125832212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801fdf0164b268eccd799a793913b7664b7f64ed43a852d97f9daa3bfcca897b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:46:25 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 03:46:25 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 03:46:25 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 03:46:25 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 03:46:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:46:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:46:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:46:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:46:50 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:46:50 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:46:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 03:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:46:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:46:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d194f12d3188cb6b7a11bde77791bbd35326da766a493465b142f98abc3caa`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fb7e8252943bfc6428758bdb8db56078cb61413b90658bef225022398a6c91`  
		Last Modified: Fri, 02 Sep 2022 03:51:21 GMT  
		Size: 85.9 MB (85917901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff39f4020c49372580edeb910dc65d7018e3fd41f3ac7747b76a2c3f146ef85`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5bd8a470bef766b74cdda1f8b8957427767298b4ec30701532008832602b53`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c24d2dc91cbb8ab7b21104ca6bc0678ce2a75602ee92e5112502f60b82e03e`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:024fed356afa64de41a956f6e776f6bd4153cd5942fb998666eeae5c5c5d9ecf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123210931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b620220f60ff7959c4ef01f7e8f924e366c6030a99f6199d7e5e499ab404b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:31:17 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:31:18 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:31:19 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:31:20 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:31:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:31:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:31:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:31:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:31:48 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:31:49 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:31:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:31:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:31:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:31:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6380fc1f620ea4d1844db54f67020beef6fcb7bdbf1d91fc82dc9dcfba62ee`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87fc1eae5da293ad72b1e887673101bc88b41da34be266e0cb9ffb925b1cd9e`  
		Last Modified: Fri, 02 Sep 2022 05:37:20 GMT  
		Size: 85.1 MB (85128514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c839d061ae3488844d609e2d33783651ac4f61a1ac2a3ab91e5843ffb46c09`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7ad044b07820a01e4f3d7d005bcc5b85daddee7d33023b78e2b70415e93c39`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb528ea63c8052a53adc17b551adf2d399599d826dc846e12e6f7fdbd043da0`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:03a7284ae289837f4fd263f9c428e9e88b2abf1618c64852f54ba1c07d315fb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136711917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0768ad7800fcff93488beec5327c571ca074cf12db86ed40c84fdc46d30a6fad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:01:06 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:01:08 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:01:09 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:01:09 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:01:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:01:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:01:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:01:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:01:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:01:58 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:01:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:01:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:02:00 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:02:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d30000abbc2f6df020005bbf80afa1517e668ffdb9b1f07fb3b8db7872f7dc`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227b438f458701243e917f16e8e93a71929afda708311e6df3b341ee34677393`  
		Last Modified: Fri, 02 Sep 2022 05:09:40 GMT  
		Size: 90.5 MB (90513260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653986903ee5b2beafc174987abe4b92d51d671d1d0332ff0ae8ac010fad4ab9`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb46793d402c50e96f68ead706d3d8038b1b7148d104abfc504d1d07d673d7e`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cf86fd9242bf89650b9e6d3c3886fdf647a3dca1bebb9c4ed2882c7cb90227`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.26`

```console
$ docker pull mariadb@sha256:1e90e1aae83341869c9938f9df91e140d07df6e87acf9fc958f29f9d71d582e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.26` - linux; amd64

```console
$ docker pull mariadb@sha256:5d2aa8c7effe3db2cd2338cc892852c247f26b5ee016372011bb4a906bfac2fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125832212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801fdf0164b268eccd799a793913b7664b7f64ed43a852d97f9daa3bfcca897b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:46:25 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 03:46:25 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 03:46:25 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 03:46:25 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 03:46:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:46:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:46:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:46:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:46:50 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:46:50 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:46:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 03:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:46:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:46:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d194f12d3188cb6b7a11bde77791bbd35326da766a493465b142f98abc3caa`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fb7e8252943bfc6428758bdb8db56078cb61413b90658bef225022398a6c91`  
		Last Modified: Fri, 02 Sep 2022 03:51:21 GMT  
		Size: 85.9 MB (85917901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff39f4020c49372580edeb910dc65d7018e3fd41f3ac7747b76a2c3f146ef85`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5bd8a470bef766b74cdda1f8b8957427767298b4ec30701532008832602b53`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c24d2dc91cbb8ab7b21104ca6bc0678ce2a75602ee92e5112502f60b82e03e`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.26` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:024fed356afa64de41a956f6e776f6bd4153cd5942fb998666eeae5c5c5d9ecf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123210931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b620220f60ff7959c4ef01f7e8f924e366c6030a99f6199d7e5e499ab404b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:31:17 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:31:18 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:31:19 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:31:20 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:31:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:31:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:31:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:31:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:31:48 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:31:49 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:31:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:31:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:31:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:31:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6380fc1f620ea4d1844db54f67020beef6fcb7bdbf1d91fc82dc9dcfba62ee`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87fc1eae5da293ad72b1e887673101bc88b41da34be266e0cb9ffb925b1cd9e`  
		Last Modified: Fri, 02 Sep 2022 05:37:20 GMT  
		Size: 85.1 MB (85128514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c839d061ae3488844d609e2d33783651ac4f61a1ac2a3ab91e5843ffb46c09`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7ad044b07820a01e4f3d7d005bcc5b85daddee7d33023b78e2b70415e93c39`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb528ea63c8052a53adc17b551adf2d399599d826dc846e12e6f7fdbd043da0`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.26` - linux; ppc64le

```console
$ docker pull mariadb@sha256:03a7284ae289837f4fd263f9c428e9e88b2abf1618c64852f54ba1c07d315fb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136711917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0768ad7800fcff93488beec5327c571ca074cf12db86ed40c84fdc46d30a6fad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:01:06 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:01:08 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:01:09 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:01:09 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:01:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:01:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:01:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:01:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:01:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:01:58 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:01:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:01:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:02:00 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:02:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d30000abbc2f6df020005bbf80afa1517e668ffdb9b1f07fb3b8db7872f7dc`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227b438f458701243e917f16e8e93a71929afda708311e6df3b341ee34677393`  
		Last Modified: Fri, 02 Sep 2022 05:09:40 GMT  
		Size: 90.5 MB (90513260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653986903ee5b2beafc174987abe4b92d51d671d1d0332ff0ae8ac010fad4ab9`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb46793d402c50e96f68ead706d3d8038b1b7148d104abfc504d1d07d673d7e`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cf86fd9242bf89650b9e6d3c3886fdf647a3dca1bebb9c4ed2882c7cb90227`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.26-focal`

```console
$ docker pull mariadb@sha256:1e90e1aae83341869c9938f9df91e140d07df6e87acf9fc958f29f9d71d582e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.26-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:5d2aa8c7effe3db2cd2338cc892852c247f26b5ee016372011bb4a906bfac2fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125832212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801fdf0164b268eccd799a793913b7664b7f64ed43a852d97f9daa3bfcca897b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:46:25 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 03:46:25 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 03:46:25 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 03:46:25 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 03:46:25 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:46:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:46:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:46:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:46:50 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:46:50 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:46:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 03:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:46:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:46:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d194f12d3188cb6b7a11bde77791bbd35326da766a493465b142f98abc3caa`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fb7e8252943bfc6428758bdb8db56078cb61413b90658bef225022398a6c91`  
		Last Modified: Fri, 02 Sep 2022 03:51:21 GMT  
		Size: 85.9 MB (85917901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff39f4020c49372580edeb910dc65d7018e3fd41f3ac7747b76a2c3f146ef85`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5bd8a470bef766b74cdda1f8b8957427767298b4ec30701532008832602b53`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 6.7 KB (6693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c24d2dc91cbb8ab7b21104ca6bc0678ce2a75602ee92e5112502f60b82e03e`  
		Last Modified: Fri, 02 Sep 2022 03:51:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.26-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:024fed356afa64de41a956f6e776f6bd4153cd5942fb998666eeae5c5c5d9ecf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123210931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b620220f60ff7959c4ef01f7e8f924e366c6030a99f6199d7e5e499ab404b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:31:17 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:31:18 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:31:19 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:31:20 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:31:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:31:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:31:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:31:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:31:48 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:31:49 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:31:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:31:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:31:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:31:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6380fc1f620ea4d1844db54f67020beef6fcb7bdbf1d91fc82dc9dcfba62ee`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87fc1eae5da293ad72b1e887673101bc88b41da34be266e0cb9ffb925b1cd9e`  
		Last Modified: Fri, 02 Sep 2022 05:37:20 GMT  
		Size: 85.1 MB (85128514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c839d061ae3488844d609e2d33783651ac4f61a1ac2a3ab91e5843ffb46c09`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7ad044b07820a01e4f3d7d005bcc5b85daddee7d33023b78e2b70415e93c39`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 6.7 KB (6691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb528ea63c8052a53adc17b551adf2d399599d826dc846e12e6f7fdbd043da0`  
		Last Modified: Fri, 02 Sep 2022 05:37:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.26-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:03a7284ae289837f4fd263f9c428e9e88b2abf1618c64852f54ba1c07d315fb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136711917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0768ad7800fcff93488beec5327c571ca074cf12db86ed40c84fdc46d30a6fad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:01:06 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:01:08 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 02 Sep 2022 05:01:09 GMT
ARG MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:01:09 GMT
ENV MARIADB_VERSION=1:10.4.26+maria~ubu2004
# Fri, 02 Sep 2022 05:01:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:01:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:01:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:01:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:01:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:01:58 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:01:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.26/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 02 Sep 2022 05:01:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:02:00 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:02:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d30000abbc2f6df020005bbf80afa1517e668ffdb9b1f07fb3b8db7872f7dc`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227b438f458701243e917f16e8e93a71929afda708311e6df3b341ee34677393`  
		Last Modified: Fri, 02 Sep 2022 05:09:40 GMT  
		Size: 90.5 MB (90513260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653986903ee5b2beafc174987abe4b92d51d671d1d0332ff0ae8ac010fad4ab9`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb46793d402c50e96f68ead706d3d8038b1b7148d104abfc504d1d07d673d7e`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cf86fd9242bf89650b9e6d3c3886fdf647a3dca1bebb9c4ed2882c7cb90227`  
		Last Modified: Fri, 02 Sep 2022 05:09:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:cb223c17bab451f086e863be6c0ae044d91a475c2e0986a576fddc5ebd8b03c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:9820c6d202c51def1ba10b398f69f4ba7d476482a6bacadabb1039644b7e304c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128133913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ded61f9b39628701b04d45359e6b4dfdc6494df043639a4e5866f928f010e945`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:45:57 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 03:45:57 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 03:45:57 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 03:45:57 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 03:45:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:45:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:46:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:46:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:46:20 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:46:21 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:46:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:46:21 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8650645dae7f81a214cdf6de7f1979757cdc06f104591a0598810d28bf22f3b4`  
		Last Modified: Fri, 02 Sep 2022 03:50:40 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395951e93aec60db53c293ee03869529f603b202b521da9a49a4e8cbbc0a489d`  
		Last Modified: Fri, 02 Sep 2022 03:50:52 GMT  
		Size: 88.2 MB (88219725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388c2c464b5a0a20263e3f6c4d6ffeaece0b64463caae20762b096cf9d120ca6`  
		Last Modified: Fri, 02 Sep 2022 03:50:39 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60223e07c9539952a8c536a9c6ebdf8ea188c8e4aa09779db2654e5414fb9824`  
		Last Modified: Fri, 02 Sep 2022 03:50:39 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6563f42f22ac9854d9651ec6c8678078cf39279d0e05b11844d04d7fc0948f32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125417664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d677303da6117bdf07de5e86e33e315437f39f3754aaeede633e57913bacd5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:30:41 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:30:41 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:30:42 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:30:43 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:30:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:30:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:31:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:31:07 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:31:08 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:31:09 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:31:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:31:10 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:31:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec09ee861f5efa74b5cf683c495565ad8c38749fa75bb9253d2239d3d2316c9`  
		Last Modified: Fri, 02 Sep 2022 05:36:36 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944eea0f56d9f2c8d2bdf1cba8834e470277f239ba0878decab2bd4722fab03d`  
		Last Modified: Fri, 02 Sep 2022 05:36:49 GMT  
		Size: 87.3 MB (87335376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfe4ac7e653b1699aa2cfe0be6d568b51562feb938a34b96cc10d767e05618a`  
		Last Modified: Fri, 02 Sep 2022 05:36:36 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b7baa3ce703ce066272ea62da81c1770b54cd404e38dcfc91e468fb6bf7b55`  
		Last Modified: Fri, 02 Sep 2022 05:36:36 GMT  
		Size: 6.7 KB (6686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5cbde6efcc94cc2a8dc06f503824d0eadbfa64898d51385ac2c76fa0861f8608
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138986000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad4d7b4580bbb4a0b0ec50c8b972e3039d0bc090beb68a45dd6f706796cb93e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:00:06 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:00:06 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:00:07 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:00:07 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:00:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:00:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:00:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:00:55 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:00:55 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:00:56 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:00:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:00:57 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:00:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ff2f2b22d087b136c098a411d584ab880b30cc3292349a5aad7fa31044ab19`  
		Last Modified: Fri, 02 Sep 2022 05:08:31 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4167723e071b265f11e3a2657897a60ebfcdd111f6d8063d561d12301d138b51`  
		Last Modified: Fri, 02 Sep 2022 05:08:55 GMT  
		Size: 92.8 MB (92787463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81389c4e7e9f6ac9f61fb353af9afc5c2f894b6ef577671254025f7c01139786`  
		Last Modified: Fri, 02 Sep 2022 05:08:31 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2db2c0414c318751c9d9a73b17333d1d2db9c3f8c4393aac957609ed961b9cc`  
		Last Modified: Fri, 02 Sep 2022 05:08:31 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; s390x

```console
$ docker pull mariadb@sha256:ca881315a1b3d98956747c5035db009cd9f4f0ed5629be840bc041776ad5843b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127350328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8708644290aca0fa955ef35e861fee938891d05c15d5065c8016e66c6f096c2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:20:37 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:20:43 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:20:52 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:20:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:20:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:20:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:22:10 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 02:22:10 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 02:22:10 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 02:22:10 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 02:22:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 02:22:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:22:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:22:36 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:22:36 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:22:37 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:22:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:22:37 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:22:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4074f18b54e21cd0e65811b1690ca103650cccbb8729233dea9b7f319f326e85`  
		Last Modified: Fri, 02 Sep 2022 02:24:57 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfde2f51ff0ee80f91c71818c78bb17bb5aad9ad1842d539f1fc1fc1600124b`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 5.4 MB (5372683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096750bf78c944bdb3aa044f8a91f3464702ff5b3835b1a03cbc0ed01f69b925`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 3.2 MB (3240190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd1d5232a1658cfbf3e897edcf448ab3e9c9694dda8d4e129df83c0bae21f9f`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f11090d6fc460a6639be04bf456fdf26e7979fabbf746cb590b589c795b830`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 2.2 MB (2168128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e8c9ae606cfbddb9544fb07bf10d7a4e2600a823df49af117309ee6251b7bf`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d2b1eb2facbef7fcdd98e89e6718e02931f71caa4743e07463689b7eaba969`  
		Last Modified: Fri, 02 Sep 2022 02:25:44 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83d047bbd6d9e4908e7f4d1242970a7a02199736ceb9b4ff2e8b39553365ffc`  
		Last Modified: Fri, 02 Sep 2022 02:25:56 GMT  
		Size: 89.5 MB (89509148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb91d85f85d7c5010237093c02f5365ea4944205ad973b3e88e14c9e44ec56a`  
		Last Modified: Fri, 02 Sep 2022 02:25:44 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe58f9e0aaab866ff7d8522a7b7c9c2003beb31f2915dd325a5525f26f00c28`  
		Last Modified: Fri, 02 Sep 2022 02:25:44 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:cb223c17bab451f086e863be6c0ae044d91a475c2e0986a576fddc5ebd8b03c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:9820c6d202c51def1ba10b398f69f4ba7d476482a6bacadabb1039644b7e304c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128133913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ded61f9b39628701b04d45359e6b4dfdc6494df043639a4e5866f928f010e945`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:45:57 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 03:45:57 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 03:45:57 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 03:45:57 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 03:45:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:45:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:46:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:46:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:46:20 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:46:21 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:46:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:46:21 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8650645dae7f81a214cdf6de7f1979757cdc06f104591a0598810d28bf22f3b4`  
		Last Modified: Fri, 02 Sep 2022 03:50:40 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395951e93aec60db53c293ee03869529f603b202b521da9a49a4e8cbbc0a489d`  
		Last Modified: Fri, 02 Sep 2022 03:50:52 GMT  
		Size: 88.2 MB (88219725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388c2c464b5a0a20263e3f6c4d6ffeaece0b64463caae20762b096cf9d120ca6`  
		Last Modified: Fri, 02 Sep 2022 03:50:39 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60223e07c9539952a8c536a9c6ebdf8ea188c8e4aa09779db2654e5414fb9824`  
		Last Modified: Fri, 02 Sep 2022 03:50:39 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6563f42f22ac9854d9651ec6c8678078cf39279d0e05b11844d04d7fc0948f32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125417664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d677303da6117bdf07de5e86e33e315437f39f3754aaeede633e57913bacd5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:30:41 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:30:41 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:30:42 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:30:43 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:30:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:30:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:31:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:31:07 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:31:08 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:31:09 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:31:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:31:10 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:31:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec09ee861f5efa74b5cf683c495565ad8c38749fa75bb9253d2239d3d2316c9`  
		Last Modified: Fri, 02 Sep 2022 05:36:36 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944eea0f56d9f2c8d2bdf1cba8834e470277f239ba0878decab2bd4722fab03d`  
		Last Modified: Fri, 02 Sep 2022 05:36:49 GMT  
		Size: 87.3 MB (87335376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfe4ac7e653b1699aa2cfe0be6d568b51562feb938a34b96cc10d767e05618a`  
		Last Modified: Fri, 02 Sep 2022 05:36:36 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b7baa3ce703ce066272ea62da81c1770b54cd404e38dcfc91e468fb6bf7b55`  
		Last Modified: Fri, 02 Sep 2022 05:36:36 GMT  
		Size: 6.7 KB (6686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5cbde6efcc94cc2a8dc06f503824d0eadbfa64898d51385ac2c76fa0861f8608
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138986000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad4d7b4580bbb4a0b0ec50c8b972e3039d0bc090beb68a45dd6f706796cb93e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:00:06 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:00:06 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:00:07 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:00:07 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:00:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:00:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:00:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:00:55 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:00:55 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:00:56 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:00:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:00:57 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:00:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ff2f2b22d087b136c098a411d584ab880b30cc3292349a5aad7fa31044ab19`  
		Last Modified: Fri, 02 Sep 2022 05:08:31 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4167723e071b265f11e3a2657897a60ebfcdd111f6d8063d561d12301d138b51`  
		Last Modified: Fri, 02 Sep 2022 05:08:55 GMT  
		Size: 92.8 MB (92787463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81389c4e7e9f6ac9f61fb353af9afc5c2f894b6ef577671254025f7c01139786`  
		Last Modified: Fri, 02 Sep 2022 05:08:31 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2db2c0414c318751c9d9a73b17333d1d2db9c3f8c4393aac957609ed961b9cc`  
		Last Modified: Fri, 02 Sep 2022 05:08:31 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:ca881315a1b3d98956747c5035db009cd9f4f0ed5629be840bc041776ad5843b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127350328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8708644290aca0fa955ef35e861fee938891d05c15d5065c8016e66c6f096c2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:20:37 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:20:43 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:20:52 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:20:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:20:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:20:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:22:10 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 02:22:10 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 02:22:10 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 02:22:10 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 02:22:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 02:22:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:22:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:22:36 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:22:36 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:22:37 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:22:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:22:37 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:22:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4074f18b54e21cd0e65811b1690ca103650cccbb8729233dea9b7f319f326e85`  
		Last Modified: Fri, 02 Sep 2022 02:24:57 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfde2f51ff0ee80f91c71818c78bb17bb5aad9ad1842d539f1fc1fc1600124b`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 5.4 MB (5372683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096750bf78c944bdb3aa044f8a91f3464702ff5b3835b1a03cbc0ed01f69b925`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 3.2 MB (3240190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd1d5232a1658cfbf3e897edcf448ab3e9c9694dda8d4e129df83c0bae21f9f`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f11090d6fc460a6639be04bf456fdf26e7979fabbf746cb590b589c795b830`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 2.2 MB (2168128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e8c9ae606cfbddb9544fb07bf10d7a4e2600a823df49af117309ee6251b7bf`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d2b1eb2facbef7fcdd98e89e6718e02931f71caa4743e07463689b7eaba969`  
		Last Modified: Fri, 02 Sep 2022 02:25:44 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83d047bbd6d9e4908e7f4d1242970a7a02199736ceb9b4ff2e8b39553365ffc`  
		Last Modified: Fri, 02 Sep 2022 02:25:56 GMT  
		Size: 89.5 MB (89509148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb91d85f85d7c5010237093c02f5365ea4944205ad973b3e88e14c9e44ec56a`  
		Last Modified: Fri, 02 Sep 2022 02:25:44 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe58f9e0aaab866ff7d8522a7b7c9c2003beb31f2915dd325a5525f26f00c28`  
		Last Modified: Fri, 02 Sep 2022 02:25:44 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.17`

```console
$ docker pull mariadb@sha256:cb223c17bab451f086e863be6c0ae044d91a475c2e0986a576fddc5ebd8b03c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.17` - linux; amd64

```console
$ docker pull mariadb@sha256:9820c6d202c51def1ba10b398f69f4ba7d476482a6bacadabb1039644b7e304c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128133913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ded61f9b39628701b04d45359e6b4dfdc6494df043639a4e5866f928f010e945`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:45:57 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 03:45:57 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 03:45:57 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 03:45:57 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 03:45:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:45:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:46:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:46:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:46:20 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:46:21 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:46:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:46:21 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8650645dae7f81a214cdf6de7f1979757cdc06f104591a0598810d28bf22f3b4`  
		Last Modified: Fri, 02 Sep 2022 03:50:40 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395951e93aec60db53c293ee03869529f603b202b521da9a49a4e8cbbc0a489d`  
		Last Modified: Fri, 02 Sep 2022 03:50:52 GMT  
		Size: 88.2 MB (88219725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388c2c464b5a0a20263e3f6c4d6ffeaece0b64463caae20762b096cf9d120ca6`  
		Last Modified: Fri, 02 Sep 2022 03:50:39 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60223e07c9539952a8c536a9c6ebdf8ea188c8e4aa09779db2654e5414fb9824`  
		Last Modified: Fri, 02 Sep 2022 03:50:39 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.17` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6563f42f22ac9854d9651ec6c8678078cf39279d0e05b11844d04d7fc0948f32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125417664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d677303da6117bdf07de5e86e33e315437f39f3754aaeede633e57913bacd5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:30:41 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:30:41 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:30:42 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:30:43 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:30:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:30:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:31:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:31:07 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:31:08 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:31:09 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:31:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:31:10 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:31:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec09ee861f5efa74b5cf683c495565ad8c38749fa75bb9253d2239d3d2316c9`  
		Last Modified: Fri, 02 Sep 2022 05:36:36 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944eea0f56d9f2c8d2bdf1cba8834e470277f239ba0878decab2bd4722fab03d`  
		Last Modified: Fri, 02 Sep 2022 05:36:49 GMT  
		Size: 87.3 MB (87335376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfe4ac7e653b1699aa2cfe0be6d568b51562feb938a34b96cc10d767e05618a`  
		Last Modified: Fri, 02 Sep 2022 05:36:36 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b7baa3ce703ce066272ea62da81c1770b54cd404e38dcfc91e468fb6bf7b55`  
		Last Modified: Fri, 02 Sep 2022 05:36:36 GMT  
		Size: 6.7 KB (6686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.17` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5cbde6efcc94cc2a8dc06f503824d0eadbfa64898d51385ac2c76fa0861f8608
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138986000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad4d7b4580bbb4a0b0ec50c8b972e3039d0bc090beb68a45dd6f706796cb93e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:00:06 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:00:06 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:00:07 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:00:07 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:00:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:00:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:00:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:00:55 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:00:55 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:00:56 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:00:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:00:57 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:00:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ff2f2b22d087b136c098a411d584ab880b30cc3292349a5aad7fa31044ab19`  
		Last Modified: Fri, 02 Sep 2022 05:08:31 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4167723e071b265f11e3a2657897a60ebfcdd111f6d8063d561d12301d138b51`  
		Last Modified: Fri, 02 Sep 2022 05:08:55 GMT  
		Size: 92.8 MB (92787463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81389c4e7e9f6ac9f61fb353af9afc5c2f894b6ef577671254025f7c01139786`  
		Last Modified: Fri, 02 Sep 2022 05:08:31 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2db2c0414c318751c9d9a73b17333d1d2db9c3f8c4393aac957609ed961b9cc`  
		Last Modified: Fri, 02 Sep 2022 05:08:31 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.17` - linux; s390x

```console
$ docker pull mariadb@sha256:ca881315a1b3d98956747c5035db009cd9f4f0ed5629be840bc041776ad5843b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127350328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8708644290aca0fa955ef35e861fee938891d05c15d5065c8016e66c6f096c2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:20:37 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:20:43 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:20:52 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:20:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:20:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:20:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:22:10 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 02:22:10 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 02:22:10 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 02:22:10 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 02:22:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 02:22:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:22:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:22:36 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:22:36 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:22:37 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:22:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:22:37 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:22:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4074f18b54e21cd0e65811b1690ca103650cccbb8729233dea9b7f319f326e85`  
		Last Modified: Fri, 02 Sep 2022 02:24:57 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfde2f51ff0ee80f91c71818c78bb17bb5aad9ad1842d539f1fc1fc1600124b`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 5.4 MB (5372683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096750bf78c944bdb3aa044f8a91f3464702ff5b3835b1a03cbc0ed01f69b925`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 3.2 MB (3240190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd1d5232a1658cfbf3e897edcf448ab3e9c9694dda8d4e129df83c0bae21f9f`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f11090d6fc460a6639be04bf456fdf26e7979fabbf746cb590b589c795b830`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 2.2 MB (2168128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e8c9ae606cfbddb9544fb07bf10d7a4e2600a823df49af117309ee6251b7bf`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d2b1eb2facbef7fcdd98e89e6718e02931f71caa4743e07463689b7eaba969`  
		Last Modified: Fri, 02 Sep 2022 02:25:44 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83d047bbd6d9e4908e7f4d1242970a7a02199736ceb9b4ff2e8b39553365ffc`  
		Last Modified: Fri, 02 Sep 2022 02:25:56 GMT  
		Size: 89.5 MB (89509148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb91d85f85d7c5010237093c02f5365ea4944205ad973b3e88e14c9e44ec56a`  
		Last Modified: Fri, 02 Sep 2022 02:25:44 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe58f9e0aaab866ff7d8522a7b7c9c2003beb31f2915dd325a5525f26f00c28`  
		Last Modified: Fri, 02 Sep 2022 02:25:44 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.17-focal`

```console
$ docker pull mariadb@sha256:cb223c17bab451f086e863be6c0ae044d91a475c2e0986a576fddc5ebd8b03c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.17-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:9820c6d202c51def1ba10b398f69f4ba7d476482a6bacadabb1039644b7e304c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128133913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ded61f9b39628701b04d45359e6b4dfdc6494df043639a4e5866f928f010e945`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:45:57 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 03:45:57 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 03:45:57 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 03:45:57 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 03:45:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:45:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:46:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:46:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:46:20 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:46:21 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:46:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:46:21 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:46:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8650645dae7f81a214cdf6de7f1979757cdc06f104591a0598810d28bf22f3b4`  
		Last Modified: Fri, 02 Sep 2022 03:50:40 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395951e93aec60db53c293ee03869529f603b202b521da9a49a4e8cbbc0a489d`  
		Last Modified: Fri, 02 Sep 2022 03:50:52 GMT  
		Size: 88.2 MB (88219725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388c2c464b5a0a20263e3f6c4d6ffeaece0b64463caae20762b096cf9d120ca6`  
		Last Modified: Fri, 02 Sep 2022 03:50:39 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60223e07c9539952a8c536a9c6ebdf8ea188c8e4aa09779db2654e5414fb9824`  
		Last Modified: Fri, 02 Sep 2022 03:50:39 GMT  
		Size: 6.7 KB (6694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.17-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6563f42f22ac9854d9651ec6c8678078cf39279d0e05b11844d04d7fc0948f32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125417664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d677303da6117bdf07de5e86e33e315437f39f3754aaeede633e57913bacd5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:30:41 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:30:41 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:30:42 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:30:43 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:30:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:30:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:31:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:31:07 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:31:08 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:31:09 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:31:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:31:10 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:31:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec09ee861f5efa74b5cf683c495565ad8c38749fa75bb9253d2239d3d2316c9`  
		Last Modified: Fri, 02 Sep 2022 05:36:36 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944eea0f56d9f2c8d2bdf1cba8834e470277f239ba0878decab2bd4722fab03d`  
		Last Modified: Fri, 02 Sep 2022 05:36:49 GMT  
		Size: 87.3 MB (87335376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfe4ac7e653b1699aa2cfe0be6d568b51562feb938a34b96cc10d767e05618a`  
		Last Modified: Fri, 02 Sep 2022 05:36:36 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b7baa3ce703ce066272ea62da81c1770b54cd404e38dcfc91e468fb6bf7b55`  
		Last Modified: Fri, 02 Sep 2022 05:36:36 GMT  
		Size: 6.7 KB (6686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.17-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:5cbde6efcc94cc2a8dc06f503824d0eadbfa64898d51385ac2c76fa0861f8608
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138986000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad4d7b4580bbb4a0b0ec50c8b972e3039d0bc090beb68a45dd6f706796cb93e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:00:06 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:00:06 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 05:00:07 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:00:07 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 05:00:07 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:00:08 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:00:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:00:55 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:00:55 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:00:56 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:00:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:00:57 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:00:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ff2f2b22d087b136c098a411d584ab880b30cc3292349a5aad7fa31044ab19`  
		Last Modified: Fri, 02 Sep 2022 05:08:31 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4167723e071b265f11e3a2657897a60ebfcdd111f6d8063d561d12301d138b51`  
		Last Modified: Fri, 02 Sep 2022 05:08:55 GMT  
		Size: 92.8 MB (92787463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81389c4e7e9f6ac9f61fb353af9afc5c2f894b6ef577671254025f7c01139786`  
		Last Modified: Fri, 02 Sep 2022 05:08:31 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2db2c0414c318751c9d9a73b17333d1d2db9c3f8c4393aac957609ed961b9cc`  
		Last Modified: Fri, 02 Sep 2022 05:08:31 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.17-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:ca881315a1b3d98956747c5035db009cd9f4f0ed5629be840bc041776ad5843b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127350328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8708644290aca0fa955ef35e861fee938891d05c15d5065c8016e66c6f096c2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:20:37 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:20:43 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:20:52 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:20:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:20:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:20:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:22:10 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 02:22:10 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 02 Sep 2022 02:22:10 GMT
ARG MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 02:22:10 GMT
ENV MARIADB_VERSION=1:10.5.17+maria~ubu2004
# Fri, 02 Sep 2022 02:22:10 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 02:22:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:22:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.17/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:22:36 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:22:36 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:22:37 GMT
COPY file:e0d9e49f1adbc1c1e2354d2dcc8c48beb9502a927b871b6815dba1ac953e0d0a in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:22:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:22:37 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:22:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4074f18b54e21cd0e65811b1690ca103650cccbb8729233dea9b7f319f326e85`  
		Last Modified: Fri, 02 Sep 2022 02:24:57 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfde2f51ff0ee80f91c71818c78bb17bb5aad9ad1842d539f1fc1fc1600124b`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 5.4 MB (5372683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096750bf78c944bdb3aa044f8a91f3464702ff5b3835b1a03cbc0ed01f69b925`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 3.2 MB (3240190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd1d5232a1658cfbf3e897edcf448ab3e9c9694dda8d4e129df83c0bae21f9f`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f11090d6fc460a6639be04bf456fdf26e7979fabbf746cb590b589c795b830`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 2.2 MB (2168128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e8c9ae606cfbddb9544fb07bf10d7a4e2600a823df49af117309ee6251b7bf`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d2b1eb2facbef7fcdd98e89e6718e02931f71caa4743e07463689b7eaba969`  
		Last Modified: Fri, 02 Sep 2022 02:25:44 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83d047bbd6d9e4908e7f4d1242970a7a02199736ceb9b4ff2e8b39553365ffc`  
		Last Modified: Fri, 02 Sep 2022 02:25:56 GMT  
		Size: 89.5 MB (89509148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb91d85f85d7c5010237093c02f5365ea4944205ad973b3e88e14c9e44ec56a`  
		Last Modified: Fri, 02 Sep 2022 02:25:44 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe58f9e0aaab866ff7d8522a7b7c9c2003beb31f2915dd325a5525f26f00c28`  
		Last Modified: Fri, 02 Sep 2022 02:25:44 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:733ee31632f417be30c80e02268df02ce039016af47d05e291a84f434b2aeef1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:88aaef966a22d39b83e24480588f5ba009e3834d4558dc19c527577439e52616
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128399441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac83b09b249a9c8213ae3cd378de584e4a31a055965b8d3af1dcb6d0ad2ed4ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:45:23 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 03:45:23 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 03:45:23 GMT
ARG MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 03:45:23 GMT
ENV MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 03:45:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:45:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:45:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:45:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:45:50 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:45:50 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:45:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:45:50 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:45:50 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d056f5551d17907ef0b8ce7bea180b4a0e0b4804934abab590fe9c9e55fb424a`  
		Last Modified: Fri, 02 Sep 2022 03:50:07 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122bd4634fa46b1bd3abf926bac0f9416d9d046e624c1317025ef42c271b815a`  
		Last Modified: Fri, 02 Sep 2022 03:50:23 GMT  
		Size: 88.5 MB (88485255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325066d6ef1f969decff991d5a34d9ba8c30df6954609786d3a0359916f7160a`  
		Last Modified: Fri, 02 Sep 2022 03:50:07 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c3ef15c487e9d5bfa41475662f9e9ef4be2fedcdb56b7348dda25ed2b931de`  
		Last Modified: Fri, 02 Sep 2022 03:50:07 GMT  
		Size: 6.7 KB (6695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:88f684f8c96cd9130a57c9c8249f068fe99d22e97715701e04b3d3232454d1dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125507229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:919a8331fc65bee8399f5d5458e887f6984e2e1c979d56214c02add520a2b68f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:29:57 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 05:29:58 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 05:29:59 GMT
ARG MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 05:30:00 GMT
ENV MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 05:30:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:30:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:30:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:30:25 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:30:27 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:30:28 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:30:29 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:30:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15059ebc811e586e3a1027fadd4dd48a67180a3f56e4717f361616cf5625d66`  
		Last Modified: Fri, 02 Sep 2022 05:36:04 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741678cc2b7812bac1dcabd4ae49d3999224015d4cf4a2c25fc93ac042203c6f`  
		Last Modified: Fri, 02 Sep 2022 05:36:17 GMT  
		Size: 87.4 MB (87424932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a252ae5930e748dd36d17dea6d255e6fed1d275929d0b1cb266f9ddeabccf6f`  
		Last Modified: Fri, 02 Sep 2022 05:36:04 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652f0cff833e23c157e974113fa97905ed7723625a4b893bb01d470373b866b5`  
		Last Modified: Fri, 02 Sep 2022 05:36:05 GMT  
		Size: 6.7 KB (6697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:673cff035456c934fc60d972c4801515ad4be89d86672e60408fe886c5d0c838
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.1 MB (139078844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995f3ded2149053826af32486aa23787eac21cd15811c553a3dd68e0f69f31f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:59:06 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 04:59:07 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 04:59:07 GMT
ARG MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 04:59:07 GMT
ENV MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 04:59:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 04:59:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:59:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:59:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:59:57 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:59:57 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:59:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:59:58 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:59:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0357631f286c401e24f8d62bb5e04d7dd01a7d40b9fe471480c0b86017acaff8`  
		Last Modified: Fri, 02 Sep 2022 05:07:41 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf9394c15655d332d52ec30176fbfe8ff211439cb61efa35dfda3117b8179f9`  
		Last Modified: Fri, 02 Sep 2022 05:08:10 GMT  
		Size: 92.9 MB (92880305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85eec6924fedc28889fea0bfdc05191dd53b9929f896f5481273278c11e4b379`  
		Last Modified: Fri, 02 Sep 2022 05:07:41 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0804dc6d8c94fe3676459da4060f5321fe82b7e98130bea6558524c4457026b`  
		Last Modified: Fri, 02 Sep 2022 05:07:41 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; s390x

```console
$ docker pull mariadb@sha256:a1440b7bbee96ad86e263bc60b419c3ebde79cea3697cd7500d0fc6cd5e74df5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127384584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86bdbbae87c58c7482aab15f0fe245837a223e64796bf7b81745632bccdfb841`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:20:37 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:20:43 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:20:52 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:20:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:20:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:20:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:21:37 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 02:21:37 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 02:21:37 GMT
ARG MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 02:21:37 GMT
ENV MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 02:21:37 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 02:21:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:21:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:22:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:22:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:22:02 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:22:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:22:03 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:22:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4074f18b54e21cd0e65811b1690ca103650cccbb8729233dea9b7f319f326e85`  
		Last Modified: Fri, 02 Sep 2022 02:24:57 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfde2f51ff0ee80f91c71818c78bb17bb5aad9ad1842d539f1fc1fc1600124b`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 5.4 MB (5372683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096750bf78c944bdb3aa044f8a91f3464702ff5b3835b1a03cbc0ed01f69b925`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 3.2 MB (3240190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd1d5232a1658cfbf3e897edcf448ab3e9c9694dda8d4e129df83c0bae21f9f`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f11090d6fc460a6639be04bf456fdf26e7979fabbf746cb590b589c795b830`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 2.2 MB (2168128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e8c9ae606cfbddb9544fb07bf10d7a4e2600a823df49af117309ee6251b7bf`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a261cd92ba1153aee1b403adb349c3baa10900ae7212adf3ec60e6d54f0f01`  
		Last Modified: Fri, 02 Sep 2022 02:25:19 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3caa29af4f4658b064cf93fc6e9618553ba9f97b09a2906b63da1419081e55e4`  
		Last Modified: Fri, 02 Sep 2022 02:25:32 GMT  
		Size: 89.5 MB (89543400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454b3cf2f11ec28c3cbb59573ccb5da2ac07278784efe19c5e74651857302562`  
		Last Modified: Fri, 02 Sep 2022 02:25:19 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9ed6fa2c09e1fe741bff204b62b7d21319da4e2673ec003848925bf8ae5c32`  
		Last Modified: Fri, 02 Sep 2022 02:25:19 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:733ee31632f417be30c80e02268df02ce039016af47d05e291a84f434b2aeef1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:88aaef966a22d39b83e24480588f5ba009e3834d4558dc19c527577439e52616
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128399441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac83b09b249a9c8213ae3cd378de584e4a31a055965b8d3af1dcb6d0ad2ed4ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:45:23 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 03:45:23 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 03:45:23 GMT
ARG MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 03:45:23 GMT
ENV MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 03:45:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:45:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:45:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:45:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:45:50 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:45:50 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:45:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:45:50 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:45:50 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d056f5551d17907ef0b8ce7bea180b4a0e0b4804934abab590fe9c9e55fb424a`  
		Last Modified: Fri, 02 Sep 2022 03:50:07 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122bd4634fa46b1bd3abf926bac0f9416d9d046e624c1317025ef42c271b815a`  
		Last Modified: Fri, 02 Sep 2022 03:50:23 GMT  
		Size: 88.5 MB (88485255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325066d6ef1f969decff991d5a34d9ba8c30df6954609786d3a0359916f7160a`  
		Last Modified: Fri, 02 Sep 2022 03:50:07 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c3ef15c487e9d5bfa41475662f9e9ef4be2fedcdb56b7348dda25ed2b931de`  
		Last Modified: Fri, 02 Sep 2022 03:50:07 GMT  
		Size: 6.7 KB (6695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:88f684f8c96cd9130a57c9c8249f068fe99d22e97715701e04b3d3232454d1dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125507229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:919a8331fc65bee8399f5d5458e887f6984e2e1c979d56214c02add520a2b68f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:29:57 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 05:29:58 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 05:29:59 GMT
ARG MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 05:30:00 GMT
ENV MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 05:30:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:30:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:30:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:30:25 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:30:27 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:30:28 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:30:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:30:29 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:30:30 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15059ebc811e586e3a1027fadd4dd48a67180a3f56e4717f361616cf5625d66`  
		Last Modified: Fri, 02 Sep 2022 05:36:04 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741678cc2b7812bac1dcabd4ae49d3999224015d4cf4a2c25fc93ac042203c6f`  
		Last Modified: Fri, 02 Sep 2022 05:36:17 GMT  
		Size: 87.4 MB (87424932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a252ae5930e748dd36d17dea6d255e6fed1d275929d0b1cb266f9ddeabccf6f`  
		Last Modified: Fri, 02 Sep 2022 05:36:04 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652f0cff833e23c157e974113fa97905ed7723625a4b893bb01d470373b866b5`  
		Last Modified: Fri, 02 Sep 2022 05:36:05 GMT  
		Size: 6.7 KB (6697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:673cff035456c934fc60d972c4801515ad4be89d86672e60408fe886c5d0c838
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.1 MB (139078844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995f3ded2149053826af32486aa23787eac21cd15811c553a3dd68e0f69f31f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:59:06 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 04:59:07 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 04:59:07 GMT
ARG MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 04:59:07 GMT
ENV MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 04:59:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 04:59:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:59:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:59:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:59:57 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:59:57 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:59:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:59:58 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:59:58 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0357631f286c401e24f8d62bb5e04d7dd01a7d40b9fe471480c0b86017acaff8`  
		Last Modified: Fri, 02 Sep 2022 05:07:41 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf9394c15655d332d52ec30176fbfe8ff211439cb61efa35dfda3117b8179f9`  
		Last Modified: Fri, 02 Sep 2022 05:08:10 GMT  
		Size: 92.9 MB (92880305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85eec6924fedc28889fea0bfdc05191dd53b9929f896f5481273278c11e4b379`  
		Last Modified: Fri, 02 Sep 2022 05:07:41 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0804dc6d8c94fe3676459da4060f5321fe82b7e98130bea6558524c4457026b`  
		Last Modified: Fri, 02 Sep 2022 05:07:41 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:a1440b7bbee96ad86e263bc60b419c3ebde79cea3697cd7500d0fc6cd5e74df5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127384584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86bdbbae87c58c7482aab15f0fe245837a223e64796bf7b81745632bccdfb841`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:20:37 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:20:43 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:20:52 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:20:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:20:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:20:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:21:37 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 02:21:37 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 02 Sep 2022 02:21:37 GMT
ARG MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 02:21:37 GMT
ENV MARIADB_VERSION=1:10.6.9+maria~ubu2004
# Fri, 02 Sep 2022 02:21:37 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 02:21:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:21:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.9/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:22:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:22:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:22:02 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:22:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:22:03 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:22:03 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4074f18b54e21cd0e65811b1690ca103650cccbb8729233dea9b7f319f326e85`  
		Last Modified: Fri, 02 Sep 2022 02:24:57 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfde2f51ff0ee80f91c71818c78bb17bb5aad9ad1842d539f1fc1fc1600124b`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 5.4 MB (5372683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096750bf78c944bdb3aa044f8a91f3464702ff5b3835b1a03cbc0ed01f69b925`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 3.2 MB (3240190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd1d5232a1658cfbf3e897edcf448ab3e9c9694dda8d4e129df83c0bae21f9f`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f11090d6fc460a6639be04bf456fdf26e7979fabbf746cb590b589c795b830`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 2.2 MB (2168128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e8c9ae606cfbddb9544fb07bf10d7a4e2600a823df49af117309ee6251b7bf`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a261cd92ba1153aee1b403adb349c3baa10900ae7212adf3ec60e6d54f0f01`  
		Last Modified: Fri, 02 Sep 2022 02:25:19 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3caa29af4f4658b064cf93fc6e9618553ba9f97b09a2906b63da1419081e55e4`  
		Last Modified: Fri, 02 Sep 2022 02:25:32 GMT  
		Size: 89.5 MB (89543400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454b3cf2f11ec28c3cbb59573ccb5da2ac07278784efe19c5e74651857302562`  
		Last Modified: Fri, 02 Sep 2022 02:25:19 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9ed6fa2c09e1fe741bff204b62b7d21319da4e2673ec003848925bf8ae5c32`  
		Last Modified: Fri, 02 Sep 2022 02:25:19 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.10`

**does not exist** (yet?)

## `mariadb:10.6.10-focal`

**does not exist** (yet?)

## `mariadb:10.7`

```console
$ docker pull mariadb@sha256:182c04ae1957dc0caa04fc993eb922f1d4cbdfc70fed9a0d62a35881962e6c45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7` - linux; amd64

```console
$ docker pull mariadb@sha256:1fbc9536ec90869d61de7f261a7caf5d25770421242cb92a5b7495994ffd3f52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128874652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4492bfbc19572e4e9e1555614ec440d80e85ed8cbd3bdcdfeffe27fbd98b74e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:44:41 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 03:44:42 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 03:44:42 GMT
ARG MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 03:44:42 GMT
ENV MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 03:44:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:44:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:45:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:45:13 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:45:13 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:45:14 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:45:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:45:14 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:45:14 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e579c77c079167ac4cf2b00a4c5f95842fb8bb961458fc24955021f59f105eee`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59833a90b3fdea3c70ff5a43637b5f76944a165a73e96ef48a1e5ddb399fbc24`  
		Last Modified: Fri, 02 Sep 2022 03:49:51 GMT  
		Size: 89.0 MB (88960462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94b681c9a42b7e6014d5d5ae2872b82aee86f8403f3cf1529414f57ce0f5b3f`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690bd4563ef7be4647fa90df0d4903fc7589f7f06af5df469aded76057e88e09`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ebe653ef0d86eb70459459deba024a4744134dd1cb7e042c707b0c74fdf12699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126005472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ccde508a2f195c49b96a65f34f85b5d556c9f39d6779b7bb91f0537cd48e327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:29:10 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 05:29:11 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 05:29:12 GMT
ARG MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 05:29:13 GMT
ENV MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 05:29:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:29:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:29:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:29:38 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:29:40 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:29:41 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:29:42 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:29:43 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f78b4c9ee113fa9b65d4009a271140553fea0d672b114b33d6aa14edc33d2ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5088985b5d3cab36c60b6692245368fc2a59c6dd724f9b4518f8f03b27322de2`  
		Last Modified: Fri, 02 Sep 2022 05:35:45 GMT  
		Size: 87.9 MB (87923174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbff1dfc120b4ee7d4c5983038ecc59f81511cc851f13cd4684838c52c4c13c`  
		Last Modified: Fri, 02 Sep 2022 05:35:31 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0309e6b9b27bfd8d2e7331ebcea3866e5aa1d4485397f006b274db8776687340`  
		Last Modified: Fri, 02 Sep 2022 05:35:31 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f91a69470434216dfbecdd7be98bcc278e1673519ff715b549c199549f3d774b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139771204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b88397ea305dda3e5603f4d1f5cc62d6085409faadf0f69df819883e4e48f25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:57:48 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 04:57:49 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 04:57:49 GMT
ARG MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 04:57:49 GMT
ENV MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 04:57:50 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 04:57:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:58:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:58:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:58:51 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:58:51 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:58:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:58:52 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:58:52 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82da8d69fe999cb3782d20c028103ca3217853d613a382fa44172693fd363226`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd8d1fc82c4400d05d6d6ac4f1e7161e9c474ca18e30fbf0d08a391097f2a27`  
		Last Modified: Fri, 02 Sep 2022 05:07:20 GMT  
		Size: 93.6 MB (93572669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95994d7b0f97304e9eeba611de5472538c959c2a056e72845d0e3154bbb75224`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357e4adc4ffc4c8e89dcb8b226aabfe430fbe9b1ab6f0d8bc72dcce9b6b9f5e3`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; s390x

```console
$ docker pull mariadb@sha256:2342b111be5d497cc004951c8f1aeff55ef5de6f6f010e73354f935e9b45fed5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127896553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5442dc97b6f86206b8c450fa1328deed9d2e85b732956a927fae39ebcd069f82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:20:37 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:20:43 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:20:52 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:20:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:20:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:20:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:20:59 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 02:20:59 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 02:20:59 GMT
ARG MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 02:20:59 GMT
ENV MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 02:20:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 02:21:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:21:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:21:28 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:21:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:21:28 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:21:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:21:29 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:21:29 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4074f18b54e21cd0e65811b1690ca103650cccbb8729233dea9b7f319f326e85`  
		Last Modified: Fri, 02 Sep 2022 02:24:57 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfde2f51ff0ee80f91c71818c78bb17bb5aad9ad1842d539f1fc1fc1600124b`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 5.4 MB (5372683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096750bf78c944bdb3aa044f8a91f3464702ff5b3835b1a03cbc0ed01f69b925`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 3.2 MB (3240190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd1d5232a1658cfbf3e897edcf448ab3e9c9694dda8d4e129df83c0bae21f9f`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f11090d6fc460a6639be04bf456fdf26e7979fabbf746cb590b589c795b830`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 2.2 MB (2168128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e8c9ae606cfbddb9544fb07bf10d7a4e2600a823df49af117309ee6251b7bf`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de2b0e7490b2291144d7194e8e4b0cac11516b3a2ef8ab2ac16ab6188525459`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965f711cfb9fad11eb407963156518aca907c20b366fc82ce6b8e2f723b3e7a2`  
		Last Modified: Fri, 02 Sep 2022 02:25:08 GMT  
		Size: 90.1 MB (90055372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266e60e5c085b8b6e235ee9ae91b1c1f5ef947e67954dd0f4f0a558dfc2494c9`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59293cc4d99570c3db4885611ccf8ea66c1e2b65b4f916819f2a58f666a9423`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7-focal`

```console
$ docker pull mariadb@sha256:182c04ae1957dc0caa04fc993eb922f1d4cbdfc70fed9a0d62a35881962e6c45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:1fbc9536ec90869d61de7f261a7caf5d25770421242cb92a5b7495994ffd3f52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128874652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4492bfbc19572e4e9e1555614ec440d80e85ed8cbd3bdcdfeffe27fbd98b74e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:44:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:44:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:21 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:44:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:44:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:44:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:44:40 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:44:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:44:41 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 03:44:42 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 03:44:42 GMT
ARG MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 03:44:42 GMT
ENV MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 03:44:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 03:44:42 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:45:13 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:45:13 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:45:13 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:45:14 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:45:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:45:14 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:45:14 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4390411700c6ce0bfeddafa32e7e8d865286ec5de202193fb5bda00f6bcc5`  
		Last Modified: Fri, 02 Sep 2022 03:49:42 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566a6a9b01f355c07f2c6781d749b81b1325a88faa60821004f3c7efe01ce4ff`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 5.5 MB (5489012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033be70909e9fe9e290ca2481c848387e78dd78a01db1292cad605ee667f60c8`  
		Last Modified: Fri, 02 Sep 2022 03:49:41 GMT  
		Size: 3.6 MB (3581822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62d5ac9f0ccc53175c445e0dae99e4049b34ffe8d240a50f5d6fa4ce4899dbb`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482b55ad0b73ae0b82ab3e488bc2cde6989966127f70d6339e34b0a6ea93f55c`  
		Last Modified: Fri, 02 Sep 2022 03:49:40 GMT  
		Size: 2.3 MB (2255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5e77b89d07f71009d9c4f9cac33ca4c20ea183a0f4ba99385e41303f52e79`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e579c77c079167ac4cf2b00a4c5f95842fb8bb961458fc24955021f59f105eee`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59833a90b3fdea3c70ff5a43637b5f76944a165a73e96ef48a1e5ddb399fbc24`  
		Last Modified: Fri, 02 Sep 2022 03:49:51 GMT  
		Size: 89.0 MB (88960462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94b681c9a42b7e6014d5d5ae2872b82aee86f8403f3cf1529414f57ce0f5b3f`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690bd4563ef7be4647fa90df0d4903fc7589f7f06af5df469aded76057e88e09`  
		Last Modified: Fri, 02 Sep 2022 03:49:38 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ebe653ef0d86eb70459459deba024a4744134dd1cb7e042c707b0c74fdf12699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126005472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ccde508a2f195c49b96a65f34f85b5d556c9f39d6779b7bb91f0537cd48e327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:28:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:28:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:28:42 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:28:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:28:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:29:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:29:07 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:29:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:29:10 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 05:29:11 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 05:29:12 GMT
ARG MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 05:29:13 GMT
ENV MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 05:29:14 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 05:29:15 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:29:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:29:38 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:29:40 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:29:41 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:29:42 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:29:43 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1387e18688e2e1f398e8eddc71832a86a038b480cdf34faea424e9fba43a879c`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915da50884179341b9a70b1b9262c296afde1518f5febc6187e5acebf95b5270`  
		Last Modified: Fri, 02 Sep 2022 05:35:35 GMT  
		Size: 5.3 MB (5321749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49f9bf1bf526742e12590b754fae559d770ffc321c6bd2e35e2287bd26de8ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 3.4 MB (3367845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05c791accac82f833680e4922c78dd5f0db9e38949eb9442391e17a16aa554b`  
		Last Modified: Fri, 02 Sep 2022 05:35:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a130f4ee234d6425768351aad2f189d02fabd64fbc4886d32167c6553ae5479`  
		Last Modified: Fri, 02 Sep 2022 05:35:34 GMT  
		Size: 2.2 MB (2186066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990908d8220dd9cb55c9da069b932d7cbef9ddc23257fa074f5d4498c05bfba`  
		Last Modified: Fri, 02 Sep 2022 05:35:32 GMT  
		Size: 2.5 KB (2469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f78b4c9ee113fa9b65d4009a271140553fea0d672b114b33d6aa14edc33d2ae`  
		Last Modified: Fri, 02 Sep 2022 05:35:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5088985b5d3cab36c60b6692245368fc2a59c6dd724f9b4518f8f03b27322de2`  
		Last Modified: Fri, 02 Sep 2022 05:35:45 GMT  
		Size: 87.9 MB (87923174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbff1dfc120b4ee7d4c5983038ecc59f81511cc851f13cd4684838c52c4c13c`  
		Last Modified: Fri, 02 Sep 2022 05:35:31 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0309e6b9b27bfd8d2e7331ebcea3866e5aa1d4485397f006b274db8776687340`  
		Last Modified: Fri, 02 Sep 2022 05:35:31 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f91a69470434216dfbecdd7be98bcc278e1673519ff715b549c199549f3d774b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139771204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b88397ea305dda3e5603f4d1f5cc62d6085409faadf0f69df819883e4e48f25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:49:54 GMT
ADD file:eb82827919ea73f9595d7b0b70fe9aa5ff23e16ea6a87f7f9ef4e1905857b789 in / 
# Thu, 01 Sep 2022 23:49:56 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:56:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:57:14 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:14 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:57:32 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:57:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:57:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:57:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:57:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:57:48 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 04:57:49 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 04:57:49 GMT
ARG MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 04:57:49 GMT
ENV MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 04:57:50 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 04:57:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:58:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:58:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:58:51 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:58:51 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:58:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:58:52 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:58:52 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:891f6400ce611ee5975f04ad6d2c68305c76a8628b846df1b1f9ac7c45b1311c`  
		Last Modified: Thu, 01 Sep 2022 23:52:11 GMT  
		Size: 33.3 MB (33295624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da11c4b60a797d7f09eb2b761711eb09e41b7de59aceaf7d7d28f445e1082463`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d463d3305d73e5f8bfc8ba97be7c6ea6d67aca35e3343bf6e0d482c585ddf6f`  
		Last Modified: Fri, 02 Sep 2022 05:06:59 GMT  
		Size: 6.7 MB (6667666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d173de46757f679cd48d69d0bce4b5996ae2ceef07ea8c57078ad379a97d701`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 3.7 MB (3669771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078ccb84a5a5ba1d3fc77f7b65bde36e5ea5fbe50da52d93c88e766e5639352f`  
		Last Modified: Fri, 02 Sep 2022 05:06:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c457604661be0a3fec3e7e212b1cd828fc431ac49b55150fc4827b983b86db`  
		Last Modified: Fri, 02 Sep 2022 05:06:58 GMT  
		Size: 2.6 MB (2550575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3484f82c4a291ff8975345be7af0da4f66b3ed340ed1c5bd2b1c1cfcdc7ead6`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82da8d69fe999cb3782d20c028103ca3217853d613a382fa44172693fd363226`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd8d1fc82c4400d05d6d6ac4f1e7161e9c474ca18e30fbf0d08a391097f2a27`  
		Last Modified: Fri, 02 Sep 2022 05:07:20 GMT  
		Size: 93.6 MB (93572669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95994d7b0f97304e9eeba611de5472538c959c2a056e72845d0e3154bbb75224`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357e4adc4ffc4c8e89dcb8b226aabfe430fbe9b1ab6f0d8bc72dcce9b6b9f5e3`  
		Last Modified: Fri, 02 Sep 2022 05:06:54 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:2342b111be5d497cc004951c8f1aeff55ef5de6f6f010e73354f935e9b45fed5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127896553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5442dc97b6f86206b8c450fa1328deed9d2e85b732956a927fae39ebcd069f82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:13 GMT
ADD file:75a78d9ec31ac5486bdde3e48ebfc534089c5f38f14850243c2ab2e632f0bbe5 in / 
# Fri, 02 Sep 2022 01:03:16 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:20:37 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:20:43 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:43 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:20:52 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:20:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:20:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:20:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:20:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:20:59 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 02:20:59 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 02 Sep 2022 02:20:59 GMT
ARG MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 02:20:59 GMT
ENV MARIADB_VERSION=1:10.7.5+maria~ubu2004
# Fri, 02 Sep 2022 02:20:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
# Fri, 02 Sep 2022 02:21:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:21:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.5/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:21:28 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:21:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:21:28 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:21:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:21:29 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:21:29 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b87ab7b8bb5c2a1f34d9a2e9887fde669c33cea7428fdb048362dfa81eccaa75`  
		Last Modified: Fri, 02 Sep 2022 01:04:49 GMT  
		Size: 27.0 MB (27045282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4074f18b54e21cd0e65811b1690ca103650cccbb8729233dea9b7f319f326e85`  
		Last Modified: Fri, 02 Sep 2022 02:24:57 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcfde2f51ff0ee80f91c71818c78bb17bb5aad9ad1842d539f1fc1fc1600124b`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 5.4 MB (5372683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096750bf78c944bdb3aa044f8a91f3464702ff5b3835b1a03cbc0ed01f69b925`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 3.2 MB (3240190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd1d5232a1658cfbf3e897edcf448ab3e9c9694dda8d4e129df83c0bae21f9f`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f11090d6fc460a6639be04bf456fdf26e7979fabbf746cb590b589c795b830`  
		Last Modified: Fri, 02 Sep 2022 02:24:56 GMT  
		Size: 2.2 MB (2168128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e8c9ae606cfbddb9544fb07bf10d7a4e2600a823df49af117309ee6251b7bf`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de2b0e7490b2291144d7194e8e4b0cac11516b3a2ef8ab2ac16ab6188525459`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965f711cfb9fad11eb407963156518aca907c20b366fc82ce6b8e2f723b3e7a2`  
		Last Modified: Fri, 02 Sep 2022 02:25:08 GMT  
		Size: 90.1 MB (90055372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266e60e5c085b8b6e235ee9ae91b1c1f5ef947e67954dd0f4f0a558dfc2494c9`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59293cc4d99570c3db4885611ccf8ea66c1e2b65b4f916819f2a58f666a9423`  
		Last Modified: Fri, 02 Sep 2022 02:24:55 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.6`

**does not exist** (yet?)

## `mariadb:10.7.6-focal`

**does not exist** (yet?)

## `mariadb:10.8`

```console
$ docker pull mariadb@sha256:c8f817ab07d329fc9ff888fd19b0c5718d177411132c4d7b3e9072a02725f98f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8` - linux; amd64

```console
$ docker pull mariadb@sha256:e61885923b93f8adcad847ea131049439478c4abf8da25b5822b97d843975480
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123922581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06dc201e9dbe1779176955d249b59ca916619ada528b73b7cd5876d7ef3aee3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:41:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:42:07 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:07 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:42:19 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:42:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:42:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:28 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:42:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:43:45 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 03:43:46 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 03:43:46 GMT
ARG MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 03:43:46 GMT
ENV MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 03:43:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 03:43:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:44:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:44:07 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:44:08 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:44:08 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:44:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:44:08 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:44:08 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf944e49ffa85996da499d5d92c328463b711fd3a1672b809e2824a964da9fb`  
		Last Modified: Fri, 02 Sep 2022 03:48:07 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020ff2b6bb0b679bc28ad3ec3d451993a1ef2282c86f87ca148774d73593a1cc`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 3.8 MB (3765427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977397ae9bc646b6dcf2321014794f535cb5a74110c608b1d1c0986ee1eb1424`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.0 MB (1992954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361cf449d40803e89980d56903e81945ce9fa372a686ea76f4a9c7a646a8337`  
		Last Modified: Fri, 02 Sep 2022 03:48:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d26195015760a28953bf9d2ad8603a66f8508da28d9878f972ddf137a5b34d`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.3 MB (2281503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a47dd94359e3cf2394add8b9de63828e53d9d2195aa09d903a5e2143e6a9c`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ada2705a971550ff67d30a9e332e9a5dbbc8dc099a5adf7d695794b8b6a0ef`  
		Last Modified: Fri, 02 Sep 2022 03:49:10 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebe3709ae35710eafcbef8ca764235706ff9bd5e14f904c97d7e2d4971bf9a4`  
		Last Modified: Fri, 02 Sep 2022 03:49:22 GMT  
		Size: 85.4 MB (85441083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ba8ee2a2efe016ad3af6d2aac5abb95e03c1d14e4f743950195a754c048ca8`  
		Last Modified: Fri, 02 Sep 2022 03:49:10 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cd9ed19156443234755fc75b00917545a92063d3cc529a5cbaaf3fc9f963fd`  
		Last Modified: Fri, 02 Sep 2022 03:49:10 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:779dfa10364555f4ed9cf875b4769b0902f32a791672de28ef64d04931bd064a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102539272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1fcd550a2404d9a576d4d5bdf81caeb71175f4f4b25a92744ab1167890f2e04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:25:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:26:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:01 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:26:17 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:26:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:26:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:26 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:26:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:27:54 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 05:27:55 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 05:27:56 GMT
ARG MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 05:27:57 GMT
ENV MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 05:27:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 05:27:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:28:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:28:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:28:22 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:28:23 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:28:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:28:24 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:28:25 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0749552ddbb27b679c4c784814a6bc9cff4dea894b4c50ff08211ac33d7141`  
		Last Modified: Fri, 02 Sep 2022 05:33:56 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f3be11a3a90d15ce271dbf8b58dc49944d979b4199b6a9810b17688f071274`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 3.6 MB (3593224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c93d9284a3d0f05825c9fdc3591a7d7d3ae34f1ae103b4ff077a235d40e0f`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 1.9 MB (1898967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232f4136dd4f7f7c1b1de60c1ce430dfdb5d873cdc0e8cf41ac08e1ece7077c2`  
		Last Modified: Fri, 02 Sep 2022 05:33:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ccd89de31befb378b3fd447ebd5efc4fc67e5969c98f28f3df064a191ec01`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 2.2 MB (2194638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea239af7d9b117acb387a6885623fe9b3dd8df83c1e1cd42c1e418f41e14ef3f`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f520cc772a5c018782a3b2d2aeb7864bc30b903639598d30edf78b5b76a1f0d`  
		Last Modified: Fri, 02 Sep 2022 05:35:03 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299de8f6d1d6b7b6de7279d8d9187feeebfe64c813ecf32f696fec7abe806ba9`  
		Last Modified: Fri, 02 Sep 2022 05:35:13 GMT  
		Size: 66.5 MB (66456271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7db3c4ba006f242df89d271d46ebca451ebc0b2ad0f4bfa410a65191c16eab7`  
		Last Modified: Fri, 02 Sep 2022 05:35:03 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d73cf9a145453a258afffbe7013fbf37718e9ac3e4bf5244f0686e7b1962a5`  
		Last Modified: Fri, 02 Sep 2022 05:35:03 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8523bffc7be281d51bf230c4291bcdc1f4a7182e27dc37f743fc3f4047dd58f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116902283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19f2a95d562371f72fbd785a81cce9f50277407823ffd4a882392bb0157afd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:52:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:53:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:53:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:53:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:53:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:55:56 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 04:55:57 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 04:55:57 GMT
ARG MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 04:55:57 GMT
ENV MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 04:55:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 04:55:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:56:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:56:42 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:56:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:56:43 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:56:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:56:43 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:56:43 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55324944c013f5e152ef0fad27126a86f0a45cfff228ed5d376984c8bcb18dbc`  
		Last Modified: Fri, 02 Sep 2022 05:04:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc5813595f57876629a096fc5630c832e5d23f1a6f8c52b86f94b395dd72973`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 4.5 MB (4503005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53136ad37739b4c4b6d5c9c41623f06a89e1c954299e6487b758572c2129b6`  
		Last Modified: Fri, 02 Sep 2022 05:04:41 GMT  
		Size: 1.9 MB (1922006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e9deaa9bc92d6868ca60db4ace55d593c6da8f7dd776648377d6df75bbcdb2`  
		Last Modified: Fri, 02 Sep 2022 05:04:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88549712edded06fae8bfa5c56fae89c47664fc83e5b4a957c2c2764649ebff`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 2.4 MB (2389323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a4751f2b2dee4c43d237fe7b4ce6e1273b2374fcce6496c681cb525e8d26c1`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7469ecdd541aa59064d462ee163843b0a640bdd11b50a89676bbbcea679905`  
		Last Modified: Fri, 02 Sep 2022 05:06:15 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c04e2951524b246e2e15a9db44ba5ab5c98f1cc0051aa98ec4289ffd26906d`  
		Last Modified: Fri, 02 Sep 2022 05:06:34 GMT  
		Size: 72.4 MB (72351846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ae7e32ee742b2f96fd3fc6e8802351ba4d2630dd1a198fffb059f203f01bf5`  
		Last Modified: Fri, 02 Sep 2022 05:06:15 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342575868d0c1b171945591fca4cca74b444347e921c956f56893c55af45ae1f`  
		Last Modified: Fri, 02 Sep 2022 05:06:15 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8` - linux; s390x

```console
$ docker pull mariadb@sha256:d92772fee81e924e9611bd74e001226e03ff5a2fd7df96fa1f37196326329f8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105038401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fb92a97724a0b1dbbd7483b82091847174d9fd86bf266e69e57303cafdb8194`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:18:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:18:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:18:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:18:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:32 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:18:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:20:00 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 02:20:00 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 02:20:00 GMT
ARG MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 02:20:00 GMT
ENV MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 02:20:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 02:20:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:20:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:20:28 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:20:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:20:28 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:20:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:20:28 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:20:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a83a742f8905e65d86bab1137abea13cf130c3c52de601dd27fc4c4188ad7`  
		Last Modified: Fri, 02 Sep 2022 02:23:46 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0074f95048477359d16a331130ff329c74b549bcc5d7a97cd5559fcfe9c7464`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 3.7 MB (3674479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792e98156ec6717f9a09ef69964b1441fc52ea8407babf26638a445cfbca24a7`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.0 MB (1956114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f52d5f8a1d48c335871d777bb6305d30ca6e0d35472d729f97839e5118e1ed`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b51775573dc421f5d01c30c0385676817ad4cd3ed88f8c69fdfe498f57a5b39`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.2 MB (2200620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c5f2dd2c4f8a5fcba9a6bd048360e2483d370947a8e8499b83147d0878d31d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5012d1a1c1703c97e125a86d1bf73a90addc79459355a470e0b322841fee12e`  
		Last Modified: Fri, 02 Sep 2022 02:24:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195f55507ba189300f9e763f1822fa3d26ddad1bfd94eb126d4ee26c239e0992`  
		Last Modified: Fri, 02 Sep 2022 02:24:44 GMT  
		Size: 68.5 MB (68549111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b20b7191a0224ec8e27eaf4a78cc1badca51853200d4c6f0e01a7c25edca63`  
		Last Modified: Fri, 02 Sep 2022 02:24:34 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b23bb246a7bf3f64fe4ac85fb341392551564d6f2c54a914ac263f125c44701`  
		Last Modified: Fri, 02 Sep 2022 02:24:35 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8-jammy`

```console
$ docker pull mariadb@sha256:c8f817ab07d329fc9ff888fd19b0c5718d177411132c4d7b3e9072a02725f98f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:e61885923b93f8adcad847ea131049439478c4abf8da25b5822b97d843975480
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123922581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06dc201e9dbe1779176955d249b59ca916619ada528b73b7cd5876d7ef3aee3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:41:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:42:07 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:07 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:42:19 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:42:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:42:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:28 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:42:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:43:45 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 03:43:46 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 03:43:46 GMT
ARG MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 03:43:46 GMT
ENV MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 03:43:46 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 03:43:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:44:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:44:07 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:44:08 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:44:08 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:44:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:44:08 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:44:08 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf944e49ffa85996da499d5d92c328463b711fd3a1672b809e2824a964da9fb`  
		Last Modified: Fri, 02 Sep 2022 03:48:07 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020ff2b6bb0b679bc28ad3ec3d451993a1ef2282c86f87ca148774d73593a1cc`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 3.8 MB (3765427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977397ae9bc646b6dcf2321014794f535cb5a74110c608b1d1c0986ee1eb1424`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.0 MB (1992954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361cf449d40803e89980d56903e81945ce9fa372a686ea76f4a9c7a646a8337`  
		Last Modified: Fri, 02 Sep 2022 03:48:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d26195015760a28953bf9d2ad8603a66f8508da28d9878f972ddf137a5b34d`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.3 MB (2281503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a47dd94359e3cf2394add8b9de63828e53d9d2195aa09d903a5e2143e6a9c`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ada2705a971550ff67d30a9e332e9a5dbbc8dc099a5adf7d695794b8b6a0ef`  
		Last Modified: Fri, 02 Sep 2022 03:49:10 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebe3709ae35710eafcbef8ca764235706ff9bd5e14f904c97d7e2d4971bf9a4`  
		Last Modified: Fri, 02 Sep 2022 03:49:22 GMT  
		Size: 85.4 MB (85441083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ba8ee2a2efe016ad3af6d2aac5abb95e03c1d14e4f743950195a754c048ca8`  
		Last Modified: Fri, 02 Sep 2022 03:49:10 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cd9ed19156443234755fc75b00917545a92063d3cc529a5cbaaf3fc9f963fd`  
		Last Modified: Fri, 02 Sep 2022 03:49:10 GMT  
		Size: 6.7 KB (6698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:779dfa10364555f4ed9cf875b4769b0902f32a791672de28ef64d04931bd064a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102539272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1fcd550a2404d9a576d4d5bdf81caeb71175f4f4b25a92744ab1167890f2e04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:25:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:26:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:01 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:26:17 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:26:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:26:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:26 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:26:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:27:54 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 05:27:55 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 05:27:56 GMT
ARG MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 05:27:57 GMT
ENV MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 05:27:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 05:27:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:28:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:28:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:28:22 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:28:23 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:28:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:28:24 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:28:25 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0749552ddbb27b679c4c784814a6bc9cff4dea894b4c50ff08211ac33d7141`  
		Last Modified: Fri, 02 Sep 2022 05:33:56 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f3be11a3a90d15ce271dbf8b58dc49944d979b4199b6a9810b17688f071274`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 3.6 MB (3593224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c93d9284a3d0f05825c9fdc3591a7d7d3ae34f1ae103b4ff077a235d40e0f`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 1.9 MB (1898967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232f4136dd4f7f7c1b1de60c1ce430dfdb5d873cdc0e8cf41ac08e1ece7077c2`  
		Last Modified: Fri, 02 Sep 2022 05:33:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ccd89de31befb378b3fd447ebd5efc4fc67e5969c98f28f3df064a191ec01`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 2.2 MB (2194638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea239af7d9b117acb387a6885623fe9b3dd8df83c1e1cd42c1e418f41e14ef3f`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f520cc772a5c018782a3b2d2aeb7864bc30b903639598d30edf78b5b76a1f0d`  
		Last Modified: Fri, 02 Sep 2022 05:35:03 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299de8f6d1d6b7b6de7279d8d9187feeebfe64c813ecf32f696fec7abe806ba9`  
		Last Modified: Fri, 02 Sep 2022 05:35:13 GMT  
		Size: 66.5 MB (66456271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7db3c4ba006f242df89d271d46ebca451ebc0b2ad0f4bfa410a65191c16eab7`  
		Last Modified: Fri, 02 Sep 2022 05:35:03 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d73cf9a145453a258afffbe7013fbf37718e9ac3e4bf5244f0686e7b1962a5`  
		Last Modified: Fri, 02 Sep 2022 05:35:03 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8523bffc7be281d51bf230c4291bcdc1f4a7182e27dc37f743fc3f4047dd58f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116902283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19f2a95d562371f72fbd785a81cce9f50277407823ffd4a882392bb0157afd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:52:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:53:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:53:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:53:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:53:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:55:56 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 04:55:57 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 04:55:57 GMT
ARG MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 04:55:57 GMT
ENV MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 04:55:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 04:55:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:56:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:56:42 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:56:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:56:43 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:56:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:56:43 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:56:43 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55324944c013f5e152ef0fad27126a86f0a45cfff228ed5d376984c8bcb18dbc`  
		Last Modified: Fri, 02 Sep 2022 05:04:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc5813595f57876629a096fc5630c832e5d23f1a6f8c52b86f94b395dd72973`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 4.5 MB (4503005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53136ad37739b4c4b6d5c9c41623f06a89e1c954299e6487b758572c2129b6`  
		Last Modified: Fri, 02 Sep 2022 05:04:41 GMT  
		Size: 1.9 MB (1922006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e9deaa9bc92d6868ca60db4ace55d593c6da8f7dd776648377d6df75bbcdb2`  
		Last Modified: Fri, 02 Sep 2022 05:04:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88549712edded06fae8bfa5c56fae89c47664fc83e5b4a957c2c2764649ebff`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 2.4 MB (2389323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a4751f2b2dee4c43d237fe7b4ce6e1273b2374fcce6496c681cb525e8d26c1`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7469ecdd541aa59064d462ee163843b0a640bdd11b50a89676bbbcea679905`  
		Last Modified: Fri, 02 Sep 2022 05:06:15 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c04e2951524b246e2e15a9db44ba5ab5c98f1cc0051aa98ec4289ffd26906d`  
		Last Modified: Fri, 02 Sep 2022 05:06:34 GMT  
		Size: 72.4 MB (72351846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ae7e32ee742b2f96fd3fc6e8802351ba4d2630dd1a198fffb059f203f01bf5`  
		Last Modified: Fri, 02 Sep 2022 05:06:15 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342575868d0c1b171945591fca4cca74b444347e921c956f56893c55af45ae1f`  
		Last Modified: Fri, 02 Sep 2022 05:06:15 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:d92772fee81e924e9611bd74e001226e03ff5a2fd7df96fa1f37196326329f8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105038401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fb92a97724a0b1dbbd7483b82091847174d9fd86bf266e69e57303cafdb8194`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:18:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:18:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:18:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:18:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:32 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:18:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:20:00 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 02:20:00 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 02 Sep 2022 02:20:00 GMT
ARG MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 02:20:00 GMT
ENV MARIADB_VERSION=1:10.8.4+maria~ubu2204
# Fri, 02 Sep 2022 02:20:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 02:20:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:20:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.4/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:20:28 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:20:28 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:20:28 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:20:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:20:28 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:20:28 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a83a742f8905e65d86bab1137abea13cf130c3c52de601dd27fc4c4188ad7`  
		Last Modified: Fri, 02 Sep 2022 02:23:46 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0074f95048477359d16a331130ff329c74b549bcc5d7a97cd5559fcfe9c7464`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 3.7 MB (3674479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792e98156ec6717f9a09ef69964b1441fc52ea8407babf26638a445cfbca24a7`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.0 MB (1956114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f52d5f8a1d48c335871d777bb6305d30ca6e0d35472d729f97839e5118e1ed`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b51775573dc421f5d01c30c0385676817ad4cd3ed88f8c69fdfe498f57a5b39`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.2 MB (2200620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c5f2dd2c4f8a5fcba9a6bd048360e2483d370947a8e8499b83147d0878d31d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5012d1a1c1703c97e125a86d1bf73a90addc79459355a470e0b322841fee12e`  
		Last Modified: Fri, 02 Sep 2022 02:24:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195f55507ba189300f9e763f1822fa3d26ddad1bfd94eb126d4ee26c239e0992`  
		Last Modified: Fri, 02 Sep 2022 02:24:44 GMT  
		Size: 68.5 MB (68549111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b20b7191a0224ec8e27eaf4a78cc1badca51853200d4c6f0e01a7c25edca63`  
		Last Modified: Fri, 02 Sep 2022 02:24:34 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b23bb246a7bf3f64fe4ac85fb341392551564d6f2c54a914ac263f125c44701`  
		Last Modified: Fri, 02 Sep 2022 02:24:35 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.5`

**does not exist** (yet?)

## `mariadb:10.8.5-jammy`

**does not exist** (yet?)

## `mariadb:10.9`

```console
$ docker pull mariadb@sha256:ca04948aca834499f728692520eff82917de1d768b47751ba4dd0fc5f261c8e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.9` - linux; amd64

```console
$ docker pull mariadb@sha256:7e613e248abdf4604776d6ace8eba9998b61b44f3c6cfd7121939c2fc3f1a7d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (124013572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c284e5e829612878511aa9fc0c383708c5a68f2167fa77a515bc2e4b2a35bf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:41:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:42:07 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:07 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:42:19 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:42:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:42:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:28 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:42:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:43:20 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 03:43:20 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 03:43:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 03:43:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:43:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:43:42 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:43:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:43:42 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:43:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:43:42 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:43:42 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf944e49ffa85996da499d5d92c328463b711fd3a1672b809e2824a964da9fb`  
		Last Modified: Fri, 02 Sep 2022 03:48:07 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020ff2b6bb0b679bc28ad3ec3d451993a1ef2282c86f87ca148774d73593a1cc`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 3.8 MB (3765427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977397ae9bc646b6dcf2321014794f535cb5a74110c608b1d1c0986ee1eb1424`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.0 MB (1992954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361cf449d40803e89980d56903e81945ce9fa372a686ea76f4a9c7a646a8337`  
		Last Modified: Fri, 02 Sep 2022 03:48:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d26195015760a28953bf9d2ad8603a66f8508da28d9878f972ddf137a5b34d`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.3 MB (2281503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a47dd94359e3cf2394add8b9de63828e53d9d2195aa09d903a5e2143e6a9c`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4132d19a681ab040d5709b46847ab664104c652bf06ef4a02a0b81d909b57979`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701416dc7e3dc54762a773a56a3140235bcd7c031e29891270df8d8156ac566`  
		Last Modified: Fri, 02 Sep 2022 03:48:43 GMT  
		Size: 85.5 MB (85532069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e314a661679bf4986516e7a5521b2ced57b07332a1bee31fdc83146474893a4`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efce0fc30145a5908ba6bf7fd4c4b33fd9d54e593bff96c19842055866bee692`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b27d6a2d4a982fb67a724692fd8edd42e1bfe20dd6d2a73b2fb0eb16c27ad7d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102629742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ecf4f48e2978426dbcc04c56a89f22f76339b1ac791bc5baf9052cb4b99890`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:25:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:26:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:01 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:26:17 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:26:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:26:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:26 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:26:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:27:16 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 05:27:17 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 05:27:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 05:27:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:27:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:27:41 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:27:43 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:27:44 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:27:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:27:45 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:27:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0749552ddbb27b679c4c784814a6bc9cff4dea894b4c50ff08211ac33d7141`  
		Last Modified: Fri, 02 Sep 2022 05:33:56 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f3be11a3a90d15ce271dbf8b58dc49944d979b4199b6a9810b17688f071274`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 3.6 MB (3593224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c93d9284a3d0f05825c9fdc3591a7d7d3ae34f1ae103b4ff077a235d40e0f`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 1.9 MB (1898967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232f4136dd4f7f7c1b1de60c1ce430dfdb5d873cdc0e8cf41ac08e1ece7077c2`  
		Last Modified: Fri, 02 Sep 2022 05:33:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ccd89de31befb378b3fd447ebd5efc4fc67e5969c98f28f3df064a191ec01`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 2.2 MB (2194638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea239af7d9b117acb387a6885623fe9b3dd8df83c1e1cd42c1e418f41e14ef3f`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b306f626891fb340fada4bee82bca7350cea48d4b7d9417c8e16d70b607625`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f977adfc1f0b0065e437818c0d56a7fbea2e66cc2c20fcffb22eb2c726a9d32a`  
		Last Modified: Fri, 02 Sep 2022 05:34:31 GMT  
		Size: 66.5 MB (66546741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c63d31682849e6f78d30d0f7433c748e8581611ada5daf827d30785d2918fd2`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d7766f9fa328aaecc5edea92a920254bf6c7d03d0155d4bbc0b2fced86eded`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9` - linux; ppc64le

```console
$ docker pull mariadb@sha256:efc520a5969afe22458ec081d2591e6c530af4bdc71f4cb66a755645faff34a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117027115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6dac49f7b083a7406a56adae7166704f912cc7c1676485947393adb8952ad3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:52:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:53:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:53:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:53:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:53:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:55:03 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 04:55:03 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 04:55:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 04:55:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:55:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:55:46 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:55:47 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:55:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:55:47 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:55:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55324944c013f5e152ef0fad27126a86f0a45cfff228ed5d376984c8bcb18dbc`  
		Last Modified: Fri, 02 Sep 2022 05:04:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc5813595f57876629a096fc5630c832e5d23f1a6f8c52b86f94b395dd72973`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 4.5 MB (4503005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53136ad37739b4c4b6d5c9c41623f06a89e1c954299e6487b758572c2129b6`  
		Last Modified: Fri, 02 Sep 2022 05:04:41 GMT  
		Size: 1.9 MB (1922006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e9deaa9bc92d6868ca60db4ace55d593c6da8f7dd776648377d6df75bbcdb2`  
		Last Modified: Fri, 02 Sep 2022 05:04:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88549712edded06fae8bfa5c56fae89c47664fc83e5b4a957c2c2764649ebff`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 2.4 MB (2389323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a4751f2b2dee4c43d237fe7b4ce6e1273b2374fcce6496c681cb525e8d26c1`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105f46c3085029c3a9f300164ffa8751b280f2ac336393e07ca596d6f1475929`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997e1406175b8de4067c34e21e14c3e22d70e65d699abfb60d8dfd481f2ef6be`  
		Last Modified: Fri, 02 Sep 2022 05:05:37 GMT  
		Size: 72.5 MB (72476684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66144ed93c4b6752c2c1059ed5ab44b752cc2444db93c44745a7c41c644be878`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39015c23b5aa07433c0d517088d4fb65a3b8e8d59ae9d235e1edc1661971bfb1`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9` - linux; s390x

```console
$ docker pull mariadb@sha256:6f4ec55b4c6a791b54f9a18f4f744b8cd3526fdfd9be7d238370ce93fecc9b8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105124376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66ac2973c068da3f5b39dcb1713654443f0ccd0cf7e315dab0de330e787d8c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:18:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:18:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:18:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:18:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:32 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:18:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:19:29 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 02:19:29 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 02:19:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 02:19:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:19:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:19:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:19:50 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:19:50 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:19:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:19:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a83a742f8905e65d86bab1137abea13cf130c3c52de601dd27fc4c4188ad7`  
		Last Modified: Fri, 02 Sep 2022 02:23:46 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0074f95048477359d16a331130ff329c74b549bcc5d7a97cd5559fcfe9c7464`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 3.7 MB (3674479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792e98156ec6717f9a09ef69964b1441fc52ea8407babf26638a445cfbca24a7`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.0 MB (1956114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f52d5f8a1d48c335871d777bb6305d30ca6e0d35472d729f97839e5118e1ed`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b51775573dc421f5d01c30c0385676817ad4cd3ed88f8c69fdfe498f57a5b39`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.2 MB (2200620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c5f2dd2c4f8a5fcba9a6bd048360e2483d370947a8e8499b83147d0878d31d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4005206c1b7f520588d957202113c82375fa4ac4b297a19265f0fc8408f6a082`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56247b961b3a212d383dc7a9d8148dfccfbcc139deb5f0c7718cac610d4707e2`  
		Last Modified: Fri, 02 Sep 2022 02:24:16 GMT  
		Size: 68.6 MB (68635084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a147a6bdb02d471ccfe5c14f82e463b195033f170feccb02e1db2bb128b051a5`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318ac1fb7ba29d893d6d9bb95215957152ae3ea476a5b7325b44532655c7c37d`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9-jammy`

```console
$ docker pull mariadb@sha256:ca04948aca834499f728692520eff82917de1d768b47751ba4dd0fc5f261c8e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.9-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:7e613e248abdf4604776d6ace8eba9998b61b44f3c6cfd7121939c2fc3f1a7d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (124013572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c284e5e829612878511aa9fc0c383708c5a68f2167fa77a515bc2e4b2a35bf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:41:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:42:07 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:07 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:42:19 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:42:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:42:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:28 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:42:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:43:20 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 03:43:20 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 03:43:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 03:43:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:43:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:43:42 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:43:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:43:42 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:43:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:43:42 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:43:42 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf944e49ffa85996da499d5d92c328463b711fd3a1672b809e2824a964da9fb`  
		Last Modified: Fri, 02 Sep 2022 03:48:07 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020ff2b6bb0b679bc28ad3ec3d451993a1ef2282c86f87ca148774d73593a1cc`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 3.8 MB (3765427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977397ae9bc646b6dcf2321014794f535cb5a74110c608b1d1c0986ee1eb1424`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.0 MB (1992954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361cf449d40803e89980d56903e81945ce9fa372a686ea76f4a9c7a646a8337`  
		Last Modified: Fri, 02 Sep 2022 03:48:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d26195015760a28953bf9d2ad8603a66f8508da28d9878f972ddf137a5b34d`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.3 MB (2281503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a47dd94359e3cf2394add8b9de63828e53d9d2195aa09d903a5e2143e6a9c`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4132d19a681ab040d5709b46847ab664104c652bf06ef4a02a0b81d909b57979`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701416dc7e3dc54762a773a56a3140235bcd7c031e29891270df8d8156ac566`  
		Last Modified: Fri, 02 Sep 2022 03:48:43 GMT  
		Size: 85.5 MB (85532069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e314a661679bf4986516e7a5521b2ced57b07332a1bee31fdc83146474893a4`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efce0fc30145a5908ba6bf7fd4c4b33fd9d54e593bff96c19842055866bee692`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b27d6a2d4a982fb67a724692fd8edd42e1bfe20dd6d2a73b2fb0eb16c27ad7d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102629742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ecf4f48e2978426dbcc04c56a89f22f76339b1ac791bc5baf9052cb4b99890`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:25:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:26:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:01 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:26:17 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:26:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:26:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:26 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:26:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:27:16 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 05:27:17 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 05:27:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 05:27:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:27:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:27:41 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:27:43 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:27:44 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:27:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:27:45 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:27:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0749552ddbb27b679c4c784814a6bc9cff4dea894b4c50ff08211ac33d7141`  
		Last Modified: Fri, 02 Sep 2022 05:33:56 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f3be11a3a90d15ce271dbf8b58dc49944d979b4199b6a9810b17688f071274`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 3.6 MB (3593224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c93d9284a3d0f05825c9fdc3591a7d7d3ae34f1ae103b4ff077a235d40e0f`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 1.9 MB (1898967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232f4136dd4f7f7c1b1de60c1ce430dfdb5d873cdc0e8cf41ac08e1ece7077c2`  
		Last Modified: Fri, 02 Sep 2022 05:33:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ccd89de31befb378b3fd447ebd5efc4fc67e5969c98f28f3df064a191ec01`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 2.2 MB (2194638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea239af7d9b117acb387a6885623fe9b3dd8df83c1e1cd42c1e418f41e14ef3f`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b306f626891fb340fada4bee82bca7350cea48d4b7d9417c8e16d70b607625`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f977adfc1f0b0065e437818c0d56a7fbea2e66cc2c20fcffb22eb2c726a9d32a`  
		Last Modified: Fri, 02 Sep 2022 05:34:31 GMT  
		Size: 66.5 MB (66546741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c63d31682849e6f78d30d0f7433c748e8581611ada5daf827d30785d2918fd2`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d7766f9fa328aaecc5edea92a920254bf6c7d03d0155d4bbc0b2fced86eded`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:efc520a5969afe22458ec081d2591e6c530af4bdc71f4cb66a755645faff34a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117027115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6dac49f7b083a7406a56adae7166704f912cc7c1676485947393adb8952ad3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:52:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:53:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:53:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:53:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:53:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:55:03 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 04:55:03 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 04:55:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 04:55:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:55:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:55:46 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:55:47 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:55:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:55:47 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:55:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55324944c013f5e152ef0fad27126a86f0a45cfff228ed5d376984c8bcb18dbc`  
		Last Modified: Fri, 02 Sep 2022 05:04:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc5813595f57876629a096fc5630c832e5d23f1a6f8c52b86f94b395dd72973`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 4.5 MB (4503005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53136ad37739b4c4b6d5c9c41623f06a89e1c954299e6487b758572c2129b6`  
		Last Modified: Fri, 02 Sep 2022 05:04:41 GMT  
		Size: 1.9 MB (1922006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e9deaa9bc92d6868ca60db4ace55d593c6da8f7dd776648377d6df75bbcdb2`  
		Last Modified: Fri, 02 Sep 2022 05:04:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88549712edded06fae8bfa5c56fae89c47664fc83e5b4a957c2c2764649ebff`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 2.4 MB (2389323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a4751f2b2dee4c43d237fe7b4ce6e1273b2374fcce6496c681cb525e8d26c1`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105f46c3085029c3a9f300164ffa8751b280f2ac336393e07ca596d6f1475929`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997e1406175b8de4067c34e21e14c3e22d70e65d699abfb60d8dfd481f2ef6be`  
		Last Modified: Fri, 02 Sep 2022 05:05:37 GMT  
		Size: 72.5 MB (72476684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66144ed93c4b6752c2c1059ed5ab44b752cc2444db93c44745a7c41c644be878`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39015c23b5aa07433c0d517088d4fb65a3b8e8d59ae9d235e1edc1661971bfb1`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.9-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:6f4ec55b4c6a791b54f9a18f4f744b8cd3526fdfd9be7d238370ce93fecc9b8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105124376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66ac2973c068da3f5b39dcb1713654443f0ccd0cf7e315dab0de330e787d8c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:18:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:18:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:18:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:18:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:32 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:18:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:19:29 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 02:19:29 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 02:19:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 02:19:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:19:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:19:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:19:50 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:19:50 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:19:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:19:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a83a742f8905e65d86bab1137abea13cf130c3c52de601dd27fc4c4188ad7`  
		Last Modified: Fri, 02 Sep 2022 02:23:46 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0074f95048477359d16a331130ff329c74b549bcc5d7a97cd5559fcfe9c7464`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 3.7 MB (3674479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792e98156ec6717f9a09ef69964b1441fc52ea8407babf26638a445cfbca24a7`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.0 MB (1956114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f52d5f8a1d48c335871d777bb6305d30ca6e0d35472d729f97839e5118e1ed`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b51775573dc421f5d01c30c0385676817ad4cd3ed88f8c69fdfe498f57a5b39`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.2 MB (2200620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c5f2dd2c4f8a5fcba9a6bd048360e2483d370947a8e8499b83147d0878d31d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4005206c1b7f520588d957202113c82375fa4ac4b297a19265f0fc8408f6a082`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56247b961b3a212d383dc7a9d8148dfccfbcc139deb5f0c7718cac610d4707e2`  
		Last Modified: Fri, 02 Sep 2022 02:24:16 GMT  
		Size: 68.6 MB (68635084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a147a6bdb02d471ccfe5c14f82e463b195033f170feccb02e1db2bb128b051a5`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318ac1fb7ba29d893d6d9bb95215957152ae3ea476a5b7325b44532655c7c37d`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.9.3`

**does not exist** (yet?)

## `mariadb:10.9.3-jammy`

**does not exist** (yet?)

## `mariadb:jammy`

```console
$ docker pull mariadb@sha256:ca04948aca834499f728692520eff82917de1d768b47751ba4dd0fc5f261c8e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:7e613e248abdf4604776d6ace8eba9998b61b44f3c6cfd7121939c2fc3f1a7d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (124013572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c284e5e829612878511aa9fc0c383708c5a68f2167fa77a515bc2e4b2a35bf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:41:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:42:07 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:07 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:42:19 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:42:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:42:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:28 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:42:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:43:20 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 03:43:20 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 03:43:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 03:43:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:43:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:43:42 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:43:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:43:42 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:43:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:43:42 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:43:42 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf944e49ffa85996da499d5d92c328463b711fd3a1672b809e2824a964da9fb`  
		Last Modified: Fri, 02 Sep 2022 03:48:07 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020ff2b6bb0b679bc28ad3ec3d451993a1ef2282c86f87ca148774d73593a1cc`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 3.8 MB (3765427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977397ae9bc646b6dcf2321014794f535cb5a74110c608b1d1c0986ee1eb1424`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.0 MB (1992954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361cf449d40803e89980d56903e81945ce9fa372a686ea76f4a9c7a646a8337`  
		Last Modified: Fri, 02 Sep 2022 03:48:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d26195015760a28953bf9d2ad8603a66f8508da28d9878f972ddf137a5b34d`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.3 MB (2281503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a47dd94359e3cf2394add8b9de63828e53d9d2195aa09d903a5e2143e6a9c`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4132d19a681ab040d5709b46847ab664104c652bf06ef4a02a0b81d909b57979`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701416dc7e3dc54762a773a56a3140235bcd7c031e29891270df8d8156ac566`  
		Last Modified: Fri, 02 Sep 2022 03:48:43 GMT  
		Size: 85.5 MB (85532069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e314a661679bf4986516e7a5521b2ced57b07332a1bee31fdc83146474893a4`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efce0fc30145a5908ba6bf7fd4c4b33fd9d54e593bff96c19842055866bee692`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b27d6a2d4a982fb67a724692fd8edd42e1bfe20dd6d2a73b2fb0eb16c27ad7d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102629742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ecf4f48e2978426dbcc04c56a89f22f76339b1ac791bc5baf9052cb4b99890`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:25:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:26:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:01 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:26:17 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:26:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:26:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:26 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:26:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:27:16 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 05:27:17 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 05:27:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 05:27:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:27:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:27:41 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:27:43 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:27:44 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:27:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:27:45 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:27:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0749552ddbb27b679c4c784814a6bc9cff4dea894b4c50ff08211ac33d7141`  
		Last Modified: Fri, 02 Sep 2022 05:33:56 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f3be11a3a90d15ce271dbf8b58dc49944d979b4199b6a9810b17688f071274`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 3.6 MB (3593224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c93d9284a3d0f05825c9fdc3591a7d7d3ae34f1ae103b4ff077a235d40e0f`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 1.9 MB (1898967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232f4136dd4f7f7c1b1de60c1ce430dfdb5d873cdc0e8cf41ac08e1ece7077c2`  
		Last Modified: Fri, 02 Sep 2022 05:33:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ccd89de31befb378b3fd447ebd5efc4fc67e5969c98f28f3df064a191ec01`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 2.2 MB (2194638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea239af7d9b117acb387a6885623fe9b3dd8df83c1e1cd42c1e418f41e14ef3f`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b306f626891fb340fada4bee82bca7350cea48d4b7d9417c8e16d70b607625`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f977adfc1f0b0065e437818c0d56a7fbea2e66cc2c20fcffb22eb2c726a9d32a`  
		Last Modified: Fri, 02 Sep 2022 05:34:31 GMT  
		Size: 66.5 MB (66546741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c63d31682849e6f78d30d0f7433c748e8581611ada5daf827d30785d2918fd2`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d7766f9fa328aaecc5edea92a920254bf6c7d03d0155d4bbc0b2fced86eded`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:efc520a5969afe22458ec081d2591e6c530af4bdc71f4cb66a755645faff34a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117027115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6dac49f7b083a7406a56adae7166704f912cc7c1676485947393adb8952ad3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:52:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:53:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:53:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:53:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:53:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:55:03 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 04:55:03 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 04:55:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 04:55:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:55:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:55:46 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:55:47 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:55:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:55:47 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:55:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55324944c013f5e152ef0fad27126a86f0a45cfff228ed5d376984c8bcb18dbc`  
		Last Modified: Fri, 02 Sep 2022 05:04:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc5813595f57876629a096fc5630c832e5d23f1a6f8c52b86f94b395dd72973`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 4.5 MB (4503005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53136ad37739b4c4b6d5c9c41623f06a89e1c954299e6487b758572c2129b6`  
		Last Modified: Fri, 02 Sep 2022 05:04:41 GMT  
		Size: 1.9 MB (1922006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e9deaa9bc92d6868ca60db4ace55d593c6da8f7dd776648377d6df75bbcdb2`  
		Last Modified: Fri, 02 Sep 2022 05:04:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88549712edded06fae8bfa5c56fae89c47664fc83e5b4a957c2c2764649ebff`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 2.4 MB (2389323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a4751f2b2dee4c43d237fe7b4ce6e1273b2374fcce6496c681cb525e8d26c1`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105f46c3085029c3a9f300164ffa8751b280f2ac336393e07ca596d6f1475929`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997e1406175b8de4067c34e21e14c3e22d70e65d699abfb60d8dfd481f2ef6be`  
		Last Modified: Fri, 02 Sep 2022 05:05:37 GMT  
		Size: 72.5 MB (72476684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66144ed93c4b6752c2c1059ed5ab44b752cc2444db93c44745a7c41c644be878`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39015c23b5aa07433c0d517088d4fb65a3b8e8d59ae9d235e1edc1661971bfb1`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:6f4ec55b4c6a791b54f9a18f4f744b8cd3526fdfd9be7d238370ce93fecc9b8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105124376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66ac2973c068da3f5b39dcb1713654443f0ccd0cf7e315dab0de330e787d8c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:18:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:18:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:18:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:18:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:32 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:18:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:19:29 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 02:19:29 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 02:19:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 02:19:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:19:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:19:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:19:50 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:19:50 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:19:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:19:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a83a742f8905e65d86bab1137abea13cf130c3c52de601dd27fc4c4188ad7`  
		Last Modified: Fri, 02 Sep 2022 02:23:46 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0074f95048477359d16a331130ff329c74b549bcc5d7a97cd5559fcfe9c7464`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 3.7 MB (3674479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792e98156ec6717f9a09ef69964b1441fc52ea8407babf26638a445cfbca24a7`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.0 MB (1956114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f52d5f8a1d48c335871d777bb6305d30ca6e0d35472d729f97839e5118e1ed`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b51775573dc421f5d01c30c0385676817ad4cd3ed88f8c69fdfe498f57a5b39`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.2 MB (2200620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c5f2dd2c4f8a5fcba9a6bd048360e2483d370947a8e8499b83147d0878d31d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4005206c1b7f520588d957202113c82375fa4ac4b297a19265f0fc8408f6a082`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56247b961b3a212d383dc7a9d8148dfccfbcc139deb5f0c7718cac610d4707e2`  
		Last Modified: Fri, 02 Sep 2022 02:24:16 GMT  
		Size: 68.6 MB (68635084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a147a6bdb02d471ccfe5c14f82e463b195033f170feccb02e1db2bb128b051a5`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318ac1fb7ba29d893d6d9bb95215957152ae3ea476a5b7325b44532655c7c37d`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:ca04948aca834499f728692520eff82917de1d768b47751ba4dd0fc5f261c8e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:7e613e248abdf4604776d6ace8eba9998b61b44f3c6cfd7121939c2fc3f1a7d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (124013572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c284e5e829612878511aa9fc0c383708c5a68f2167fa77a515bc2e4b2a35bf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:41:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 03:42:07 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:07 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 03:42:19 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 03:42:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 03:42:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:42:28 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 03:42:29 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 03:43:20 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 03:43:20 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 03:43:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 03:43:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 03:43:41 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 03:43:42 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 03:43:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 03:43:42 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 03:43:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:43:42 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 03:43:42 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf944e49ffa85996da499d5d92c328463b711fd3a1672b809e2824a964da9fb`  
		Last Modified: Fri, 02 Sep 2022 03:48:07 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020ff2b6bb0b679bc28ad3ec3d451993a1ef2282c86f87ca148774d73593a1cc`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 3.8 MB (3765427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977397ae9bc646b6dcf2321014794f535cb5a74110c608b1d1c0986ee1eb1424`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.0 MB (1992954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361cf449d40803e89980d56903e81945ce9fa372a686ea76f4a9c7a646a8337`  
		Last Modified: Fri, 02 Sep 2022 03:48:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d26195015760a28953bf9d2ad8603a66f8508da28d9878f972ddf137a5b34d`  
		Last Modified: Fri, 02 Sep 2022 03:48:05 GMT  
		Size: 2.3 MB (2281503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a47dd94359e3cf2394add8b9de63828e53d9d2195aa09d903a5e2143e6a9c`  
		Last Modified: Fri, 02 Sep 2022 03:48:02 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4132d19a681ab040d5709b46847ab664104c652bf06ef4a02a0b81d909b57979`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701416dc7e3dc54762a773a56a3140235bcd7c031e29891270df8d8156ac566`  
		Last Modified: Fri, 02 Sep 2022 03:48:43 GMT  
		Size: 85.5 MB (85532069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e314a661679bf4986516e7a5521b2ced57b07332a1bee31fdc83146474893a4`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efce0fc30145a5908ba6bf7fd4c4b33fd9d54e593bff96c19842055866bee692`  
		Last Modified: Fri, 02 Sep 2022 03:48:31 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b27d6a2d4a982fb67a724692fd8edd42e1bfe20dd6d2a73b2fb0eb16c27ad7d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102629742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ecf4f48e2978426dbcc04c56a89f22f76339b1ac791bc5baf9052cb4b99890`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:25:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 05:26:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:01 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 05:26:17 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 05:26:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 05:26:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:26:26 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 05:26:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 05:27:16 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 05:27:17 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 05:27:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 05:27:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 05:27:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 05:27:41 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 05:27:43 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 05:27:44 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 05:27:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 05:27:45 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 05:27:46 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0749552ddbb27b679c4c784814a6bc9cff4dea894b4c50ff08211ac33d7141`  
		Last Modified: Fri, 02 Sep 2022 05:33:56 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f3be11a3a90d15ce271dbf8b58dc49944d979b4199b6a9810b17688f071274`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 3.6 MB (3593224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c93d9284a3d0f05825c9fdc3591a7d7d3ae34f1ae103b4ff077a235d40e0f`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 1.9 MB (1898967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232f4136dd4f7f7c1b1de60c1ce430dfdb5d873cdc0e8cf41ac08e1ece7077c2`  
		Last Modified: Fri, 02 Sep 2022 05:33:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ccd89de31befb378b3fd447ebd5efc4fc67e5969c98f28f3df064a191ec01`  
		Last Modified: Fri, 02 Sep 2022 05:33:54 GMT  
		Size: 2.2 MB (2194638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea239af7d9b117acb387a6885623fe9b3dd8df83c1e1cd42c1e418f41e14ef3f`  
		Last Modified: Fri, 02 Sep 2022 05:33:51 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b306f626891fb340fada4bee82bca7350cea48d4b7d9417c8e16d70b607625`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f977adfc1f0b0065e437818c0d56a7fbea2e66cc2c20fcffb22eb2c726a9d32a`  
		Last Modified: Fri, 02 Sep 2022 05:34:31 GMT  
		Size: 66.5 MB (66546741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c63d31682849e6f78d30d0f7433c748e8581611ada5daf827d30785d2918fd2`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d7766f9fa328aaecc5edea92a920254bf6c7d03d0155d4bbc0b2fced86eded`  
		Last Modified: Fri, 02 Sep 2022 05:34:21 GMT  
		Size: 6.7 KB (6701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:efc520a5969afe22458ec081d2591e6c530af4bdc71f4cb66a755645faff34a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117027115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6dac49f7b083a7406a56adae7166704f912cc7c1676485947393adb8952ad3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:09 GMT
ADD file:39b6fa94f6e1300a6fc4b6094e8250c22ecaa6e7c9f934841765d45b919402c5 in / 
# Thu, 01 Sep 2022 23:50:11 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:52:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 04:53:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:12 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 04:53:29 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 04:53:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 04:53:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:53:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 04:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 04:55:03 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 04:55:03 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 04:55:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 04:55:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 04:55:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 04:55:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 04:55:46 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 04:55:47 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 04:55:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 04:55:47 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 04:55:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:9ef77d5e46df05bf9f34e5871097fd038295a2aa5e29f1806ac3a96aa2545b5f`  
		Last Modified: Thu, 01 Sep 2022 23:52:34 GMT  
		Size: 35.7 MB (35721187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55324944c013f5e152ef0fad27126a86f0a45cfff228ed5d376984c8bcb18dbc`  
		Last Modified: Fri, 02 Sep 2022 05:04:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc5813595f57876629a096fc5630c832e5d23f1a6f8c52b86f94b395dd72973`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 4.5 MB (4503005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53136ad37739b4c4b6d5c9c41623f06a89e1c954299e6487b758572c2129b6`  
		Last Modified: Fri, 02 Sep 2022 05:04:41 GMT  
		Size: 1.9 MB (1922006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e9deaa9bc92d6868ca60db4ace55d593c6da8f7dd776648377d6df75bbcdb2`  
		Last Modified: Fri, 02 Sep 2022 05:04:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88549712edded06fae8bfa5c56fae89c47664fc83e5b4a957c2c2764649ebff`  
		Last Modified: Fri, 02 Sep 2022 05:04:42 GMT  
		Size: 2.4 MB (2389323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a4751f2b2dee4c43d237fe7b4ce6e1273b2374fcce6496c681cb525e8d26c1`  
		Last Modified: Fri, 02 Sep 2022 05:04:38 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105f46c3085029c3a9f300164ffa8751b280f2ac336393e07ca596d6f1475929`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997e1406175b8de4067c34e21e14c3e22d70e65d699abfb60d8dfd481f2ef6be`  
		Last Modified: Fri, 02 Sep 2022 05:05:37 GMT  
		Size: 72.5 MB (72476684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66144ed93c4b6752c2c1059ed5ab44b752cc2444db93c44745a7c41c644be878`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39015c23b5aa07433c0d517088d4fb65a3b8e8d59ae9d235e1edc1661971bfb1`  
		Last Modified: Fri, 02 Sep 2022 05:05:19 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:6f4ec55b4c6a791b54f9a18f4f744b8cd3526fdfd9be7d238370ce93fecc9b8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105124376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66ac2973c068da3f5b39dcb1713654443f0ccd0cf7e315dab0de330e787d8c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:18:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 02 Sep 2022 02:18:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 02 Sep 2022 02:18:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 02 Sep 2022 02:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 02 Sep 2022 02:18:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:18:32 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 02 Sep 2022 02:18:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 02 Sep 2022 02:19:29 GMT
ARG MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 02:19:29 GMT
ENV MARIADB_VERSION=1:10.9.2+maria~ubu2204
# Fri, 02 Sep 2022 02:19:29 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
# Fri, 02 Sep 2022 02:19:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 02 Sep 2022 02:19:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.2/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 02 Sep 2022 02:19:50 GMT
VOLUME [/var/lib/mysql]
# Fri, 02 Sep 2022 02:19:50 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 02 Sep 2022 02:19:50 GMT
COPY file:7032e58fbba6784f90935fcf1ff3c389e5b2936aa9e1c6b8b291cbb26774ee2e in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:19:51 GMT
EXPOSE 3306
# Fri, 02 Sep 2022 02:19:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a83a742f8905e65d86bab1137abea13cf130c3c52de601dd27fc4c4188ad7`  
		Last Modified: Fri, 02 Sep 2022 02:23:46 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0074f95048477359d16a331130ff329c74b549bcc5d7a97cd5559fcfe9c7464`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 3.7 MB (3674479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792e98156ec6717f9a09ef69964b1441fc52ea8407babf26638a445cfbca24a7`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.0 MB (1956114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f52d5f8a1d48c335871d777bb6305d30ca6e0d35472d729f97839e5118e1ed`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b51775573dc421f5d01c30c0385676817ad4cd3ed88f8c69fdfe498f57a5b39`  
		Last Modified: Fri, 02 Sep 2022 02:23:45 GMT  
		Size: 2.2 MB (2200620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c5f2dd2c4f8a5fcba9a6bd048360e2483d370947a8e8499b83147d0878d31d`  
		Last Modified: Fri, 02 Sep 2022 02:23:44 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4005206c1b7f520588d957202113c82375fa4ac4b297a19265f0fc8408f6a082`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56247b961b3a212d383dc7a9d8148dfccfbcc139deb5f0c7718cac610d4707e2`  
		Last Modified: Fri, 02 Sep 2022 02:24:16 GMT  
		Size: 68.6 MB (68635084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a147a6bdb02d471ccfe5c14f82e463b195033f170feccb02e1db2bb128b051a5`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318ac1fb7ba29d893d6d9bb95215957152ae3ea476a5b7325b44532655c7c37d`  
		Last Modified: Fri, 02 Sep 2022 02:24:06 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
