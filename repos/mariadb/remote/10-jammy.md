## `mariadb:10-jammy`

```console
$ docker pull mariadb@sha256:59ef1139afa1ec26f98e316a8dbef657daf9f64f84e9378b190d1d7557ad2feb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:d0e123b5f1a7ff84400e414f314fd4a2612fb41964e4198645bc0bab13cca257
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124063339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14f1097913ecb422c61f9b35604339c1ac74394e7df7f84f765917b018605b5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:19:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Oct 2022 18:20:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:20:13 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Oct 2022 18:20:24 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 18:20:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 18:20:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 18:20:32 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Oct 2022 18:20:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 05 Oct 2022 18:21:18 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 05 Oct 2022 18:21:18 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 05 Oct 2022 18:21:18 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 05 Oct 2022 18:21:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Oct 2022 18:21:39 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 05 Oct 2022 18:21:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Oct 2022 18:21:40 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Oct 2022 18:21:40 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 05 Oct 2022 18:21:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:21:40 GMT
EXPOSE 3306
# Wed, 05 Oct 2022 18:21:40 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a7b642a1b0a294f22a84cef0a64e49b4cc577be51ba20610b1b4779975bf70`  
		Last Modified: Wed, 05 Oct 2022 18:26:02 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05db1f7ddc9cd3a0c79485afd837c0297f587c324caf591eeed30bf156f8cb8`  
		Last Modified: Wed, 05 Oct 2022 18:26:01 GMT  
		Size: 3.8 MB (3765925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043662c3afa15736ef23ed73c90d3393dcace02c6b30901d8b83a2a3363e605c`  
		Last Modified: Wed, 05 Oct 2022 18:26:01 GMT  
		Size: 2.0 MB (1993403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de48eea2079512802b53a7cd68f28181531de82282b6f4d858e9d0931f82598c`  
		Last Modified: Wed, 05 Oct 2022 18:26:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a40b9e7476df9e56ca11b2af7f84e6a6785b452c69e40abafccc632b2b7b24c`  
		Last Modified: Wed, 05 Oct 2022 18:26:00 GMT  
		Size: 2.3 MB (2281989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d053ff7fa7cc2b81dc849479d911cfe131f00f698ef2dba91187d83d63877251`  
		Last Modified: Wed, 05 Oct 2022 18:25:58 GMT  
		Size: 2.5 KB (2486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4459f17c9a820d11290206f0884cbe7331a1b3f871232d01f0ea159909b97d3`  
		Last Modified: Wed, 05 Oct 2022 18:26:29 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ae67b7d96ad681d29189c35d030f5ec8a32eadaad77c96053bb30923b8f875`  
		Last Modified: Wed, 05 Oct 2022 18:26:41 GMT  
		Size: 85.6 MB (85577843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd55ebdb8b38d8a634c6ce32da44216bc460bdbb1c0b3bf2448288b313199a0`  
		Last Modified: Wed, 05 Oct 2022 18:26:29 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf1cda74ce367c9ad6ce95e30437ade711ac8f028911b45b029e218a842444c`  
		Last Modified: Wed, 05 Oct 2022 18:26:29 GMT  
		Size: 7.1 KB (7051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bc8dad79c60dbee794c978c938513edf7e7a46d8b4165a3dbec40f0ebcd8df87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118458840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bace6f58537f6d5dbd005c09307435d45f2319c9a40c0253d6996c48ab71f23`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:07:12 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Oct 2022 16:07:21 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:07:22 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Oct 2022 16:07:38 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 16:07:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 16:07:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:07:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Oct 2022 16:07:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 05 Oct 2022 16:08:25 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 05 Oct 2022 16:08:26 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 05 Oct 2022 16:08:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 05 Oct 2022 16:08:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Oct 2022 16:08:49 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 05 Oct 2022 16:08:50 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Oct 2022 16:08:52 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Oct 2022 16:08:53 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 05 Oct 2022 16:08:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 16:08:54 GMT
EXPOSE 3306
# Wed, 05 Oct 2022 16:08:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f45cf86f5dae7ede91d56c422ba172d128ec239afb29b501694825a3a6b9c8`  
		Last Modified: Wed, 05 Oct 2022 16:15:03 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828f7983eb40e7a9d41441b18adb7f7f6fe0ee244ee594017d65cb4a35a8f22c`  
		Last Modified: Wed, 05 Oct 2022 16:15:02 GMT  
		Size: 3.6 MB (3593384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b55bf63d622781c97dd6892ab84e218db42cb8e1543e94c5b088bff48dcc10d`  
		Last Modified: Wed, 05 Oct 2022 16:15:01 GMT  
		Size: 1.9 MB (1899044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02da7854b91e6d5e3e6aa68c38e4100a8db2b24f597b399e17ad7f8b5419228`  
		Last Modified: Wed, 05 Oct 2022 16:15:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392aa3b0997115941497e7ffc3c011b1ab034d6a498e8d5b54531338f0474e1`  
		Last Modified: Wed, 05 Oct 2022 16:15:01 GMT  
		Size: 2.2 MB (2194811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce511e95889a4fa1be31558e47511ff7fa76561561251df17d152ecd28e1291`  
		Last Modified: Wed, 05 Oct 2022 16:14:58 GMT  
		Size: 2.5 KB (2466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7355d74c33c487645701c9011022e02134eadb348bc359a54c4d291933f68`  
		Last Modified: Wed, 05 Oct 2022 16:15:29 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e8bb90d0b9a31e15b2388e3dab511fae6f4b267070d6244ee26c89469ca4b9`  
		Last Modified: Wed, 05 Oct 2022 16:15:41 GMT  
		Size: 82.4 MB (82374167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307600b8892c8580b654482e8688afad55a6b1fe8c82d7b612bee697e7a12c55`  
		Last Modified: Wed, 05 Oct 2022 16:15:29 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6426d43a7b283292c47c5cf2e0801be51b93b43d9cb01fa8b5a9d8c698445fb`  
		Last Modified: Wed, 05 Oct 2022 16:15:29 GMT  
		Size: 7.1 KB (7053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8c7ccaf2235de2e305c9966499745bf689d8a1c4b272d10c82b8d7fecf7e625a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117037301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef52765abc10bd9a8bca6bdbd245a8a457113aa5a2fac32e77a6f52cbc1430a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 05 Oct 2022 10:52:24 GMT
ADD file:5f3953a21754ce756642c9ddcf521f2cfe220a5fe988ccec51085bd074fbe46e in / 
# Wed, 05 Oct 2022 10:52:26 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 19:39:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Oct 2022 19:39:27 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 19:39:27 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Oct 2022 19:39:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 19:39:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 19:39:59 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 19:40:00 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Oct 2022 19:40:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 05 Oct 2022 19:41:23 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 05 Oct 2022 19:41:23 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 05 Oct 2022 19:41:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 05 Oct 2022 19:41:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Oct 2022 19:42:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 05 Oct 2022 19:42:16 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Oct 2022 19:42:16 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Oct 2022 19:42:17 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 05 Oct 2022 19:42:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 19:42:17 GMT
EXPOSE 3306
# Wed, 05 Oct 2022 19:42:18 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:5053ecffedc109608feacf4836ad15e0f7b2f6a411250a41574342de479c4760`  
		Last Modified: Wed, 05 Oct 2022 10:54:49 GMT  
		Size: 35.7 MB (35709341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6492521ba34bca4d3879faa842813d6598d6a3f95a7d3d8e272d28a49d6742`  
		Last Modified: Wed, 05 Oct 2022 19:51:20 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df256ac100aa9d47e1affe5db73042991edd4973f6c390aee0b21cf78650037f`  
		Last Modified: Wed, 05 Oct 2022 19:51:19 GMT  
		Size: 4.5 MB (4503334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f499034fea8bdb938bc658c8c66629513704b21564124730fb50de2332147b8`  
		Last Modified: Wed, 05 Oct 2022 19:51:18 GMT  
		Size: 1.9 MB (1922298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee1809af9435200c8e022c33a196d2ffb4bffd60039f3d4644f9f2ddcde8528`  
		Last Modified: Wed, 05 Oct 2022 19:51:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee54937a0b44b9aec11cc1783a0ef096d4833294252023fb69ec5529407e199b`  
		Last Modified: Wed, 05 Oct 2022 19:51:19 GMT  
		Size: 2.4 MB (2389681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f4efe335c8c3c61679c040d8d57bddd0c9d7cb89437cb619e0929ce0387251`  
		Last Modified: Wed, 05 Oct 2022 19:51:16 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d827306f778d6fc0b94f38de086f1adc3d329a8ba8193dd0a1addbf0dc69119`  
		Last Modified: Wed, 05 Oct 2022 19:51:55 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e2f021e75fa92f6e8e61cf7ea2812d7f74de6a3ab11bdade539c942ddb4c90`  
		Last Modified: Wed, 05 Oct 2022 19:52:14 GMT  
		Size: 72.5 MB (72497380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdf8f08f146ebe42d4cbd9e78e9ad1b3834ccf310ed3b31136b5fb424af7703`  
		Last Modified: Wed, 05 Oct 2022 19:51:55 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f26fcd40063abc524a729020b6d5ce455d24bccccde3ff5d911d99f5d5728ad`  
		Last Modified: Wed, 05 Oct 2022 19:51:55 GMT  
		Size: 7.1 KB (7053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:38506030317607d8b7e3f0b4c61ea2deace18b5ec30296db4d1b272748422618
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105148860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cecd0240a7c3c2deb6fc2f7d179ce194fc4827a13d73e12cc8c02ee04fe9bf28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 04 Oct 2022 23:52:57 GMT
ADD file:b1fcc8690fce8195995c8eab6b853225d65017d69692537273760bf84bfb72ec in / 
# Tue, 04 Oct 2022 23:52:59 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 07:38:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Oct 2022 07:38:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 07:38:19 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Oct 2022 07:38:27 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 07:38:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 07:38:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 07:38:33 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 05 Oct 2022 07:38:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 05 Oct 2022 07:39:15 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 05 Oct 2022 07:39:15 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 05 Oct 2022 07:39:16 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 05 Oct 2022 07:39:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 05 Oct 2022 07:39:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 05 Oct 2022 07:39:34 GMT
VOLUME [/var/lib/mysql]
# Wed, 05 Oct 2022 07:39:34 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 05 Oct 2022 07:39:34 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 05 Oct 2022 07:39:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 07:39:34 GMT
EXPOSE 3306
# Wed, 05 Oct 2022 07:39:34 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:29c30188ad5f0c76a8b336bfa488a1bdf199dc8127ed81e4051c1c71d4da8f87`  
		Last Modified: Tue, 04 Oct 2022 23:54:34 GMT  
		Size: 28.6 MB (28643466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5552eadcd8cbe4fbd91ec56c5adde7f174149b98f796ef39772979a4e857a`  
		Last Modified: Wed, 05 Oct 2022 07:43:47 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8eb60e84545d83364f64670912b666ca195c42501e4bfc5e712f7260e70fac`  
		Last Modified: Wed, 05 Oct 2022 07:43:46 GMT  
		Size: 3.7 MB (3674820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab416e636daf0aa6f9b54c5a58f297b1b42d737eda48c895d9355de48c852803`  
		Last Modified: Wed, 05 Oct 2022 07:43:46 GMT  
		Size: 2.0 MB (1956637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e204894bc2ef3297f6f485cb66d29f1260f7cde20b119c3158e8ae2f146491`  
		Last Modified: Wed, 05 Oct 2022 07:43:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89656060a3112850052080e2be6f1ef7b6aa739325820f5a7c5ed3ab4fd70add`  
		Last Modified: Wed, 05 Oct 2022 07:43:46 GMT  
		Size: 2.2 MB (2200973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde6fbb6c94194a3112545dd18dcdad0d19139e2638908de582494e2ee0b288c`  
		Last Modified: Wed, 05 Oct 2022 07:43:45 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268a0653ff5ab49acba0df669507fe8204ed46a7524780e01d532d1649105dba`  
		Last Modified: Wed, 05 Oct 2022 07:44:05 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6cd2387479a39d04056914d3f07e49894a75d2e67d6bc86e280ddf9519d0d2`  
		Last Modified: Wed, 05 Oct 2022 07:44:14 GMT  
		Size: 68.7 MB (68657707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b7fdcee1a32e583740921cae255c05c3ef6c439f3b9d7da368aa62fa3ba55b`  
		Last Modified: Wed, 05 Oct 2022 07:44:05 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a3e8f62e4022ae1c4769e1c99e967e06d9af658132850e8fdebf2c381fe972`  
		Last Modified: Wed, 05 Oct 2022 07:44:05 GMT  
		Size: 7.0 KB (7050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
