## `mariadb:focal`

```console
$ docker pull mariadb@sha256:6b27df78e91348af6ac28e120a9d3f2852bb4c17d427365a4dad01b206616271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:9d8e15413edbb1d3427eb6d7c0c6c29c753fc8ec90198b2cb0d267848be5ef8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128669750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2347bb009b3aed43ac2d34e8ee63742db209d11aead54f52aa8516e8cadd93d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:33 GMT
ADD file:8a50ad78a668527e974b05a3dfbfd64760de3cb643ceb8a8805d21f6ceab3389 in / 
# Thu, 03 Mar 2022 20:19:33 GMT
CMD ["bash"]
# Fri, 04 Mar 2022 01:29:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 04 Mar 2022 01:29:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 01:29:20 GMT
ENV GOSU_VERSION=1.14
# Fri, 04 Mar 2022 01:29:33 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 04 Mar 2022 01:29:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 04 Mar 2022 01:29:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 01:29:41 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 04 Mar 2022 01:30:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 04 Mar 2022 01:31:02 GMT
ARG MARIADB_MAJOR=10.7
# Fri, 04 Mar 2022 01:31:02 GMT
ENV MARIADB_MAJOR=10.7
# Fri, 04 Mar 2022 01:31:02 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 04 Mar 2022 01:31:02 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Fri, 04 Mar 2022 01:31:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:31:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:31:25 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:31:26 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:31:26 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:31:26 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:31:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:31:26 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:31:26 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:7c3b88808835aa80f1ef7f03083c5ae781d0f44e644537cd72de4ce6c5e62e00`  
		Last Modified: Thu, 03 Mar 2022 20:20:44 GMT  
		Size: 28.6 MB (28565751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea07b32fcfa501c174644efe526fd720030360a22e639f0032b8812ba6fbd16`  
		Last Modified: Fri, 04 Mar 2022 01:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0da78414e6707b17fbf5b24d5ecea5daf2524ff199379e30b1194ca75c6341`  
		Last Modified: Fri, 04 Mar 2022 01:36:34 GMT  
		Size: 5.5 MB (5488522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d4a282af8c4c8caa7de3456f04056a1ef892abca8f79657a5085fdef373dda`  
		Last Modified: Fri, 04 Mar 2022 01:36:34 GMT  
		Size: 3.6 MB (3585327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5ebf090d5054559c071aa461510b09c63b2325f73337582250928b802e9186`  
		Last Modified: Fri, 04 Mar 2022 01:36:33 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fb17be3731c394ef7eee6288691f6749d0bd05bdde6f81a256c610e477c098`  
		Last Modified: Fri, 04 Mar 2022 01:36:34 GMT  
		Size: 2.3 MB (2273146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c50e71525408faaa7cb99f46386124056960332ddcc895ba4321cb34054efa6`  
		Last Modified: Fri, 04 Mar 2022 01:36:31 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e743776c21971bddfd2d6f10d988d2c0553fc40dc820280dfb60ed74db47ad`  
		Last Modified: Fri, 04 Mar 2022 01:37:00 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1d9df5057abf34e16b21bb8f5cfc4dc24a51731d99fa16daad8c9b9694d22d`  
		Last Modified: Fri, 04 Mar 2022 01:37:13 GMT  
		Size: 88.7 MB (88742187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aff42e578374ee1309d18ae266450f909b543639cd73cd7211f340b3db92ec`  
		Last Modified: Fri, 04 Mar 2022 01:37:00 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801f750ef6ac9e27b226a993dd24c018db119e420445fd8e5b56506980fae1e2`  
		Last Modified: Fri, 04 Mar 2022 01:37:00 GMT  
		Size: 6.6 KB (6606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c64c786cd5c9a0375bc3fc876cc8986f2487449446f41e74f4a86de5257e77ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125722169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a1261884782075e3e63b9fc658aefde2d97fee2f128ae762adefe89c74e3c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 03 Mar 2022 19:41:02 GMT
ADD file:f2fffe739729839aa17484bc4d79d33425549c5052824eac12131b16c23565d3 in / 
# Thu, 03 Mar 2022 19:41:03 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 20:37:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Mar 2022 20:38:02 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 20:38:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Mar 2022 20:38:19 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Mar 2022 20:38:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Mar 2022 20:38:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 20:38:28 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Mar 2022 20:39:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Thu, 03 Mar 2022 20:40:01 GMT
ARG MARIADB_MAJOR=10.7
# Thu, 03 Mar 2022 20:40:02 GMT
ENV MARIADB_MAJOR=10.7
# Thu, 03 Mar 2022 20:40:03 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Thu, 03 Mar 2022 20:40:04 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Thu, 03 Mar 2022 20:40:05 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:40:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:40:40 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:40:40 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:40:42 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:40:43 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:40:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:40:44 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:40:45 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:5a7855fb0d7ae372c824d9c76be5ad2f42ce178c1910fa54a8543036b5325fd5`  
		Last Modified: Thu, 03 Mar 2022 19:42:38 GMT  
		Size: 27.2 MB (27169631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cb7d0a0ede3c37656907f69e20caac835e038b51861b994bda59caf5a2da5d`  
		Last Modified: Thu, 03 Mar 2022 20:47:16 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba30ee1ecbe99ea01b720ceabe3c6ebac15c37034a6804ae11d3e1fa3663555f`  
		Last Modified: Thu, 03 Mar 2022 20:47:15 GMT  
		Size: 5.3 MB (5320409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb3762cc26da63c43e9112e69fa7083ba111f316a2e5b152b9c9c1aab772d83`  
		Last Modified: Thu, 03 Mar 2022 20:47:15 GMT  
		Size: 3.4 MB (3370515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d1b9ba1beb6444e8ee93dcadc841d674c0cd537878398475c2fdaad9f81ec6`  
		Last Modified: Thu, 03 Mar 2022 20:47:13 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3768809df5a747edaa773acaed77e8bce8202000597b81eea0db0ec8e72ff4ea`  
		Last Modified: Thu, 03 Mar 2022 20:47:14 GMT  
		Size: 2.2 MB (2203656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c40dafa20f5b392e53f63cdc07967793a12af7f907ba859d8fe8cdb14182fe`  
		Last Modified: Thu, 03 Mar 2022 20:47:11 GMT  
		Size: 2.5 KB (2467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd51e9cd15ff53865e0c48e457dc6c42c508a4898bdfa3c64646e8c0db551a7`  
		Last Modified: Thu, 03 Mar 2022 20:47:43 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaf8b6fef525616f67dd35f4dce7a88b036237fa21182619f3f4e312dce31fe`  
		Last Modified: Thu, 03 Mar 2022 20:47:56 GMT  
		Size: 87.6 MB (87643221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c697180d8d09b61ae1f8dbccc0ebe9178d175b4d2cad717290e7389bbd611d3`  
		Last Modified: Thu, 03 Mar 2022 20:47:43 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d34ac18dfa47481af3310526cb3f715fc0153db7ffc4308aee7ae53d5b0143d`  
		Last Modified: Thu, 03 Mar 2022 20:47:43 GMT  
		Size: 6.6 KB (6612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:211f00b6a71e1253b592dcbf9c7ed4e69aabda3fe19a0c499221493fe3407074
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139539796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ad0d6046ce0e058db17c2a612f1d620a8539483f498069100e0b7cf0a344aeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 03 Mar 2022 20:28:30 GMT
ADD file:039f04ac6c5dbbe3fb0a5eee16945cf7c5fb7565751d6bdf8ec0c1102798c1de in / 
# Thu, 03 Mar 2022 20:28:38 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 22:25:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Mar 2022 22:26:00 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 22:26:04 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Mar 2022 22:26:49 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Mar 2022 22:26:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Mar 2022 22:27:27 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 22:27:31 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Mar 2022 22:28:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Thu, 03 Mar 2022 22:32:58 GMT
ARG MARIADB_MAJOR=10.7
# Thu, 03 Mar 2022 22:33:00 GMT
ENV MARIADB_MAJOR=10.7
# Thu, 03 Mar 2022 22:33:05 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Thu, 03 Mar 2022 22:33:08 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Thu, 03 Mar 2022 22:33:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:33:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:35:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:35:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:35:52 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:35:53 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:35:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:35:57 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:36:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:a16b43de69d1e799ea2cb675e7e605db0ff3a8d692fd326fbde80a370e0676d5`  
		Last Modified: Thu, 03 Mar 2022 20:33:55 GMT  
		Size: 33.3 MB (33292195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c034414663f1a434487a3200e969ad3ad696cb4f4baffc6f55f9d71b5e181f6`  
		Last Modified: Thu, 03 Mar 2022 22:56:21 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0d1b26b3589734688e17cd5573020dcd0a0b5e9f1c2b80500e1234f06ef909`  
		Last Modified: Thu, 03 Mar 2022 22:56:20 GMT  
		Size: 6.7 MB (6667314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd32076c999b7de1dda89f33686295c3cf9016efe05539645e8f7795666feb0`  
		Last Modified: Thu, 03 Mar 2022 22:56:19 GMT  
		Size: 3.7 MB (3672816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb38eff6b0f5b0233130edf2655b851c2a61bfd9c29bc1966188fefb6b8a3d7b`  
		Last Modified: Thu, 03 Mar 2022 22:56:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ac6e9d97473d01db85343a7802a13bc7223469b25132e47bae1735b99e2256`  
		Last Modified: Thu, 03 Mar 2022 22:56:19 GMT  
		Size: 2.6 MB (2568911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7840a85b52c91cf10213329ddcc4f98f52132c800cb2dda3f233eee11b102852`  
		Last Modified: Thu, 03 Mar 2022 22:56:16 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f9ee0bb0d24cd0add12e6950c2cf01d9445e2f5f364febe61669d8190dcb80`  
		Last Modified: Thu, 03 Mar 2022 22:56:55 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c7d67d6391a0c3d226ee10f0980227b312e8add329a36e50fa7abc0cd02a7e`  
		Last Modified: Thu, 03 Mar 2022 22:57:13 GMT  
		Size: 93.3 MB (93323724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379ad556719b3bcc9146a78f22f7c561aa65bb5204dba0a31b0185fbbe2a1d2b`  
		Last Modified: Thu, 03 Mar 2022 22:56:55 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3907dcc782f1b86d6124cb34d21064b10f5758cfacff1b16b8d267ee1207ce1`  
		Last Modified: Thu, 03 Mar 2022 22:56:55 GMT  
		Size: 6.6 KB (6612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; s390x

```console
$ docker pull mariadb@sha256:cbd7d6f9b3ede39745b2cbf2da80a586ff5604c4094b2916ef6e3639866883d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127723404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8004db21ce18c49ba9bf6051185b5eb210857e08d130616e084493d2d7ad57c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 03 Mar 2022 19:41:52 GMT
ADD file:3162233da685a36a9f274a7fa1d99452cab76f37e3640d38851c782ca506f75b in / 
# Thu, 03 Mar 2022 19:41:53 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 20:24:54 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Mar 2022 20:25:02 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 20:25:02 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Mar 2022 20:25:12 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Mar 2022 20:25:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Mar 2022 20:25:18 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 20:25:18 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Mar 2022 20:25:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Thu, 03 Mar 2022 20:26:27 GMT
ARG MARIADB_MAJOR=10.7
# Thu, 03 Mar 2022 20:26:27 GMT
ENV MARIADB_MAJOR=10.7
# Thu, 03 Mar 2022 20:26:27 GMT
ARG MARIADB_VERSION=1:10.7.3+maria~focal
# Thu, 03 Mar 2022 20:26:27 GMT
ENV MARIADB_VERSION=1:10.7.3+maria~focal
# Thu, 03 Mar 2022 20:26:28 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:26:28 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:26:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.7.3/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:26:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:26:51 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:26:51 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:26:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:26:51 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:26:51 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:ade7e68f4e34f438527a34c9761a285c3c3864e3daab0544b2c4f4163c7c3f56`  
		Last Modified: Thu, 03 Mar 2022 19:43:22 GMT  
		Size: 27.1 MB (27084671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1c901b7fe0ba768d35affda39a426a2ce110374db907162a6385e8a60d911d`  
		Last Modified: Thu, 03 Mar 2022 20:28:47 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72521e4e02fa0f83161feb3a74cab677ffb98d7428f240562458443a90e3d440`  
		Last Modified: Thu, 03 Mar 2022 20:28:47 GMT  
		Size: 5.4 MB (5378449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c05ecc05421ad4cbd7bdde741a0e84ffe463c756a4e2607efa3faed80e4158`  
		Last Modified: Thu, 03 Mar 2022 20:28:46 GMT  
		Size: 3.2 MB (3244671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5987189c967beb2e7697770afea0ff68de57a6fdfa15ad187bf4af2beb4956c`  
		Last Modified: Thu, 03 Mar 2022 20:28:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3ea0a1fc33d2cb1b563fd34db789822089fd3e154876737411462e200dcd87`  
		Last Modified: Thu, 03 Mar 2022 20:28:46 GMT  
		Size: 2.2 MB (2185670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327e498818aa1839545fa3d69e3806bdaf581a6ea0047d877248831f39fbc892`  
		Last Modified: Thu, 03 Mar 2022 20:28:44 GMT  
		Size: 2.5 KB (2494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673e09ffa6454810dab819d93e984d2e1c5cae77e306aed3e46ce13b103820f5`  
		Last Modified: Thu, 03 Mar 2022 20:29:32 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1547c46f046cd1e58fcc8349853eb9e33cf64b48ed1d40aa6b70597cd0f76edc`  
		Last Modified: Thu, 03 Mar 2022 20:29:45 GMT  
		Size: 89.8 MB (89815119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8f47ca9916820fbdf4e98fa5d171bca18ffb6b1985e3def02821a4c9eaa32a`  
		Last Modified: Thu, 03 Mar 2022 20:29:32 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c12da7d297a9eea8de987ea587edf9600adaefa9f299883e4dc18fc75b73dca`  
		Last Modified: Thu, 03 Mar 2022 20:29:32 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
