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
$ docker pull mariadb@sha256:6b27df78e91348af6ac28e120a9d3f2852bb4c17d427365a4dad01b206616271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

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

### `mariadb:10` - linux; arm64 variant v8

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

### `mariadb:10` - linux; ppc64le

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

### `mariadb:10` - linux; s390x

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

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:6b27df78e91348af6ac28e120a9d3f2852bb4c17d427365a4dad01b206616271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-focal` - linux; amd64

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

### `mariadb:10-focal` - linux; arm64 variant v8

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

### `mariadb:10-focal` - linux; ppc64le

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

### `mariadb:10-focal` - linux; s390x

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

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:2be735c31a84f8bef59453e25096f00725996ecc898cd63c85a5bab9d8d55e73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:c39c39622a5c7f76b822660e443065eb19ec5953e5d2d2f38480152bc1add1f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109315472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd38a6d0e06c967211edb3cd5373a2243add1743670d6f73d1c770bc0fcfbf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:25 GMT
ADD file:dee0aa8497bd26ca41dffa17adff99be2523f66f9b2c557ba9ad2388ed052dca in / 
# Thu, 03 Mar 2022 20:19:25 GMT
CMD ["bash"]
# Fri, 04 Mar 2022 01:34:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 04 Mar 2022 01:34:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 01:34:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 04 Mar 2022 01:34:37 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 04 Mar 2022 01:34:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 04 Mar 2022 01:34:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 01:34:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 04 Mar 2022 01:35:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 04 Mar 2022 01:35:11 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 04 Mar 2022 01:35:11 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 04 Mar 2022 01:35:11 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 04 Mar 2022 01:35:11 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 04 Mar 2022 01:35:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 04 Mar 2022 01:35:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:35:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:35:51 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:35:51 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:35:52 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:35:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 04 Mar 2022 01:35:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:35:52 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:35:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:cf06a7c3161117888114e7e91dbd21915efae33c2dbfb086380f7b21946d6e59`  
		Last Modified: Thu, 03 Mar 2022 20:20:28 GMT  
		Size: 26.7 MB (26708326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1093d8856850aa9c407c0e1fbd1fd9c15586ef180aa93eb761ac908b69d2282`  
		Last Modified: Fri, 04 Mar 2022 01:39:49 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a501f32201bd7d878d0e3e40672ff7d4cde1f009265e5f5dc41e626ed778a9fb`  
		Last Modified: Fri, 04 Mar 2022 01:39:50 GMT  
		Size: 4.8 MB (4813149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070a1d79248ddb35249fef2cc00563b5d69128c495de75a85b5c677c406744bb`  
		Last Modified: Fri, 04 Mar 2022 01:39:48 GMT  
		Size: 3.6 MB (3552993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed8642e399ce3b898bd2ca29fcacd177c602b46c76e2b7cd4bde91cbf0707ef`  
		Last Modified: Fri, 04 Mar 2022 01:39:47 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3d8aa77bbb83cb3894f356d831ab4bf8a4928c7e7ef3ce326ef0251f5b8e6c`  
		Last Modified: Fri, 04 Mar 2022 01:39:47 GMT  
		Size: 1.6 MB (1583490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ca5f9a654b7771b85ba3c9a1fdf3ea5202c1556cdbaff5df8428a97776b936`  
		Last Modified: Fri, 04 Mar 2022 01:39:47 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a19aa6be0453f90b8e4d4d14ab00cd2e173b16da308b6bba508671850ef80a9`  
		Last Modified: Fri, 04 Mar 2022 01:39:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525c33b687750e1ea4ac295fbd5e0726fd76645397b10729d54b6a2543779b8b`  
		Last Modified: Fri, 04 Mar 2022 01:39:55 GMT  
		Size: 72.6 MB (72639774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328b707107df2094612185e8e0cdf827e5cdf2faf77feb910472951cd6a5f852`  
		Last Modified: Fri, 04 Mar 2022 01:39:45 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d139578a9ff1f46e3fc6beb40f77200e225a4026b3ba9af39810a986c00552a8`  
		Last Modified: Fri, 04 Mar 2022 01:39:44 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c8a23bc4f63b279ed68b773deefadbc03777fd5cbf93aad09122f249e30a2c`  
		Last Modified: Fri, 04 Mar 2022 01:39:44 GMT  
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
$ docker pull mariadb@sha256:9e490cca468a229e193f8cb2f332b7df05fccc9b60b8cf2d4b19cebd67e02b91
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117714556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:127048d88c5a6d84b48e16081ba344dcf776c12231f7b07021c13df97044fcdb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 03 Mar 2022 20:27:52 GMT
ADD file:1070cef5a9454e0fdf7349b67652cf1ee9f02fb2679b05c10cfd1d7e2c378145 in / 
# Thu, 03 Mar 2022 20:27:59 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 22:48:37 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Mar 2022 22:49:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 22:49:31 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Mar 2022 22:50:10 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Mar 2022 22:50:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Mar 2022 22:50:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 22:50:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Mar 2022 22:51:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Thu, 03 Mar 2022 22:51:36 GMT
ARG MARIADB_MAJOR=10.2
# Thu, 03 Mar 2022 22:51:38 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 03 Mar 2022 22:51:44 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Thu, 03 Mar 2022 22:51:48 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Thu, 03 Mar 2022 22:51:51 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Thu, 03 Mar 2022 22:51:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:54:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:54:23 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:54:25 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:54:26 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:54:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 22:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:54:38 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:54:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b055ba315c818484fa9979213cb00d276e7ec194a6928dd1270f73cf2aaa73b2`  
		Last Modified: Thu, 03 Mar 2022 20:31:51 GMT  
		Size: 30.4 MB (30437967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c620c1117b04b4361d6cb2a7f3132a902c470ef490a580adf92e228684d9a80`  
		Last Modified: Thu, 03 Mar 2022 23:00:35 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337f7ec9c79a70e8842a990f15c3fec40eb9d60ee94f17d05b56b140760355e3`  
		Last Modified: Thu, 03 Mar 2022 23:00:36 GMT  
		Size: 5.6 MB (5630255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea0329aec4cd6e9ddaec81b348644870bffc5656f689913a674ff60d8465162`  
		Last Modified: Thu, 03 Mar 2022 23:00:33 GMT  
		Size: 3.5 MB (3533410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6636508862ed43866cfe1adb9f5f559baadd5dc9dfdc983b0bd9ccddf284651c`  
		Last Modified: Thu, 03 Mar 2022 23:00:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc06a5aedd0cf1630c57f568b3235456a35847b57936023021163febaa137a7`  
		Last Modified: Thu, 03 Mar 2022 23:00:34 GMT  
		Size: 1.9 MB (1936887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587759812d41db503d090ee22cfb13feab044198f0614f43d3e85d7e072b152`  
		Last Modified: Thu, 03 Mar 2022 23:00:32 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edacceebe5a06ed65de2c5d44d8d85803b15042d7596aeddc0c8358137bc5632`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752a59645d11034250c172beddc43288de66adfb92afcd9b003166ab7b51353d`  
		Last Modified: Thu, 03 Mar 2022 23:00:43 GMT  
		Size: 76.2 MB (76158279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e75e04a702fccd39453db3fa3403a02011ba43e8f916a5d32991d7d7f3bc2`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf170e56ee4ff8df80df9dca523ed343f28660be7551b85540e1757b5dac1d`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d468e43ff2f8907cefe84aca573474e795738ce7c8ffaa5480206b4b6d0852c`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:2be735c31a84f8bef59453e25096f00725996ecc898cd63c85a5bab9d8d55e73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:c39c39622a5c7f76b822660e443065eb19ec5953e5d2d2f38480152bc1add1f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109315472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd38a6d0e06c967211edb3cd5373a2243add1743670d6f73d1c770bc0fcfbf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:25 GMT
ADD file:dee0aa8497bd26ca41dffa17adff99be2523f66f9b2c557ba9ad2388ed052dca in / 
# Thu, 03 Mar 2022 20:19:25 GMT
CMD ["bash"]
# Fri, 04 Mar 2022 01:34:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 04 Mar 2022 01:34:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 01:34:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 04 Mar 2022 01:34:37 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 04 Mar 2022 01:34:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 04 Mar 2022 01:34:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 01:34:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 04 Mar 2022 01:35:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 04 Mar 2022 01:35:11 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 04 Mar 2022 01:35:11 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 04 Mar 2022 01:35:11 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 04 Mar 2022 01:35:11 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 04 Mar 2022 01:35:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 04 Mar 2022 01:35:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:35:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:35:51 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:35:51 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:35:52 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:35:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 04 Mar 2022 01:35:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:35:52 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:35:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:cf06a7c3161117888114e7e91dbd21915efae33c2dbfb086380f7b21946d6e59`  
		Last Modified: Thu, 03 Mar 2022 20:20:28 GMT  
		Size: 26.7 MB (26708326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1093d8856850aa9c407c0e1fbd1fd9c15586ef180aa93eb761ac908b69d2282`  
		Last Modified: Fri, 04 Mar 2022 01:39:49 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a501f32201bd7d878d0e3e40672ff7d4cde1f009265e5f5dc41e626ed778a9fb`  
		Last Modified: Fri, 04 Mar 2022 01:39:50 GMT  
		Size: 4.8 MB (4813149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070a1d79248ddb35249fef2cc00563b5d69128c495de75a85b5c677c406744bb`  
		Last Modified: Fri, 04 Mar 2022 01:39:48 GMT  
		Size: 3.6 MB (3552993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed8642e399ce3b898bd2ca29fcacd177c602b46c76e2b7cd4bde91cbf0707ef`  
		Last Modified: Fri, 04 Mar 2022 01:39:47 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3d8aa77bbb83cb3894f356d831ab4bf8a4928c7e7ef3ce326ef0251f5b8e6c`  
		Last Modified: Fri, 04 Mar 2022 01:39:47 GMT  
		Size: 1.6 MB (1583490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ca5f9a654b7771b85ba3c9a1fdf3ea5202c1556cdbaff5df8428a97776b936`  
		Last Modified: Fri, 04 Mar 2022 01:39:47 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a19aa6be0453f90b8e4d4d14ab00cd2e173b16da308b6bba508671850ef80a9`  
		Last Modified: Fri, 04 Mar 2022 01:39:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525c33b687750e1ea4ac295fbd5e0726fd76645397b10729d54b6a2543779b8b`  
		Last Modified: Fri, 04 Mar 2022 01:39:55 GMT  
		Size: 72.6 MB (72639774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328b707107df2094612185e8e0cdf827e5cdf2faf77feb910472951cd6a5f852`  
		Last Modified: Fri, 04 Mar 2022 01:39:45 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d139578a9ff1f46e3fc6beb40f77200e225a4026b3ba9af39810a986c00552a8`  
		Last Modified: Fri, 04 Mar 2022 01:39:44 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c8a23bc4f63b279ed68b773deefadbc03777fd5cbf93aad09122f249e30a2c`  
		Last Modified: Fri, 04 Mar 2022 01:39:44 GMT  
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
$ docker pull mariadb@sha256:9e490cca468a229e193f8cb2f332b7df05fccc9b60b8cf2d4b19cebd67e02b91
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117714556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:127048d88c5a6d84b48e16081ba344dcf776c12231f7b07021c13df97044fcdb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 03 Mar 2022 20:27:52 GMT
ADD file:1070cef5a9454e0fdf7349b67652cf1ee9f02fb2679b05c10cfd1d7e2c378145 in / 
# Thu, 03 Mar 2022 20:27:59 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 22:48:37 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Mar 2022 22:49:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 22:49:31 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Mar 2022 22:50:10 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Mar 2022 22:50:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Mar 2022 22:50:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 22:50:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Mar 2022 22:51:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Thu, 03 Mar 2022 22:51:36 GMT
ARG MARIADB_MAJOR=10.2
# Thu, 03 Mar 2022 22:51:38 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 03 Mar 2022 22:51:44 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Thu, 03 Mar 2022 22:51:48 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Thu, 03 Mar 2022 22:51:51 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Thu, 03 Mar 2022 22:51:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:54:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:54:23 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:54:25 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:54:26 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:54:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 22:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:54:38 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:54:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b055ba315c818484fa9979213cb00d276e7ec194a6928dd1270f73cf2aaa73b2`  
		Last Modified: Thu, 03 Mar 2022 20:31:51 GMT  
		Size: 30.4 MB (30437967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c620c1117b04b4361d6cb2a7f3132a902c470ef490a580adf92e228684d9a80`  
		Last Modified: Thu, 03 Mar 2022 23:00:35 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337f7ec9c79a70e8842a990f15c3fec40eb9d60ee94f17d05b56b140760355e3`  
		Last Modified: Thu, 03 Mar 2022 23:00:36 GMT  
		Size: 5.6 MB (5630255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea0329aec4cd6e9ddaec81b348644870bffc5656f689913a674ff60d8465162`  
		Last Modified: Thu, 03 Mar 2022 23:00:33 GMT  
		Size: 3.5 MB (3533410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6636508862ed43866cfe1adb9f5f559baadd5dc9dfdc983b0bd9ccddf284651c`  
		Last Modified: Thu, 03 Mar 2022 23:00:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc06a5aedd0cf1630c57f568b3235456a35847b57936023021163febaa137a7`  
		Last Modified: Thu, 03 Mar 2022 23:00:34 GMT  
		Size: 1.9 MB (1936887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587759812d41db503d090ee22cfb13feab044198f0614f43d3e85d7e072b152`  
		Last Modified: Thu, 03 Mar 2022 23:00:32 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edacceebe5a06ed65de2c5d44d8d85803b15042d7596aeddc0c8358137bc5632`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752a59645d11034250c172beddc43288de66adfb92afcd9b003166ab7b51353d`  
		Last Modified: Thu, 03 Mar 2022 23:00:43 GMT  
		Size: 76.2 MB (76158279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e75e04a702fccd39453db3fa3403a02011ba43e8f916a5d32991d7d7f3bc2`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf170e56ee4ff8df80df9dca523ed343f28660be7551b85540e1757b5dac1d`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d468e43ff2f8907cefe84aca573474e795738ce7c8ffaa5480206b4b6d0852c`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.43`

```console
$ docker pull mariadb@sha256:c350866ca888dd6c496f2de70311bd70e3884df1e69daf44d2e8a2edd89c25c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; ppc64le

### `mariadb:10.2.43` - linux; amd64

```console
$ docker pull mariadb@sha256:c39c39622a5c7f76b822660e443065eb19ec5953e5d2d2f38480152bc1add1f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109315472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd38a6d0e06c967211edb3cd5373a2243add1743670d6f73d1c770bc0fcfbf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:25 GMT
ADD file:dee0aa8497bd26ca41dffa17adff99be2523f66f9b2c557ba9ad2388ed052dca in / 
# Thu, 03 Mar 2022 20:19:25 GMT
CMD ["bash"]
# Fri, 04 Mar 2022 01:34:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 04 Mar 2022 01:34:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 01:34:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 04 Mar 2022 01:34:37 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 04 Mar 2022 01:34:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 04 Mar 2022 01:34:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 01:34:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 04 Mar 2022 01:35:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 04 Mar 2022 01:35:11 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 04 Mar 2022 01:35:11 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 04 Mar 2022 01:35:11 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 04 Mar 2022 01:35:11 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 04 Mar 2022 01:35:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 04 Mar 2022 01:35:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:35:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:35:51 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:35:51 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:35:52 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:35:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 04 Mar 2022 01:35:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:35:52 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:35:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:cf06a7c3161117888114e7e91dbd21915efae33c2dbfb086380f7b21946d6e59`  
		Last Modified: Thu, 03 Mar 2022 20:20:28 GMT  
		Size: 26.7 MB (26708326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1093d8856850aa9c407c0e1fbd1fd9c15586ef180aa93eb761ac908b69d2282`  
		Last Modified: Fri, 04 Mar 2022 01:39:49 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a501f32201bd7d878d0e3e40672ff7d4cde1f009265e5f5dc41e626ed778a9fb`  
		Last Modified: Fri, 04 Mar 2022 01:39:50 GMT  
		Size: 4.8 MB (4813149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070a1d79248ddb35249fef2cc00563b5d69128c495de75a85b5c677c406744bb`  
		Last Modified: Fri, 04 Mar 2022 01:39:48 GMT  
		Size: 3.6 MB (3552993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed8642e399ce3b898bd2ca29fcacd177c602b46c76e2b7cd4bde91cbf0707ef`  
		Last Modified: Fri, 04 Mar 2022 01:39:47 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3d8aa77bbb83cb3894f356d831ab4bf8a4928c7e7ef3ce326ef0251f5b8e6c`  
		Last Modified: Fri, 04 Mar 2022 01:39:47 GMT  
		Size: 1.6 MB (1583490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ca5f9a654b7771b85ba3c9a1fdf3ea5202c1556cdbaff5df8428a97776b936`  
		Last Modified: Fri, 04 Mar 2022 01:39:47 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a19aa6be0453f90b8e4d4d14ab00cd2e173b16da308b6bba508671850ef80a9`  
		Last Modified: Fri, 04 Mar 2022 01:39:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525c33b687750e1ea4ac295fbd5e0726fd76645397b10729d54b6a2543779b8b`  
		Last Modified: Fri, 04 Mar 2022 01:39:55 GMT  
		Size: 72.6 MB (72639774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328b707107df2094612185e8e0cdf827e5cdf2faf77feb910472951cd6a5f852`  
		Last Modified: Fri, 04 Mar 2022 01:39:45 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d139578a9ff1f46e3fc6beb40f77200e225a4026b3ba9af39810a986c00552a8`  
		Last Modified: Fri, 04 Mar 2022 01:39:44 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c8a23bc4f63b279ed68b773deefadbc03777fd5cbf93aad09122f249e30a2c`  
		Last Modified: Fri, 04 Mar 2022 01:39:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43` - linux; ppc64le

```console
$ docker pull mariadb@sha256:9e490cca468a229e193f8cb2f332b7df05fccc9b60b8cf2d4b19cebd67e02b91
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117714556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:127048d88c5a6d84b48e16081ba344dcf776c12231f7b07021c13df97044fcdb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 03 Mar 2022 20:27:52 GMT
ADD file:1070cef5a9454e0fdf7349b67652cf1ee9f02fb2679b05c10cfd1d7e2c378145 in / 
# Thu, 03 Mar 2022 20:27:59 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 22:48:37 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Mar 2022 22:49:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 22:49:31 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Mar 2022 22:50:10 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Mar 2022 22:50:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Mar 2022 22:50:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 22:50:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Mar 2022 22:51:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Thu, 03 Mar 2022 22:51:36 GMT
ARG MARIADB_MAJOR=10.2
# Thu, 03 Mar 2022 22:51:38 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 03 Mar 2022 22:51:44 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Thu, 03 Mar 2022 22:51:48 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Thu, 03 Mar 2022 22:51:51 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Thu, 03 Mar 2022 22:51:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:54:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:54:23 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:54:25 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:54:26 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:54:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 22:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:54:38 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:54:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b055ba315c818484fa9979213cb00d276e7ec194a6928dd1270f73cf2aaa73b2`  
		Last Modified: Thu, 03 Mar 2022 20:31:51 GMT  
		Size: 30.4 MB (30437967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c620c1117b04b4361d6cb2a7f3132a902c470ef490a580adf92e228684d9a80`  
		Last Modified: Thu, 03 Mar 2022 23:00:35 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337f7ec9c79a70e8842a990f15c3fec40eb9d60ee94f17d05b56b140760355e3`  
		Last Modified: Thu, 03 Mar 2022 23:00:36 GMT  
		Size: 5.6 MB (5630255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea0329aec4cd6e9ddaec81b348644870bffc5656f689913a674ff60d8465162`  
		Last Modified: Thu, 03 Mar 2022 23:00:33 GMT  
		Size: 3.5 MB (3533410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6636508862ed43866cfe1adb9f5f559baadd5dc9dfdc983b0bd9ccddf284651c`  
		Last Modified: Thu, 03 Mar 2022 23:00:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc06a5aedd0cf1630c57f568b3235456a35847b57936023021163febaa137a7`  
		Last Modified: Thu, 03 Mar 2022 23:00:34 GMT  
		Size: 1.9 MB (1936887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587759812d41db503d090ee22cfb13feab044198f0614f43d3e85d7e072b152`  
		Last Modified: Thu, 03 Mar 2022 23:00:32 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edacceebe5a06ed65de2c5d44d8d85803b15042d7596aeddc0c8358137bc5632`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752a59645d11034250c172beddc43288de66adfb92afcd9b003166ab7b51353d`  
		Last Modified: Thu, 03 Mar 2022 23:00:43 GMT  
		Size: 76.2 MB (76158279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e75e04a702fccd39453db3fa3403a02011ba43e8f916a5d32991d7d7f3bc2`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf170e56ee4ff8df80df9dca523ed343f28660be7551b85540e1757b5dac1d`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d468e43ff2f8907cefe84aca573474e795738ce7c8ffaa5480206b4b6d0852c`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.43-bionic`

```console
$ docker pull mariadb@sha256:c350866ca888dd6c496f2de70311bd70e3884df1e69daf44d2e8a2edd89c25c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; ppc64le

### `mariadb:10.2.43-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:c39c39622a5c7f76b822660e443065eb19ec5953e5d2d2f38480152bc1add1f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109315472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd38a6d0e06c967211edb3cd5373a2243add1743670d6f73d1c770bc0fcfbf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:25 GMT
ADD file:dee0aa8497bd26ca41dffa17adff99be2523f66f9b2c557ba9ad2388ed052dca in / 
# Thu, 03 Mar 2022 20:19:25 GMT
CMD ["bash"]
# Fri, 04 Mar 2022 01:34:08 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 04 Mar 2022 01:34:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 01:34:23 GMT
ENV GOSU_VERSION=1.14
# Fri, 04 Mar 2022 01:34:37 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 04 Mar 2022 01:34:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 04 Mar 2022 01:34:45 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 01:34:46 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 04 Mar 2022 01:35:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 04 Mar 2022 01:35:11 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 04 Mar 2022 01:35:11 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 04 Mar 2022 01:35:11 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 04 Mar 2022 01:35:11 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 04 Mar 2022 01:35:12 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 04 Mar 2022 01:35:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:35:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:35:51 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:35:51 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:35:52 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:35:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 04 Mar 2022 01:35:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:35:52 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:35:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:cf06a7c3161117888114e7e91dbd21915efae33c2dbfb086380f7b21946d6e59`  
		Last Modified: Thu, 03 Mar 2022 20:20:28 GMT  
		Size: 26.7 MB (26708326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1093d8856850aa9c407c0e1fbd1fd9c15586ef180aa93eb761ac908b69d2282`  
		Last Modified: Fri, 04 Mar 2022 01:39:49 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a501f32201bd7d878d0e3e40672ff7d4cde1f009265e5f5dc41e626ed778a9fb`  
		Last Modified: Fri, 04 Mar 2022 01:39:50 GMT  
		Size: 4.8 MB (4813149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070a1d79248ddb35249fef2cc00563b5d69128c495de75a85b5c677c406744bb`  
		Last Modified: Fri, 04 Mar 2022 01:39:48 GMT  
		Size: 3.6 MB (3552993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed8642e399ce3b898bd2ca29fcacd177c602b46c76e2b7cd4bde91cbf0707ef`  
		Last Modified: Fri, 04 Mar 2022 01:39:47 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3d8aa77bbb83cb3894f356d831ab4bf8a4928c7e7ef3ce326ef0251f5b8e6c`  
		Last Modified: Fri, 04 Mar 2022 01:39:47 GMT  
		Size: 1.6 MB (1583490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ca5f9a654b7771b85ba3c9a1fdf3ea5202c1556cdbaff5df8428a97776b936`  
		Last Modified: Fri, 04 Mar 2022 01:39:47 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a19aa6be0453f90b8e4d4d14ab00cd2e173b16da308b6bba508671850ef80a9`  
		Last Modified: Fri, 04 Mar 2022 01:39:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525c33b687750e1ea4ac295fbd5e0726fd76645397b10729d54b6a2543779b8b`  
		Last Modified: Fri, 04 Mar 2022 01:39:55 GMT  
		Size: 72.6 MB (72639774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328b707107df2094612185e8e0cdf827e5cdf2faf77feb910472951cd6a5f852`  
		Last Modified: Fri, 04 Mar 2022 01:39:45 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d139578a9ff1f46e3fc6beb40f77200e225a4026b3ba9af39810a986c00552a8`  
		Last Modified: Fri, 04 Mar 2022 01:39:44 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c8a23bc4f63b279ed68b773deefadbc03777fd5cbf93aad09122f249e30a2c`  
		Last Modified: Fri, 04 Mar 2022 01:39:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:9e490cca468a229e193f8cb2f332b7df05fccc9b60b8cf2d4b19cebd67e02b91
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117714556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:127048d88c5a6d84b48e16081ba344dcf776c12231f7b07021c13df97044fcdb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 03 Mar 2022 20:27:52 GMT
ADD file:1070cef5a9454e0fdf7349b67652cf1ee9f02fb2679b05c10cfd1d7e2c378145 in / 
# Thu, 03 Mar 2022 20:27:59 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 22:48:37 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 03 Mar 2022 22:49:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 22:49:31 GMT
ENV GOSU_VERSION=1.14
# Thu, 03 Mar 2022 22:50:10 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 03 Mar 2022 22:50:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 03 Mar 2022 22:50:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 22:50:43 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 03 Mar 2022 22:51:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Thu, 03 Mar 2022 22:51:36 GMT
ARG MARIADB_MAJOR=10.2
# Thu, 03 Mar 2022 22:51:38 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 03 Mar 2022 22:51:44 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Thu, 03 Mar 2022 22:51:48 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Thu, 03 Mar 2022 22:51:51 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Thu, 03 Mar 2022 22:51:57 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:54:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:54:23 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:54:25 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:54:26 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:54:32 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 22:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:54:38 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:54:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b055ba315c818484fa9979213cb00d276e7ec194a6928dd1270f73cf2aaa73b2`  
		Last Modified: Thu, 03 Mar 2022 20:31:51 GMT  
		Size: 30.4 MB (30437967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c620c1117b04b4361d6cb2a7f3132a902c470ef490a580adf92e228684d9a80`  
		Last Modified: Thu, 03 Mar 2022 23:00:35 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337f7ec9c79a70e8842a990f15c3fec40eb9d60ee94f17d05b56b140760355e3`  
		Last Modified: Thu, 03 Mar 2022 23:00:36 GMT  
		Size: 5.6 MB (5630255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea0329aec4cd6e9ddaec81b348644870bffc5656f689913a674ff60d8465162`  
		Last Modified: Thu, 03 Mar 2022 23:00:33 GMT  
		Size: 3.5 MB (3533410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6636508862ed43866cfe1adb9f5f559baadd5dc9dfdc983b0bd9ccddf284651c`  
		Last Modified: Thu, 03 Mar 2022 23:00:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc06a5aedd0cf1630c57f568b3235456a35847b57936023021163febaa137a7`  
		Last Modified: Thu, 03 Mar 2022 23:00:34 GMT  
		Size: 1.9 MB (1936887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587759812d41db503d090ee22cfb13feab044198f0614f43d3e85d7e072b152`  
		Last Modified: Thu, 03 Mar 2022 23:00:32 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edacceebe5a06ed65de2c5d44d8d85803b15042d7596aeddc0c8358137bc5632`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752a59645d11034250c172beddc43288de66adfb92afcd9b003166ab7b51353d`  
		Last Modified: Thu, 03 Mar 2022 23:00:43 GMT  
		Size: 76.2 MB (76158279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e75e04a702fccd39453db3fa3403a02011ba43e8f916a5d32991d7d7f3bc2`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf170e56ee4ff8df80df9dca523ed343f28660be7551b85540e1757b5dac1d`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d468e43ff2f8907cefe84aca573474e795738ce7c8ffaa5480206b4b6d0852c`  
		Last Modified: Thu, 03 Mar 2022 23:00:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:ebcb6e992ef604e1bd754f8ee811d9a510364fb46d2afaeac745db3d7d946ef1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:a99416d1864bc3b4bce8e9031f35b78d3b6d3304818e8bea96b935874fde90ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120118799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f52c14d4e09c22dbccea6d1ee1632e0b39fb3d356351265c680fbc044ae3687`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Fri, 04 Mar 2022 01:33:34 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 04 Mar 2022 01:33:35 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 04 Mar 2022 01:33:35 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 04 Mar 2022 01:33:35 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 04 Mar 2022 01:33:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:33:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:34:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:34:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:34:02 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:34:02 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:34:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 04 Mar 2022 01:34:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:34:03 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:34:03 GMT
CMD ["mysqld"]
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
	-	`sha256:4021fab8a340817d46cf77acd03ca874abb79e76e9316e95ae29fde940f83e1c`  
		Last Modified: Fri, 04 Mar 2022 01:39:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0249ad56f65a484c68b786f772095ca981050aadbacf32eb5c21cfc9230568`  
		Last Modified: Fri, 04 Mar 2022 01:39:28 GMT  
		Size: 80.2 MB (80191123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac62dbc9c317cb8b2850714c929f287e639946a5f12d7a62a62a38c1fd61432`  
		Last Modified: Fri, 04 Mar 2022 01:39:17 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49439b48c7e27a9eabd3f775b8016b48fb61da8b6d9e0735199397267990904b`  
		Last Modified: Fri, 04 Mar 2022 01:39:16 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efcd95f926748a8f284072a9541986b06c61234d454deb59dc5ac3d8044f9bc0`  
		Last Modified: Fri, 04 Mar 2022 01:39:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dacd236b36bc458e4015952d4ee592e45aaae13f18bb3079b7d17f204e60eaa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117609970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b44f61379408de2bffba45aac163ca3c8c41cd099e2f3609621251a97f748a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:43:30 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 20:43:31 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 20:43:32 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 20:43:33 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 20:43:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:43:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:44:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:44:10 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:44:11 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:44:12 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:44:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 20:44:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:44:14 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:44:15 GMT
CMD ["mysqld"]
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
	-	`sha256:83dc742380af91b69fe3b91d6f26138ac74a8411226a5740719eb0d19045e0da`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0219e24c6a21d875b9f1eae501c6bbd2dbd2e261e3d92b808cec301ab1d8e1e`  
		Last Modified: Thu, 03 Mar 2022 20:50:17 GMT  
		Size: 79.5 MB (79530908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debe05639bd474d06ece0de01c8ad45253f6a0d3df57d0650faa8bc9a30273a0`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72bce70db9946aad23c0d69098fd49a7a01bea4ea26aa604f04f8d5e7302d41`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aafdef5005c36002e7377240148b2b28444e19ff76103314392eea812975235`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0cb8df34fa5932a039bd34e6b9eb666ba815e6336f570540070910f2f0dfecc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131007916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a853159ca8430d2f1457531002aabc04746262c7f8519a56be9bdbf56643b686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 22:45:40 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 22:45:46 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 22:45:51 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 22:45:53 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 22:45:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:46:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:47:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:47:53 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:47:55 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:47:55 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:48:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 22:48:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:48:16 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:48:21 GMT
CMD ["mysqld"]
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
	-	`sha256:2dfbca3f713e45cb1092bb18734cb78402e35df75f52e8bdeaf06ed0f1ebd888`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df6abbc14fcfef5098b57bcc1adc0393ecc970dfc7b94431c9809d266cc2b81`  
		Last Modified: Thu, 03 Mar 2022 23:00:06 GMT  
		Size: 84.8 MB (84791731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb010ed7c71ddbd9adb409057a1ce179d5030e28043a9658ee8ceb5c9ed1fec`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903caa29bc7dc4bfcc6cc5f265f9b197eef44a12ba54ce57d3331a6fe1cf6f6d`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19e23161548f9dd24a7b0304af45d94ac95973dd3b0bcf241c6ab7da32f1892`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:ebcb6e992ef604e1bd754f8ee811d9a510364fb46d2afaeac745db3d7d946ef1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:a99416d1864bc3b4bce8e9031f35b78d3b6d3304818e8bea96b935874fde90ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120118799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f52c14d4e09c22dbccea6d1ee1632e0b39fb3d356351265c680fbc044ae3687`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Fri, 04 Mar 2022 01:33:34 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 04 Mar 2022 01:33:35 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 04 Mar 2022 01:33:35 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 04 Mar 2022 01:33:35 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 04 Mar 2022 01:33:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:33:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:34:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:34:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:34:02 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:34:02 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:34:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 04 Mar 2022 01:34:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:34:03 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:34:03 GMT
CMD ["mysqld"]
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
	-	`sha256:4021fab8a340817d46cf77acd03ca874abb79e76e9316e95ae29fde940f83e1c`  
		Last Modified: Fri, 04 Mar 2022 01:39:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0249ad56f65a484c68b786f772095ca981050aadbacf32eb5c21cfc9230568`  
		Last Modified: Fri, 04 Mar 2022 01:39:28 GMT  
		Size: 80.2 MB (80191123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac62dbc9c317cb8b2850714c929f287e639946a5f12d7a62a62a38c1fd61432`  
		Last Modified: Fri, 04 Mar 2022 01:39:17 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49439b48c7e27a9eabd3f775b8016b48fb61da8b6d9e0735199397267990904b`  
		Last Modified: Fri, 04 Mar 2022 01:39:16 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efcd95f926748a8f284072a9541986b06c61234d454deb59dc5ac3d8044f9bc0`  
		Last Modified: Fri, 04 Mar 2022 01:39:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dacd236b36bc458e4015952d4ee592e45aaae13f18bb3079b7d17f204e60eaa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117609970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b44f61379408de2bffba45aac163ca3c8c41cd099e2f3609621251a97f748a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:43:30 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 20:43:31 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 20:43:32 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 20:43:33 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 20:43:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:43:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:44:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:44:10 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:44:11 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:44:12 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:44:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 20:44:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:44:14 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:44:15 GMT
CMD ["mysqld"]
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
	-	`sha256:83dc742380af91b69fe3b91d6f26138ac74a8411226a5740719eb0d19045e0da`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0219e24c6a21d875b9f1eae501c6bbd2dbd2e261e3d92b808cec301ab1d8e1e`  
		Last Modified: Thu, 03 Mar 2022 20:50:17 GMT  
		Size: 79.5 MB (79530908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debe05639bd474d06ece0de01c8ad45253f6a0d3df57d0650faa8bc9a30273a0`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72bce70db9946aad23c0d69098fd49a7a01bea4ea26aa604f04f8d5e7302d41`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aafdef5005c36002e7377240148b2b28444e19ff76103314392eea812975235`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0cb8df34fa5932a039bd34e6b9eb666ba815e6336f570540070910f2f0dfecc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131007916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a853159ca8430d2f1457531002aabc04746262c7f8519a56be9bdbf56643b686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 22:45:40 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 22:45:46 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 22:45:51 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 22:45:53 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 22:45:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:46:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:47:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:47:53 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:47:55 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:47:55 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:48:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 22:48:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:48:16 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:48:21 GMT
CMD ["mysqld"]
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
	-	`sha256:2dfbca3f713e45cb1092bb18734cb78402e35df75f52e8bdeaf06ed0f1ebd888`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df6abbc14fcfef5098b57bcc1adc0393ecc970dfc7b94431c9809d266cc2b81`  
		Last Modified: Thu, 03 Mar 2022 23:00:06 GMT  
		Size: 84.8 MB (84791731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb010ed7c71ddbd9adb409057a1ce179d5030e28043a9658ee8ceb5c9ed1fec`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903caa29bc7dc4bfcc6cc5f265f9b197eef44a12ba54ce57d3331a6fe1cf6f6d`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19e23161548f9dd24a7b0304af45d94ac95973dd3b0bcf241c6ab7da32f1892`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.34`

```console
$ docker pull mariadb@sha256:ebcb6e992ef604e1bd754f8ee811d9a510364fb46d2afaeac745db3d7d946ef1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.34` - linux; amd64

```console
$ docker pull mariadb@sha256:a99416d1864bc3b4bce8e9031f35b78d3b6d3304818e8bea96b935874fde90ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120118799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f52c14d4e09c22dbccea6d1ee1632e0b39fb3d356351265c680fbc044ae3687`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Fri, 04 Mar 2022 01:33:34 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 04 Mar 2022 01:33:35 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 04 Mar 2022 01:33:35 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 04 Mar 2022 01:33:35 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 04 Mar 2022 01:33:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:33:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:34:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:34:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:34:02 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:34:02 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:34:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 04 Mar 2022 01:34:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:34:03 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:34:03 GMT
CMD ["mysqld"]
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
	-	`sha256:4021fab8a340817d46cf77acd03ca874abb79e76e9316e95ae29fde940f83e1c`  
		Last Modified: Fri, 04 Mar 2022 01:39:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0249ad56f65a484c68b786f772095ca981050aadbacf32eb5c21cfc9230568`  
		Last Modified: Fri, 04 Mar 2022 01:39:28 GMT  
		Size: 80.2 MB (80191123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac62dbc9c317cb8b2850714c929f287e639946a5f12d7a62a62a38c1fd61432`  
		Last Modified: Fri, 04 Mar 2022 01:39:17 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49439b48c7e27a9eabd3f775b8016b48fb61da8b6d9e0735199397267990904b`  
		Last Modified: Fri, 04 Mar 2022 01:39:16 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efcd95f926748a8f284072a9541986b06c61234d454deb59dc5ac3d8044f9bc0`  
		Last Modified: Fri, 04 Mar 2022 01:39:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dacd236b36bc458e4015952d4ee592e45aaae13f18bb3079b7d17f204e60eaa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117609970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b44f61379408de2bffba45aac163ca3c8c41cd099e2f3609621251a97f748a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:43:30 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 20:43:31 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 20:43:32 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 20:43:33 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 20:43:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:43:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:44:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:44:10 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:44:11 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:44:12 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:44:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 20:44:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:44:14 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:44:15 GMT
CMD ["mysqld"]
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
	-	`sha256:83dc742380af91b69fe3b91d6f26138ac74a8411226a5740719eb0d19045e0da`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0219e24c6a21d875b9f1eae501c6bbd2dbd2e261e3d92b808cec301ab1d8e1e`  
		Last Modified: Thu, 03 Mar 2022 20:50:17 GMT  
		Size: 79.5 MB (79530908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debe05639bd474d06ece0de01c8ad45253f6a0d3df57d0650faa8bc9a30273a0`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72bce70db9946aad23c0d69098fd49a7a01bea4ea26aa604f04f8d5e7302d41`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aafdef5005c36002e7377240148b2b28444e19ff76103314392eea812975235`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0cb8df34fa5932a039bd34e6b9eb666ba815e6336f570540070910f2f0dfecc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131007916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a853159ca8430d2f1457531002aabc04746262c7f8519a56be9bdbf56643b686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 22:45:40 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 22:45:46 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 22:45:51 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 22:45:53 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 22:45:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:46:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:47:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:47:53 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:47:55 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:47:55 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:48:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 22:48:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:48:16 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:48:21 GMT
CMD ["mysqld"]
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
	-	`sha256:2dfbca3f713e45cb1092bb18734cb78402e35df75f52e8bdeaf06ed0f1ebd888`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df6abbc14fcfef5098b57bcc1adc0393ecc970dfc7b94431c9809d266cc2b81`  
		Last Modified: Thu, 03 Mar 2022 23:00:06 GMT  
		Size: 84.8 MB (84791731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb010ed7c71ddbd9adb409057a1ce179d5030e28043a9658ee8ceb5c9ed1fec`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903caa29bc7dc4bfcc6cc5f265f9b197eef44a12ba54ce57d3331a6fe1cf6f6d`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19e23161548f9dd24a7b0304af45d94ac95973dd3b0bcf241c6ab7da32f1892`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.34-focal`

```console
$ docker pull mariadb@sha256:ebcb6e992ef604e1bd754f8ee811d9a510364fb46d2afaeac745db3d7d946ef1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.34-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:a99416d1864bc3b4bce8e9031f35b78d3b6d3304818e8bea96b935874fde90ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120118799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f52c14d4e09c22dbccea6d1ee1632e0b39fb3d356351265c680fbc044ae3687`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Fri, 04 Mar 2022 01:33:34 GMT
ARG MARIADB_MAJOR=10.3
# Fri, 04 Mar 2022 01:33:35 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 04 Mar 2022 01:33:35 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 04 Mar 2022 01:33:35 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Fri, 04 Mar 2022 01:33:35 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:33:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:34:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:34:02 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:34:02 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:34:02 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:34:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 04 Mar 2022 01:34:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:34:03 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:34:03 GMT
CMD ["mysqld"]
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
	-	`sha256:4021fab8a340817d46cf77acd03ca874abb79e76e9316e95ae29fde940f83e1c`  
		Last Modified: Fri, 04 Mar 2022 01:39:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0249ad56f65a484c68b786f772095ca981050aadbacf32eb5c21cfc9230568`  
		Last Modified: Fri, 04 Mar 2022 01:39:28 GMT  
		Size: 80.2 MB (80191123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac62dbc9c317cb8b2850714c929f287e639946a5f12d7a62a62a38c1fd61432`  
		Last Modified: Fri, 04 Mar 2022 01:39:17 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49439b48c7e27a9eabd3f775b8016b48fb61da8b6d9e0735199397267990904b`  
		Last Modified: Fri, 04 Mar 2022 01:39:16 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efcd95f926748a8f284072a9541986b06c61234d454deb59dc5ac3d8044f9bc0`  
		Last Modified: Fri, 04 Mar 2022 01:39:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dacd236b36bc458e4015952d4ee592e45aaae13f18bb3079b7d17f204e60eaa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117609970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b44f61379408de2bffba45aac163ca3c8c41cd099e2f3609621251a97f748a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:43:30 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 20:43:31 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 20:43:32 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 20:43:33 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 20:43:34 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:43:35 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:44:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:44:10 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:44:11 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:44:12 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:44:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 20:44:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:44:14 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:44:15 GMT
CMD ["mysqld"]
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
	-	`sha256:83dc742380af91b69fe3b91d6f26138ac74a8411226a5740719eb0d19045e0da`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0219e24c6a21d875b9f1eae501c6bbd2dbd2e261e3d92b808cec301ab1d8e1e`  
		Last Modified: Thu, 03 Mar 2022 20:50:17 GMT  
		Size: 79.5 MB (79530908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debe05639bd474d06ece0de01c8ad45253f6a0d3df57d0650faa8bc9a30273a0`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72bce70db9946aad23c0d69098fd49a7a01bea4ea26aa604f04f8d5e7302d41`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aafdef5005c36002e7377240148b2b28444e19ff76103314392eea812975235`  
		Last Modified: Thu, 03 Mar 2022 20:50:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0cb8df34fa5932a039bd34e6b9eb666ba815e6336f570540070910f2f0dfecc7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131007916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a853159ca8430d2f1457531002aabc04746262c7f8519a56be9bdbf56643b686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 22:45:40 GMT
ARG MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 22:45:46 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 03 Mar 2022 22:45:51 GMT
ARG MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 22:45:53 GMT
ENV MARIADB_VERSION=1:10.3.34+maria~focal
# Thu, 03 Mar 2022 22:45:56 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:46:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:47:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:47:53 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:47:55 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:47:55 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:48:06 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 22:48:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:48:16 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:48:21 GMT
CMD ["mysqld"]
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
	-	`sha256:2dfbca3f713e45cb1092bb18734cb78402e35df75f52e8bdeaf06ed0f1ebd888`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df6abbc14fcfef5098b57bcc1adc0393ecc970dfc7b94431c9809d266cc2b81`  
		Last Modified: Thu, 03 Mar 2022 23:00:06 GMT  
		Size: 84.8 MB (84791731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb010ed7c71ddbd9adb409057a1ce179d5030e28043a9658ee8ceb5c9ed1fec`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903caa29bc7dc4bfcc6cc5f265f9b197eef44a12ba54ce57d3331a6fe1cf6f6d`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19e23161548f9dd24a7b0304af45d94ac95973dd3b0bcf241c6ab7da32f1892`  
		Last Modified: Thu, 03 Mar 2022 22:59:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:a877d885e60014fed237a51dbf984c57ff198ea847a7fdd279152685a045b7d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:9e5eebb45bc37ac6f75ce81e75e3ae6afa7575952943ade393a37167ee5f597b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125680334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e123194a0569e8ff701b7d0069ecaca8fedb067a43662a81684140342f8d4e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Fri, 04 Mar 2022 01:32:25 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 04 Mar 2022 01:32:26 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 04 Mar 2022 01:32:26 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 04 Mar 2022 01:32:26 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 04 Mar 2022 01:32:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:32:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:33:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:33:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:33:21 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:33:21 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:33:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 04 Mar 2022 01:33:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:33:21 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:33:22 GMT
CMD ["mysqld"]
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
	-	`sha256:760ed87f68aef4740c38d9c540d7f763581b56a04e6946fbb37682d4d2dc72bd`  
		Last Modified: Fri, 04 Mar 2022 01:38:47 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e908c8b8ede8a591b73046a93dde1771c9c68ce423515608209f604bc4bfc7df`  
		Last Modified: Fri, 04 Mar 2022 01:38:59 GMT  
		Size: 85.8 MB (85752658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ded44b111024245c21ee35f6da29de369c670220aff5e9eb8cf551fb5cd92a`  
		Last Modified: Fri, 04 Mar 2022 01:38:46 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c45211f764202babc2db2e6906a0766869a04b599d2f128311f312d1d895d9`  
		Last Modified: Fri, 04 Mar 2022 01:38:46 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e49ad40a430b9bba97e4982275b90e444dc5d1edd4dc3dadbc4612f06992f`  
		Last Modified: Fri, 04 Mar 2022 01:38:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:49b9acdfe1baacb3b637f347665b9aa6ec6ddb86dc6e689ef139669d98e606c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123004813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c022054000b7e1463de40e0c6f3a5de6529f40154979f59bc402437a40c6aaeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:42:38 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 20:42:39 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 20:42:40 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 20:42:41 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 20:42:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:42:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:43:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:43:13 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:43:15 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:43:16 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:43:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 20:43:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:43:18 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:43:19 GMT
CMD ["mysqld"]
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
	-	`sha256:f9ac1f4f7e9b468c3eeb65444dbab35dd4ca154d8b8e9357f318ef6b6c0bd9f1`  
		Last Modified: Thu, 03 Mar 2022 20:49:31 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f6cc828d96d68421bdea1c0a09ac891c6ac3a29a97e650051d1935b0343d7e`  
		Last Modified: Thu, 03 Mar 2022 20:49:45 GMT  
		Size: 84.9 MB (84925755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5755a535927e3186875d9f15c2d2b56fec60cc6175fcc34dc1d4a1a90161f1b3`  
		Last Modified: Thu, 03 Mar 2022 20:49:31 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b081d1ed0ba60f64f57890e773e532d767f0ca97499e2b45c86b168936fee9f`  
		Last Modified: Thu, 03 Mar 2022 20:49:31 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccb453194a3773b32c344aa6fbef45b447de70a88b870154cd29e8546c2e39c`  
		Last Modified: Thu, 03 Mar 2022 20:49:32 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6f80e519a618856c8e77c42c646846932e6b344dd9234adb545800270a8efa21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136562220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2653adb8f09b70c75d50a80c051260088b8a8cc643e6bc68ca61f1d2e11710d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 22:42:39 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 22:42:42 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 22:42:44 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 22:42:46 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 22:42:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:42:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:44:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:45:02 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:45:04 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:45:05 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:45:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 22:45:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:45:17 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:45:24 GMT
CMD ["mysqld"]
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
	-	`sha256:09c324b785747d19072d8db31b45ce9e654691c5e679a165eab222c48f5f0d97`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30d5b8161bd3b9323f9ba25e25de30d2b710c3c68e32e56e7f26fea0d057c40`  
		Last Modified: Thu, 03 Mar 2022 22:59:28 GMT  
		Size: 90.3 MB (90346036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8049e6856df33d33c730ae35bf5ca620ca8b1e535fae7cb046331969ef8ef21`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a490775690683b38a3c3fd84d79024d18d8074532943f478571a4a10bd22767`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6f60e94c55b6a5e56fb8608f7511f45682c23273f2ae066c506164e0e95ed`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:a877d885e60014fed237a51dbf984c57ff198ea847a7fdd279152685a045b7d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:9e5eebb45bc37ac6f75ce81e75e3ae6afa7575952943ade393a37167ee5f597b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125680334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e123194a0569e8ff701b7d0069ecaca8fedb067a43662a81684140342f8d4e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Fri, 04 Mar 2022 01:32:25 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 04 Mar 2022 01:32:26 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 04 Mar 2022 01:32:26 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 04 Mar 2022 01:32:26 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 04 Mar 2022 01:32:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:32:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:33:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:33:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:33:21 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:33:21 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:33:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 04 Mar 2022 01:33:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:33:21 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:33:22 GMT
CMD ["mysqld"]
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
	-	`sha256:760ed87f68aef4740c38d9c540d7f763581b56a04e6946fbb37682d4d2dc72bd`  
		Last Modified: Fri, 04 Mar 2022 01:38:47 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e908c8b8ede8a591b73046a93dde1771c9c68ce423515608209f604bc4bfc7df`  
		Last Modified: Fri, 04 Mar 2022 01:38:59 GMT  
		Size: 85.8 MB (85752658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ded44b111024245c21ee35f6da29de369c670220aff5e9eb8cf551fb5cd92a`  
		Last Modified: Fri, 04 Mar 2022 01:38:46 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c45211f764202babc2db2e6906a0766869a04b599d2f128311f312d1d895d9`  
		Last Modified: Fri, 04 Mar 2022 01:38:46 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e49ad40a430b9bba97e4982275b90e444dc5d1edd4dc3dadbc4612f06992f`  
		Last Modified: Fri, 04 Mar 2022 01:38:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:49b9acdfe1baacb3b637f347665b9aa6ec6ddb86dc6e689ef139669d98e606c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123004813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c022054000b7e1463de40e0c6f3a5de6529f40154979f59bc402437a40c6aaeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:42:38 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 20:42:39 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 20:42:40 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 20:42:41 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 20:42:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:42:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:43:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:43:13 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:43:15 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:43:16 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:43:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 20:43:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:43:18 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:43:19 GMT
CMD ["mysqld"]
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
	-	`sha256:f9ac1f4f7e9b468c3eeb65444dbab35dd4ca154d8b8e9357f318ef6b6c0bd9f1`  
		Last Modified: Thu, 03 Mar 2022 20:49:31 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f6cc828d96d68421bdea1c0a09ac891c6ac3a29a97e650051d1935b0343d7e`  
		Last Modified: Thu, 03 Mar 2022 20:49:45 GMT  
		Size: 84.9 MB (84925755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5755a535927e3186875d9f15c2d2b56fec60cc6175fcc34dc1d4a1a90161f1b3`  
		Last Modified: Thu, 03 Mar 2022 20:49:31 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b081d1ed0ba60f64f57890e773e532d767f0ca97499e2b45c86b168936fee9f`  
		Last Modified: Thu, 03 Mar 2022 20:49:31 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccb453194a3773b32c344aa6fbef45b447de70a88b870154cd29e8546c2e39c`  
		Last Modified: Thu, 03 Mar 2022 20:49:32 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6f80e519a618856c8e77c42c646846932e6b344dd9234adb545800270a8efa21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136562220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2653adb8f09b70c75d50a80c051260088b8a8cc643e6bc68ca61f1d2e11710d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 22:42:39 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 22:42:42 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 22:42:44 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 22:42:46 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 22:42:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:42:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:44:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:45:02 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:45:04 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:45:05 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:45:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 22:45:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:45:17 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:45:24 GMT
CMD ["mysqld"]
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
	-	`sha256:09c324b785747d19072d8db31b45ce9e654691c5e679a165eab222c48f5f0d97`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30d5b8161bd3b9323f9ba25e25de30d2b710c3c68e32e56e7f26fea0d057c40`  
		Last Modified: Thu, 03 Mar 2022 22:59:28 GMT  
		Size: 90.3 MB (90346036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8049e6856df33d33c730ae35bf5ca620ca8b1e535fae7cb046331969ef8ef21`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a490775690683b38a3c3fd84d79024d18d8074532943f478571a4a10bd22767`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6f60e94c55b6a5e56fb8608f7511f45682c23273f2ae066c506164e0e95ed`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.24`

```console
$ docker pull mariadb@sha256:a877d885e60014fed237a51dbf984c57ff198ea847a7fdd279152685a045b7d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.24` - linux; amd64

```console
$ docker pull mariadb@sha256:9e5eebb45bc37ac6f75ce81e75e3ae6afa7575952943ade393a37167ee5f597b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125680334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e123194a0569e8ff701b7d0069ecaca8fedb067a43662a81684140342f8d4e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Fri, 04 Mar 2022 01:32:25 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 04 Mar 2022 01:32:26 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 04 Mar 2022 01:32:26 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 04 Mar 2022 01:32:26 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 04 Mar 2022 01:32:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:32:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:33:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:33:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:33:21 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:33:21 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:33:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 04 Mar 2022 01:33:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:33:21 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:33:22 GMT
CMD ["mysqld"]
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
	-	`sha256:760ed87f68aef4740c38d9c540d7f763581b56a04e6946fbb37682d4d2dc72bd`  
		Last Modified: Fri, 04 Mar 2022 01:38:47 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e908c8b8ede8a591b73046a93dde1771c9c68ce423515608209f604bc4bfc7df`  
		Last Modified: Fri, 04 Mar 2022 01:38:59 GMT  
		Size: 85.8 MB (85752658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ded44b111024245c21ee35f6da29de369c670220aff5e9eb8cf551fb5cd92a`  
		Last Modified: Fri, 04 Mar 2022 01:38:46 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c45211f764202babc2db2e6906a0766869a04b599d2f128311f312d1d895d9`  
		Last Modified: Fri, 04 Mar 2022 01:38:46 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e49ad40a430b9bba97e4982275b90e444dc5d1edd4dc3dadbc4612f06992f`  
		Last Modified: Fri, 04 Mar 2022 01:38:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:49b9acdfe1baacb3b637f347665b9aa6ec6ddb86dc6e689ef139669d98e606c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123004813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c022054000b7e1463de40e0c6f3a5de6529f40154979f59bc402437a40c6aaeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:42:38 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 20:42:39 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 20:42:40 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 20:42:41 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 20:42:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:42:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:43:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:43:13 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:43:15 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:43:16 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:43:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 20:43:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:43:18 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:43:19 GMT
CMD ["mysqld"]
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
	-	`sha256:f9ac1f4f7e9b468c3eeb65444dbab35dd4ca154d8b8e9357f318ef6b6c0bd9f1`  
		Last Modified: Thu, 03 Mar 2022 20:49:31 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f6cc828d96d68421bdea1c0a09ac891c6ac3a29a97e650051d1935b0343d7e`  
		Last Modified: Thu, 03 Mar 2022 20:49:45 GMT  
		Size: 84.9 MB (84925755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5755a535927e3186875d9f15c2d2b56fec60cc6175fcc34dc1d4a1a90161f1b3`  
		Last Modified: Thu, 03 Mar 2022 20:49:31 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b081d1ed0ba60f64f57890e773e532d767f0ca97499e2b45c86b168936fee9f`  
		Last Modified: Thu, 03 Mar 2022 20:49:31 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccb453194a3773b32c344aa6fbef45b447de70a88b870154cd29e8546c2e39c`  
		Last Modified: Thu, 03 Mar 2022 20:49:32 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6f80e519a618856c8e77c42c646846932e6b344dd9234adb545800270a8efa21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136562220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2653adb8f09b70c75d50a80c051260088b8a8cc643e6bc68ca61f1d2e11710d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 22:42:39 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 22:42:42 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 22:42:44 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 22:42:46 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 22:42:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:42:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:44:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:45:02 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:45:04 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:45:05 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:45:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 22:45:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:45:17 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:45:24 GMT
CMD ["mysqld"]
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
	-	`sha256:09c324b785747d19072d8db31b45ce9e654691c5e679a165eab222c48f5f0d97`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30d5b8161bd3b9323f9ba25e25de30d2b710c3c68e32e56e7f26fea0d057c40`  
		Last Modified: Thu, 03 Mar 2022 22:59:28 GMT  
		Size: 90.3 MB (90346036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8049e6856df33d33c730ae35bf5ca620ca8b1e535fae7cb046331969ef8ef21`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a490775690683b38a3c3fd84d79024d18d8074532943f478571a4a10bd22767`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6f60e94c55b6a5e56fb8608f7511f45682c23273f2ae066c506164e0e95ed`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.24-focal`

```console
$ docker pull mariadb@sha256:a877d885e60014fed237a51dbf984c57ff198ea847a7fdd279152685a045b7d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.24-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:9e5eebb45bc37ac6f75ce81e75e3ae6afa7575952943ade393a37167ee5f597b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125680334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e123194a0569e8ff701b7d0069ecaca8fedb067a43662a81684140342f8d4e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Fri, 04 Mar 2022 01:32:25 GMT
ARG MARIADB_MAJOR=10.4
# Fri, 04 Mar 2022 01:32:26 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 04 Mar 2022 01:32:26 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 04 Mar 2022 01:32:26 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Fri, 04 Mar 2022 01:32:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:32:26 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:33:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:33:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:33:21 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:33:21 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:33:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 04 Mar 2022 01:33:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:33:21 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:33:22 GMT
CMD ["mysqld"]
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
	-	`sha256:760ed87f68aef4740c38d9c540d7f763581b56a04e6946fbb37682d4d2dc72bd`  
		Last Modified: Fri, 04 Mar 2022 01:38:47 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e908c8b8ede8a591b73046a93dde1771c9c68ce423515608209f604bc4bfc7df`  
		Last Modified: Fri, 04 Mar 2022 01:38:59 GMT  
		Size: 85.8 MB (85752658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ded44b111024245c21ee35f6da29de369c670220aff5e9eb8cf551fb5cd92a`  
		Last Modified: Fri, 04 Mar 2022 01:38:46 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c45211f764202babc2db2e6906a0766869a04b599d2f128311f312d1d895d9`  
		Last Modified: Fri, 04 Mar 2022 01:38:46 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e49ad40a430b9bba97e4982275b90e444dc5d1edd4dc3dadbc4612f06992f`  
		Last Modified: Fri, 04 Mar 2022 01:38:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:49b9acdfe1baacb3b637f347665b9aa6ec6ddb86dc6e689ef139669d98e606c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123004813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c022054000b7e1463de40e0c6f3a5de6529f40154979f59bc402437a40c6aaeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:42:38 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 20:42:39 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 20:42:40 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 20:42:41 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 20:42:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:42:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:43:12 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:43:13 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:43:15 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:43:16 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:43:16 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 20:43:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:43:18 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:43:19 GMT
CMD ["mysqld"]
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
	-	`sha256:f9ac1f4f7e9b468c3eeb65444dbab35dd4ca154d8b8e9357f318ef6b6c0bd9f1`  
		Last Modified: Thu, 03 Mar 2022 20:49:31 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f6cc828d96d68421bdea1c0a09ac891c6ac3a29a97e650051d1935b0343d7e`  
		Last Modified: Thu, 03 Mar 2022 20:49:45 GMT  
		Size: 84.9 MB (84925755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5755a535927e3186875d9f15c2d2b56fec60cc6175fcc34dc1d4a1a90161f1b3`  
		Last Modified: Thu, 03 Mar 2022 20:49:31 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b081d1ed0ba60f64f57890e773e532d767f0ca97499e2b45c86b168936fee9f`  
		Last Modified: Thu, 03 Mar 2022 20:49:31 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccb453194a3773b32c344aa6fbef45b447de70a88b870154cd29e8546c2e39c`  
		Last Modified: Thu, 03 Mar 2022 20:49:32 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6f80e519a618856c8e77c42c646846932e6b344dd9234adb545800270a8efa21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136562220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2653adb8f09b70c75d50a80c051260088b8a8cc643e6bc68ca61f1d2e11710d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 22:42:39 GMT
ARG MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 22:42:42 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 03 Mar 2022 22:42:44 GMT
ARG MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 22:42:46 GMT
ENV MARIADB_VERSION=1:10.4.24+maria~focal
# Thu, 03 Mar 2022 22:42:48 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:42:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:44:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:45:02 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:45:04 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:45:05 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:45:11 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 03 Mar 2022 22:45:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:45:17 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:45:24 GMT
CMD ["mysqld"]
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
	-	`sha256:09c324b785747d19072d8db31b45ce9e654691c5e679a165eab222c48f5f0d97`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30d5b8161bd3b9323f9ba25e25de30d2b710c3c68e32e56e7f26fea0d057c40`  
		Last Modified: Thu, 03 Mar 2022 22:59:28 GMT  
		Size: 90.3 MB (90346036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8049e6856df33d33c730ae35bf5ca620ca8b1e535fae7cb046331969ef8ef21`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a490775690683b38a3c3fd84d79024d18d8074532943f478571a4a10bd22767`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6f60e94c55b6a5e56fb8608f7511f45682c23273f2ae066c506164e0e95ed`  
		Last Modified: Thu, 03 Mar 2022 22:59:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:c911279a1005ed40435962466920eafa5e55b1f5c51182086e76ccf7262b45cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:5fe9402ead3500189d4d4a6dc2d9760f9a23c0eb062a5f2e1b0c21279ca2bb3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127924075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3064294be3f0fa4c9b22629b99ae8f72ecb58c2660d8e9cac84bb8530f2e012`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Fri, 04 Mar 2022 01:31:58 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 04 Mar 2022 01:31:58 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 04 Mar 2022 01:31:58 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 04 Mar 2022 01:31:58 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 04 Mar 2022 01:31:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:31:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:32:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:32:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:32:21 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:32:21 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:32:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:32:21 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:32:21 GMT
CMD ["mysqld"]
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
	-	`sha256:f0a4e0b44fcfe18fa5a9d7589f1fc5bd75475368785ba75c50a3f7a328a31f2e`  
		Last Modified: Fri, 04 Mar 2022 01:38:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bfedcbd3213cc1eed42a479958c112f125381e679515efdbf06e0556b419d3`  
		Last Modified: Fri, 04 Mar 2022 01:38:30 GMT  
		Size: 88.0 MB (87996522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cecff94944ea743316290b8f0cac45b29458510c8c6d0709ca30baaa50911d`  
		Last Modified: Fri, 04 Mar 2022 01:38:14 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a26e5a5e3a85365a677c7393e9b5e99641e763499e923d863aa8eb93895ff6`  
		Last Modified: Fri, 04 Mar 2022 01:38:14 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:3297dd5b0f3601e9f85e4cd5f367374f59a8de29f425f6eaa9f003d930408fe1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125188376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae50fcf92720d57c07dfdd700d94a8b17f8894f6fd5a23225c2158c506ae5475`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:41:54 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:41:55 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:41:56 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:41:57 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:41:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:41:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:42:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:42:27 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:42:29 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:42:30 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:42:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:42:31 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:42:32 GMT
CMD ["mysqld"]
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
	-	`sha256:b4d721e6fc5efce7fbbd1c36ea5a31bf6b170bc2f39f3ac5305ee6e4e6995e3d`  
		Last Modified: Thu, 03 Mar 2022 20:48:59 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807c4721435197ae088699ce96ed47699bd2bd93ea79729ce4a470ccbb5e6892`  
		Last Modified: Thu, 03 Mar 2022 20:49:13 GMT  
		Size: 87.1 MB (87109433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe9ac2833b6208f0f063e5d27fd9f5cb94950d1b67d331c9967b2cb6cf590d2`  
		Last Modified: Thu, 03 Mar 2022 20:48:59 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e29965adfb74be988cf499e8191781185f9b3fcba4d1d9eee4f292465c694d`  
		Last Modified: Thu, 03 Mar 2022 20:48:59 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:34cf705ab803ca4fe1dae15b2f9d5f1e46386edb5cec8fe4638328418d1e094a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138783487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ffd60e82fbf661808deb1b562e4891c6c051ce73c9b9cc0561a60d0da825d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 22:39:28 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 22:39:31 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 22:39:35 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 22:39:39 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 22:39:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:39:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:41:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:42:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:42:10 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:42:13 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:42:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:42:23 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:42:29 GMT
CMD ["mysqld"]
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
	-	`sha256:bc32b5b1a3e95962ab92d81ae7112b90be634990754beca8aa79509b6bf2adad`  
		Last Modified: Thu, 03 Mar 2022 22:58:31 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a462106b10b0a56368053a93118e69cfb72799c1ea6de996f46107ebe46d10`  
		Last Modified: Thu, 03 Mar 2022 22:58:49 GMT  
		Size: 92.6 MB (92567426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adba2138cb6bd5a2215370e4d35e6688cb3ec56dc15c7bcbad799c07c429b21`  
		Last Modified: Thu, 03 Mar 2022 22:58:31 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f61700cea55b4667f884ff8d62c03ce19435ed2fc86c6a795f813802e474c6`  
		Last Modified: Thu, 03 Mar 2022 22:58:31 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; s390x

```console
$ docker pull mariadb@sha256:2864c929c6ed53374eb54c6bb6c0b328e7df3a8f97cd56c538a27dbd994ad50e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127198286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:471d0bc7483c45ee37fd0c0df1c60eb09b6daece039ce1606ff1c9c2c46f19e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:27:32 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:27:32 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:27:32 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:27:32 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:27:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:27:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:27:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:27:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:27:54 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:27:54 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:27:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:27:54 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:27:54 GMT
CMD ["mysqld"]
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
	-	`sha256:7dafda56bcd5961ac47ac25c3a318ec6aef7f1d7f95354cce9a6db91844b98c3`  
		Last Modified: Thu, 03 Mar 2022 20:30:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b02aa5ff7ac6ecfb28c8f8a433a21f8bc833296f143b77eda121ef8e47b8824`  
		Last Modified: Thu, 03 Mar 2022 20:31:07 GMT  
		Size: 89.3 MB (89290007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59402275dd68159a767b4f0772a3c1fc0b12fc4967474d038bbc68d49a4e716`  
		Last Modified: Thu, 03 Mar 2022 20:30:55 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0de4b83ab3a66d2705297f0a72c4a35c88958b0b5e3cd5215b4684b61253e5c`  
		Last Modified: Thu, 03 Mar 2022 20:30:55 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:c911279a1005ed40435962466920eafa5e55b1f5c51182086e76ccf7262b45cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:5fe9402ead3500189d4d4a6dc2d9760f9a23c0eb062a5f2e1b0c21279ca2bb3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127924075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3064294be3f0fa4c9b22629b99ae8f72ecb58c2660d8e9cac84bb8530f2e012`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Fri, 04 Mar 2022 01:31:58 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 04 Mar 2022 01:31:58 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 04 Mar 2022 01:31:58 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 04 Mar 2022 01:31:58 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 04 Mar 2022 01:31:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:31:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:32:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:32:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:32:21 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:32:21 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:32:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:32:21 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:32:21 GMT
CMD ["mysqld"]
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
	-	`sha256:f0a4e0b44fcfe18fa5a9d7589f1fc5bd75475368785ba75c50a3f7a328a31f2e`  
		Last Modified: Fri, 04 Mar 2022 01:38:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bfedcbd3213cc1eed42a479958c112f125381e679515efdbf06e0556b419d3`  
		Last Modified: Fri, 04 Mar 2022 01:38:30 GMT  
		Size: 88.0 MB (87996522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cecff94944ea743316290b8f0cac45b29458510c8c6d0709ca30baaa50911d`  
		Last Modified: Fri, 04 Mar 2022 01:38:14 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a26e5a5e3a85365a677c7393e9b5e99641e763499e923d863aa8eb93895ff6`  
		Last Modified: Fri, 04 Mar 2022 01:38:14 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:3297dd5b0f3601e9f85e4cd5f367374f59a8de29f425f6eaa9f003d930408fe1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125188376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae50fcf92720d57c07dfdd700d94a8b17f8894f6fd5a23225c2158c506ae5475`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:41:54 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:41:55 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:41:56 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:41:57 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:41:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:41:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:42:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:42:27 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:42:29 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:42:30 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:42:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:42:31 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:42:32 GMT
CMD ["mysqld"]
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
	-	`sha256:b4d721e6fc5efce7fbbd1c36ea5a31bf6b170bc2f39f3ac5305ee6e4e6995e3d`  
		Last Modified: Thu, 03 Mar 2022 20:48:59 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807c4721435197ae088699ce96ed47699bd2bd93ea79729ce4a470ccbb5e6892`  
		Last Modified: Thu, 03 Mar 2022 20:49:13 GMT  
		Size: 87.1 MB (87109433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe9ac2833b6208f0f063e5d27fd9f5cb94950d1b67d331c9967b2cb6cf590d2`  
		Last Modified: Thu, 03 Mar 2022 20:48:59 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e29965adfb74be988cf499e8191781185f9b3fcba4d1d9eee4f292465c694d`  
		Last Modified: Thu, 03 Mar 2022 20:48:59 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:34cf705ab803ca4fe1dae15b2f9d5f1e46386edb5cec8fe4638328418d1e094a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138783487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ffd60e82fbf661808deb1b562e4891c6c051ce73c9b9cc0561a60d0da825d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 22:39:28 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 22:39:31 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 22:39:35 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 22:39:39 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 22:39:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:39:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:41:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:42:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:42:10 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:42:13 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:42:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:42:23 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:42:29 GMT
CMD ["mysqld"]
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
	-	`sha256:bc32b5b1a3e95962ab92d81ae7112b90be634990754beca8aa79509b6bf2adad`  
		Last Modified: Thu, 03 Mar 2022 22:58:31 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a462106b10b0a56368053a93118e69cfb72799c1ea6de996f46107ebe46d10`  
		Last Modified: Thu, 03 Mar 2022 22:58:49 GMT  
		Size: 92.6 MB (92567426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adba2138cb6bd5a2215370e4d35e6688cb3ec56dc15c7bcbad799c07c429b21`  
		Last Modified: Thu, 03 Mar 2022 22:58:31 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f61700cea55b4667f884ff8d62c03ce19435ed2fc86c6a795f813802e474c6`  
		Last Modified: Thu, 03 Mar 2022 22:58:31 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:2864c929c6ed53374eb54c6bb6c0b328e7df3a8f97cd56c538a27dbd994ad50e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127198286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:471d0bc7483c45ee37fd0c0df1c60eb09b6daece039ce1606ff1c9c2c46f19e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:27:32 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:27:32 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:27:32 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:27:32 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:27:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:27:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:27:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:27:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:27:54 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:27:54 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:27:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:27:54 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:27:54 GMT
CMD ["mysqld"]
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
	-	`sha256:7dafda56bcd5961ac47ac25c3a318ec6aef7f1d7f95354cce9a6db91844b98c3`  
		Last Modified: Thu, 03 Mar 2022 20:30:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b02aa5ff7ac6ecfb28c8f8a433a21f8bc833296f143b77eda121ef8e47b8824`  
		Last Modified: Thu, 03 Mar 2022 20:31:07 GMT  
		Size: 89.3 MB (89290007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59402275dd68159a767b4f0772a3c1fc0b12fc4967474d038bbc68d49a4e716`  
		Last Modified: Thu, 03 Mar 2022 20:30:55 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0de4b83ab3a66d2705297f0a72c4a35c88958b0b5e3cd5215b4684b61253e5c`  
		Last Modified: Thu, 03 Mar 2022 20:30:55 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.15`

```console
$ docker pull mariadb@sha256:c911279a1005ed40435962466920eafa5e55b1f5c51182086e76ccf7262b45cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.15` - linux; amd64

```console
$ docker pull mariadb@sha256:5fe9402ead3500189d4d4a6dc2d9760f9a23c0eb062a5f2e1b0c21279ca2bb3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127924075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3064294be3f0fa4c9b22629b99ae8f72ecb58c2660d8e9cac84bb8530f2e012`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Fri, 04 Mar 2022 01:31:58 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 04 Mar 2022 01:31:58 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 04 Mar 2022 01:31:58 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 04 Mar 2022 01:31:58 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 04 Mar 2022 01:31:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:31:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:32:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:32:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:32:21 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:32:21 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:32:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:32:21 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:32:21 GMT
CMD ["mysqld"]
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
	-	`sha256:f0a4e0b44fcfe18fa5a9d7589f1fc5bd75475368785ba75c50a3f7a328a31f2e`  
		Last Modified: Fri, 04 Mar 2022 01:38:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bfedcbd3213cc1eed42a479958c112f125381e679515efdbf06e0556b419d3`  
		Last Modified: Fri, 04 Mar 2022 01:38:30 GMT  
		Size: 88.0 MB (87996522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cecff94944ea743316290b8f0cac45b29458510c8c6d0709ca30baaa50911d`  
		Last Modified: Fri, 04 Mar 2022 01:38:14 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a26e5a5e3a85365a677c7393e9b5e99641e763499e923d863aa8eb93895ff6`  
		Last Modified: Fri, 04 Mar 2022 01:38:14 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:3297dd5b0f3601e9f85e4cd5f367374f59a8de29f425f6eaa9f003d930408fe1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125188376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae50fcf92720d57c07dfdd700d94a8b17f8894f6fd5a23225c2158c506ae5475`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:41:54 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:41:55 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:41:56 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:41:57 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:41:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:41:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:42:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:42:27 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:42:29 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:42:30 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:42:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:42:31 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:42:32 GMT
CMD ["mysqld"]
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
	-	`sha256:b4d721e6fc5efce7fbbd1c36ea5a31bf6b170bc2f39f3ac5305ee6e4e6995e3d`  
		Last Modified: Thu, 03 Mar 2022 20:48:59 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807c4721435197ae088699ce96ed47699bd2bd93ea79729ce4a470ccbb5e6892`  
		Last Modified: Thu, 03 Mar 2022 20:49:13 GMT  
		Size: 87.1 MB (87109433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe9ac2833b6208f0f063e5d27fd9f5cb94950d1b67d331c9967b2cb6cf590d2`  
		Last Modified: Thu, 03 Mar 2022 20:48:59 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e29965adfb74be988cf499e8191781185f9b3fcba4d1d9eee4f292465c694d`  
		Last Modified: Thu, 03 Mar 2022 20:48:59 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; ppc64le

```console
$ docker pull mariadb@sha256:34cf705ab803ca4fe1dae15b2f9d5f1e46386edb5cec8fe4638328418d1e094a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138783487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ffd60e82fbf661808deb1b562e4891c6c051ce73c9b9cc0561a60d0da825d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 22:39:28 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 22:39:31 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 22:39:35 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 22:39:39 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 22:39:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:39:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:41:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:42:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:42:10 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:42:13 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:42:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:42:23 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:42:29 GMT
CMD ["mysqld"]
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
	-	`sha256:bc32b5b1a3e95962ab92d81ae7112b90be634990754beca8aa79509b6bf2adad`  
		Last Modified: Thu, 03 Mar 2022 22:58:31 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a462106b10b0a56368053a93118e69cfb72799c1ea6de996f46107ebe46d10`  
		Last Modified: Thu, 03 Mar 2022 22:58:49 GMT  
		Size: 92.6 MB (92567426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adba2138cb6bd5a2215370e4d35e6688cb3ec56dc15c7bcbad799c07c429b21`  
		Last Modified: Thu, 03 Mar 2022 22:58:31 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f61700cea55b4667f884ff8d62c03ce19435ed2fc86c6a795f813802e474c6`  
		Last Modified: Thu, 03 Mar 2022 22:58:31 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; s390x

```console
$ docker pull mariadb@sha256:2864c929c6ed53374eb54c6bb6c0b328e7df3a8f97cd56c538a27dbd994ad50e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127198286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:471d0bc7483c45ee37fd0c0df1c60eb09b6daece039ce1606ff1c9c2c46f19e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:27:32 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:27:32 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:27:32 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:27:32 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:27:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:27:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:27:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:27:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:27:54 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:27:54 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:27:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:27:54 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:27:54 GMT
CMD ["mysqld"]
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
	-	`sha256:7dafda56bcd5961ac47ac25c3a318ec6aef7f1d7f95354cce9a6db91844b98c3`  
		Last Modified: Thu, 03 Mar 2022 20:30:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b02aa5ff7ac6ecfb28c8f8a433a21f8bc833296f143b77eda121ef8e47b8824`  
		Last Modified: Thu, 03 Mar 2022 20:31:07 GMT  
		Size: 89.3 MB (89290007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59402275dd68159a767b4f0772a3c1fc0b12fc4967474d038bbc68d49a4e716`  
		Last Modified: Thu, 03 Mar 2022 20:30:55 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0de4b83ab3a66d2705297f0a72c4a35c88958b0b5e3cd5215b4684b61253e5c`  
		Last Modified: Thu, 03 Mar 2022 20:30:55 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.15-focal`

```console
$ docker pull mariadb@sha256:c911279a1005ed40435962466920eafa5e55b1f5c51182086e76ccf7262b45cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.15-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:5fe9402ead3500189d4d4a6dc2d9760f9a23c0eb062a5f2e1b0c21279ca2bb3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127924075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3064294be3f0fa4c9b22629b99ae8f72ecb58c2660d8e9cac84bb8530f2e012`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Fri, 04 Mar 2022 01:31:58 GMT
ARG MARIADB_MAJOR=10.5
# Fri, 04 Mar 2022 01:31:58 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 04 Mar 2022 01:31:58 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 04 Mar 2022 01:31:58 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Fri, 04 Mar 2022 01:31:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:31:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:32:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:32:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:32:21 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:32:21 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:32:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:32:21 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:32:21 GMT
CMD ["mysqld"]
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
	-	`sha256:f0a4e0b44fcfe18fa5a9d7589f1fc5bd75475368785ba75c50a3f7a328a31f2e`  
		Last Modified: Fri, 04 Mar 2022 01:38:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bfedcbd3213cc1eed42a479958c112f125381e679515efdbf06e0556b419d3`  
		Last Modified: Fri, 04 Mar 2022 01:38:30 GMT  
		Size: 88.0 MB (87996522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cecff94944ea743316290b8f0cac45b29458510c8c6d0709ca30baaa50911d`  
		Last Modified: Fri, 04 Mar 2022 01:38:14 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a26e5a5e3a85365a677c7393e9b5e99641e763499e923d863aa8eb93895ff6`  
		Last Modified: Fri, 04 Mar 2022 01:38:14 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:3297dd5b0f3601e9f85e4cd5f367374f59a8de29f425f6eaa9f003d930408fe1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125188376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae50fcf92720d57c07dfdd700d94a8b17f8894f6fd5a23225c2158c506ae5475`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:41:54 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:41:55 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:41:56 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:41:57 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:41:58 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:41:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:42:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:42:27 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:42:29 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:42:30 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:42:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:42:31 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:42:32 GMT
CMD ["mysqld"]
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
	-	`sha256:b4d721e6fc5efce7fbbd1c36ea5a31bf6b170bc2f39f3ac5305ee6e4e6995e3d`  
		Last Modified: Thu, 03 Mar 2022 20:48:59 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807c4721435197ae088699ce96ed47699bd2bd93ea79729ce4a470ccbb5e6892`  
		Last Modified: Thu, 03 Mar 2022 20:49:13 GMT  
		Size: 87.1 MB (87109433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe9ac2833b6208f0f063e5d27fd9f5cb94950d1b67d331c9967b2cb6cf590d2`  
		Last Modified: Thu, 03 Mar 2022 20:48:59 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e29965adfb74be988cf499e8191781185f9b3fcba4d1d9eee4f292465c694d`  
		Last Modified: Thu, 03 Mar 2022 20:48:59 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:34cf705ab803ca4fe1dae15b2f9d5f1e46386edb5cec8fe4638328418d1e094a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138783487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85ffd60e82fbf661808deb1b562e4891c6c051ce73c9b9cc0561a60d0da825d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 22:39:28 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 22:39:31 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 22:39:35 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 22:39:39 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 22:39:42 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:39:51 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:41:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:42:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:42:10 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:42:13 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:42:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:42:23 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:42:29 GMT
CMD ["mysqld"]
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
	-	`sha256:bc32b5b1a3e95962ab92d81ae7112b90be634990754beca8aa79509b6bf2adad`  
		Last Modified: Thu, 03 Mar 2022 22:58:31 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a462106b10b0a56368053a93118e69cfb72799c1ea6de996f46107ebe46d10`  
		Last Modified: Thu, 03 Mar 2022 22:58:49 GMT  
		Size: 92.6 MB (92567426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adba2138cb6bd5a2215370e4d35e6688cb3ec56dc15c7bcbad799c07c429b21`  
		Last Modified: Thu, 03 Mar 2022 22:58:31 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f61700cea55b4667f884ff8d62c03ce19435ed2fc86c6a795f813802e474c6`  
		Last Modified: Thu, 03 Mar 2022 22:58:31 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:2864c929c6ed53374eb54c6bb6c0b328e7df3a8f97cd56c538a27dbd994ad50e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127198286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:471d0bc7483c45ee37fd0c0df1c60eb09b6daece039ce1606ff1c9c2c46f19e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

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
# Thu, 03 Mar 2022 20:27:32 GMT
ARG MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:27:32 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 03 Mar 2022 20:27:32 GMT
ARG MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:27:32 GMT
ENV MARIADB_VERSION=1:10.5.15+maria~focal
# Thu, 03 Mar 2022 20:27:32 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:27:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:27:50 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.5.15/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:27:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:27:54 GMT
COPY file:ce532f6a17eccaa5fe9b3ea2a12e11efb381940167405d65a5d17184d08c3e52 in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:27:54 GMT
COPY file:05f3e2611ebac993f6f8674a52f9b7cf554603c70791f023bb7786ec99a3e34d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:27:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:27:54 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:27:54 GMT
CMD ["mysqld"]
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
	-	`sha256:7dafda56bcd5961ac47ac25c3a318ec6aef7f1d7f95354cce9a6db91844b98c3`  
		Last Modified: Thu, 03 Mar 2022 20:30:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b02aa5ff7ac6ecfb28c8f8a433a21f8bc833296f143b77eda121ef8e47b8824`  
		Last Modified: Thu, 03 Mar 2022 20:31:07 GMT  
		Size: 89.3 MB (89290007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59402275dd68159a767b4f0772a3c1fc0b12fc4967474d038bbc68d49a4e716`  
		Last Modified: Thu, 03 Mar 2022 20:30:55 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0de4b83ab3a66d2705297f0a72c4a35c88958b0b5e3cd5215b4684b61253e5c`  
		Last Modified: Thu, 03 Mar 2022 20:30:55 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:12b9c4f245768f8da658e6522e997c71a2e552a46706385d506c11f54adef251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:e03977921dd2db626ecaf2b4532d94ad751c9582c414185e50d2bb97384d892d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128170997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:620b63fe38917f03bb4112d5b054b56a6c53c81bac2c9cc97cabdd27b0829ca7`
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
# Fri, 04 Mar 2022 01:31:30 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 04 Mar 2022 01:31:30 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 04 Mar 2022 01:31:30 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 04 Mar 2022 01:31:30 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 04 Mar 2022 01:31:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:31:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:31:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:31:52 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:31:52 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:31:52 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:31:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:31:53 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:31:53 GMT
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
	-	`sha256:826648ee598623517d0d7220f84d08e06083c241d2ed18ec3b2e58a6a65ab139`  
		Last Modified: Fri, 04 Mar 2022 01:37:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a4e8c445a8ab5cc95b8aac3be489186967339b501f008b32ac5e6afe2b5bb2`  
		Last Modified: Fri, 04 Mar 2022 01:37:58 GMT  
		Size: 88.2 MB (88243434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26185829be6c3515418d5d67d4a029d15449a406c1caf040b7fb2b1dabfb9732`  
		Last Modified: Fri, 04 Mar 2022 01:37:45 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fbe2843af9a80080db2616e300901f07b2e316ceae114ef73944b273ef0b78`  
		Last Modified: Fri, 04 Mar 2022 01:37:45 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2e63655d3dcda10398a00fe59c1449639c6d327e874b1b535c38ed96e291cd5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125272295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4becc48f1267a03af39174241e1b363a2751aae95467135aa4272dca37b628`
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
# Thu, 03 Mar 2022 20:40:53 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:40:54 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:40:55 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:40:56 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:40:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:40:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:41:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:41:43 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:41:45 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:41:46 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:41:47 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:41:48 GMT
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
	-	`sha256:5e27f8ed6152cf5948fe3a9e969d85b0440accb551ac54d6f0af0ddd93ff2ae0`  
		Last Modified: Thu, 03 Mar 2022 20:48:28 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fffed44945c62c5aa8ea9a28442be6b0d6ce971d64af292d8a32c87d6d29cd`  
		Last Modified: Thu, 03 Mar 2022 20:48:41 GMT  
		Size: 87.2 MB (87193340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f2291bce3188e6f8c5b57f69b0e91a7944464e3aa6788a52a26e4156008151`  
		Last Modified: Thu, 03 Mar 2022 20:48:28 GMT  
		Size: 3.5 KB (3499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3f567c5523a194e3e6a89b6da2722e7b0320de83187349eb59ec0bf85963ae`  
		Last Modified: Thu, 03 Mar 2022 20:48:28 GMT  
		Size: 6.6 KB (6613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f758537ac96c70413a7b1d14fe10304ecddf5b2d0a8538039ecd8c5ec6652892
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138843558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a24184cb912c166a8ad69bb7ca78ec86a2c2f1057e237b2707978a96312c2bf4`
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
# Thu, 03 Mar 2022 22:36:18 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 22:36:20 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 22:36:23 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 22:36:25 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 22:36:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:36:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:38:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:39:00 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:39:01 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:39:02 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:39:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:39:13 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:39:18 GMT
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
	-	`sha256:71cb363fe09ede4ac2b79683b784ca486daa6e2a04ee625f17b456ac62d12546`  
		Last Modified: Thu, 03 Mar 2022 22:57:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c687de9d44db628292beb2f67ca3a28ef4e33417873895f10fd910aa4083fc`  
		Last Modified: Thu, 03 Mar 2022 22:58:08 GMT  
		Size: 92.6 MB (92627492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58bbd1f4ea5a77ec482b3bc6a9255482bc9965ab89ee911a94521a309f1492d`  
		Last Modified: Thu, 03 Mar 2022 22:57:51 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ad299176fed6dc1af9521a6ac06a6b27fcc1203061ae8c69440ad625128d76`  
		Last Modified: Thu, 03 Mar 2022 22:57:51 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; s390x

```console
$ docker pull mariadb@sha256:879031c66c9bd9d8de98d92923bb19d54b0607d95e968738a942b8a936448d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127224463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef9a724a160577a9a2fb30b256b5c70fe9904bba2ee32632646c62c1cd5a15f8`
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
# Thu, 03 Mar 2022 20:27:00 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:27:00 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:27:00 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:27:01 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:27:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:27:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:27:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:27:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:27:24 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:27:24 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:27:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:27:25 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:27:25 GMT
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
	-	`sha256:abf2eee58f1bbc8fb38adf7d1c9e23cb1e7907e5a9d2d92a8972c5c9a4dc5902`  
		Last Modified: Thu, 03 Mar 2022 20:30:03 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c40cb2a4b9cd0cf70c8910f4c2e49c3ac9c2b4c967fc0b6747a4840c6116866`  
		Last Modified: Thu, 03 Mar 2022 20:30:16 GMT  
		Size: 89.3 MB (89316186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb294697e222af0ffdd191b4feaac5f8594b6122bc5ffd3ae6d8428cab91572`  
		Last Modified: Thu, 03 Mar 2022 20:30:03 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e7c77a9f5f140a834508d363d71ef86a567a96b5d395efca67a62484cff44d`  
		Last Modified: Thu, 03 Mar 2022 20:30:04 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:12b9c4f245768f8da658e6522e997c71a2e552a46706385d506c11f54adef251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:e03977921dd2db626ecaf2b4532d94ad751c9582c414185e50d2bb97384d892d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128170997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:620b63fe38917f03bb4112d5b054b56a6c53c81bac2c9cc97cabdd27b0829ca7`
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
# Fri, 04 Mar 2022 01:31:30 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 04 Mar 2022 01:31:30 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 04 Mar 2022 01:31:30 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 04 Mar 2022 01:31:30 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 04 Mar 2022 01:31:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:31:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:31:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:31:52 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:31:52 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:31:52 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:31:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:31:53 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:31:53 GMT
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
	-	`sha256:826648ee598623517d0d7220f84d08e06083c241d2ed18ec3b2e58a6a65ab139`  
		Last Modified: Fri, 04 Mar 2022 01:37:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a4e8c445a8ab5cc95b8aac3be489186967339b501f008b32ac5e6afe2b5bb2`  
		Last Modified: Fri, 04 Mar 2022 01:37:58 GMT  
		Size: 88.2 MB (88243434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26185829be6c3515418d5d67d4a029d15449a406c1caf040b7fb2b1dabfb9732`  
		Last Modified: Fri, 04 Mar 2022 01:37:45 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fbe2843af9a80080db2616e300901f07b2e316ceae114ef73944b273ef0b78`  
		Last Modified: Fri, 04 Mar 2022 01:37:45 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2e63655d3dcda10398a00fe59c1449639c6d327e874b1b535c38ed96e291cd5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125272295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4becc48f1267a03af39174241e1b363a2751aae95467135aa4272dca37b628`
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
# Thu, 03 Mar 2022 20:40:53 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:40:54 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:40:55 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:40:56 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:40:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:40:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:41:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:41:43 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:41:45 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:41:46 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:41:47 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:41:48 GMT
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
	-	`sha256:5e27f8ed6152cf5948fe3a9e969d85b0440accb551ac54d6f0af0ddd93ff2ae0`  
		Last Modified: Thu, 03 Mar 2022 20:48:28 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fffed44945c62c5aa8ea9a28442be6b0d6ce971d64af292d8a32c87d6d29cd`  
		Last Modified: Thu, 03 Mar 2022 20:48:41 GMT  
		Size: 87.2 MB (87193340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f2291bce3188e6f8c5b57f69b0e91a7944464e3aa6788a52a26e4156008151`  
		Last Modified: Thu, 03 Mar 2022 20:48:28 GMT  
		Size: 3.5 KB (3499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3f567c5523a194e3e6a89b6da2722e7b0320de83187349eb59ec0bf85963ae`  
		Last Modified: Thu, 03 Mar 2022 20:48:28 GMT  
		Size: 6.6 KB (6613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f758537ac96c70413a7b1d14fe10304ecddf5b2d0a8538039ecd8c5ec6652892
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138843558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a24184cb912c166a8ad69bb7ca78ec86a2c2f1057e237b2707978a96312c2bf4`
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
# Thu, 03 Mar 2022 22:36:18 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 22:36:20 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 22:36:23 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 22:36:25 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 22:36:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:36:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:38:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:39:00 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:39:01 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:39:02 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:39:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:39:13 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:39:18 GMT
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
	-	`sha256:71cb363fe09ede4ac2b79683b784ca486daa6e2a04ee625f17b456ac62d12546`  
		Last Modified: Thu, 03 Mar 2022 22:57:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c687de9d44db628292beb2f67ca3a28ef4e33417873895f10fd910aa4083fc`  
		Last Modified: Thu, 03 Mar 2022 22:58:08 GMT  
		Size: 92.6 MB (92627492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58bbd1f4ea5a77ec482b3bc6a9255482bc9965ab89ee911a94521a309f1492d`  
		Last Modified: Thu, 03 Mar 2022 22:57:51 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ad299176fed6dc1af9521a6ac06a6b27fcc1203061ae8c69440ad625128d76`  
		Last Modified: Thu, 03 Mar 2022 22:57:51 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:879031c66c9bd9d8de98d92923bb19d54b0607d95e968738a942b8a936448d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127224463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef9a724a160577a9a2fb30b256b5c70fe9904bba2ee32632646c62c1cd5a15f8`
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
# Thu, 03 Mar 2022 20:27:00 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:27:00 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:27:00 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:27:01 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:27:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:27:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:27:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:27:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:27:24 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:27:24 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:27:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:27:25 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:27:25 GMT
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
	-	`sha256:abf2eee58f1bbc8fb38adf7d1c9e23cb1e7907e5a9d2d92a8972c5c9a4dc5902`  
		Last Modified: Thu, 03 Mar 2022 20:30:03 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c40cb2a4b9cd0cf70c8910f4c2e49c3ac9c2b4c967fc0b6747a4840c6116866`  
		Last Modified: Thu, 03 Mar 2022 20:30:16 GMT  
		Size: 89.3 MB (89316186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb294697e222af0ffdd191b4feaac5f8594b6122bc5ffd3ae6d8428cab91572`  
		Last Modified: Thu, 03 Mar 2022 20:30:03 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e7c77a9f5f140a834508d363d71ef86a567a96b5d395efca67a62484cff44d`  
		Last Modified: Thu, 03 Mar 2022 20:30:04 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.7`

```console
$ docker pull mariadb@sha256:12b9c4f245768f8da658e6522e997c71a2e552a46706385d506c11f54adef251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.7` - linux; amd64

```console
$ docker pull mariadb@sha256:e03977921dd2db626ecaf2b4532d94ad751c9582c414185e50d2bb97384d892d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128170997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:620b63fe38917f03bb4112d5b054b56a6c53c81bac2c9cc97cabdd27b0829ca7`
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
# Fri, 04 Mar 2022 01:31:30 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 04 Mar 2022 01:31:30 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 04 Mar 2022 01:31:30 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 04 Mar 2022 01:31:30 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 04 Mar 2022 01:31:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:31:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:31:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:31:52 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:31:52 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:31:52 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:31:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:31:53 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:31:53 GMT
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
	-	`sha256:826648ee598623517d0d7220f84d08e06083c241d2ed18ec3b2e58a6a65ab139`  
		Last Modified: Fri, 04 Mar 2022 01:37:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a4e8c445a8ab5cc95b8aac3be489186967339b501f008b32ac5e6afe2b5bb2`  
		Last Modified: Fri, 04 Mar 2022 01:37:58 GMT  
		Size: 88.2 MB (88243434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26185829be6c3515418d5d67d4a029d15449a406c1caf040b7fb2b1dabfb9732`  
		Last Modified: Fri, 04 Mar 2022 01:37:45 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fbe2843af9a80080db2616e300901f07b2e316ceae114ef73944b273ef0b78`  
		Last Modified: Fri, 04 Mar 2022 01:37:45 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2e63655d3dcda10398a00fe59c1449639c6d327e874b1b535c38ed96e291cd5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125272295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4becc48f1267a03af39174241e1b363a2751aae95467135aa4272dca37b628`
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
# Thu, 03 Mar 2022 20:40:53 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:40:54 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:40:55 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:40:56 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:40:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:40:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:41:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:41:43 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:41:45 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:41:46 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:41:47 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:41:48 GMT
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
	-	`sha256:5e27f8ed6152cf5948fe3a9e969d85b0440accb551ac54d6f0af0ddd93ff2ae0`  
		Last Modified: Thu, 03 Mar 2022 20:48:28 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fffed44945c62c5aa8ea9a28442be6b0d6ce971d64af292d8a32c87d6d29cd`  
		Last Modified: Thu, 03 Mar 2022 20:48:41 GMT  
		Size: 87.2 MB (87193340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f2291bce3188e6f8c5b57f69b0e91a7944464e3aa6788a52a26e4156008151`  
		Last Modified: Thu, 03 Mar 2022 20:48:28 GMT  
		Size: 3.5 KB (3499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3f567c5523a194e3e6a89b6da2722e7b0320de83187349eb59ec0bf85963ae`  
		Last Modified: Thu, 03 Mar 2022 20:48:28 GMT  
		Size: 6.6 KB (6613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f758537ac96c70413a7b1d14fe10304ecddf5b2d0a8538039ecd8c5ec6652892
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138843558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a24184cb912c166a8ad69bb7ca78ec86a2c2f1057e237b2707978a96312c2bf4`
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
# Thu, 03 Mar 2022 22:36:18 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 22:36:20 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 22:36:23 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 22:36:25 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 22:36:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:36:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:38:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:39:00 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:39:01 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:39:02 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:39:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:39:13 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:39:18 GMT
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
	-	`sha256:71cb363fe09ede4ac2b79683b784ca486daa6e2a04ee625f17b456ac62d12546`  
		Last Modified: Thu, 03 Mar 2022 22:57:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c687de9d44db628292beb2f67ca3a28ef4e33417873895f10fd910aa4083fc`  
		Last Modified: Thu, 03 Mar 2022 22:58:08 GMT  
		Size: 92.6 MB (92627492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58bbd1f4ea5a77ec482b3bc6a9255482bc9965ab89ee911a94521a309f1492d`  
		Last Modified: Thu, 03 Mar 2022 22:57:51 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ad299176fed6dc1af9521a6ac06a6b27fcc1203061ae8c69440ad625128d76`  
		Last Modified: Thu, 03 Mar 2022 22:57:51 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; s390x

```console
$ docker pull mariadb@sha256:879031c66c9bd9d8de98d92923bb19d54b0607d95e968738a942b8a936448d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127224463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef9a724a160577a9a2fb30b256b5c70fe9904bba2ee32632646c62c1cd5a15f8`
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
# Thu, 03 Mar 2022 20:27:00 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:27:00 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:27:00 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:27:01 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:27:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:27:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:27:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:27:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:27:24 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:27:24 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:27:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:27:25 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:27:25 GMT
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
	-	`sha256:abf2eee58f1bbc8fb38adf7d1c9e23cb1e7907e5a9d2d92a8972c5c9a4dc5902`  
		Last Modified: Thu, 03 Mar 2022 20:30:03 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c40cb2a4b9cd0cf70c8910f4c2e49c3ac9c2b4c967fc0b6747a4840c6116866`  
		Last Modified: Thu, 03 Mar 2022 20:30:16 GMT  
		Size: 89.3 MB (89316186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb294697e222af0ffdd191b4feaac5f8594b6122bc5ffd3ae6d8428cab91572`  
		Last Modified: Thu, 03 Mar 2022 20:30:03 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e7c77a9f5f140a834508d363d71ef86a567a96b5d395efca67a62484cff44d`  
		Last Modified: Thu, 03 Mar 2022 20:30:04 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.7-focal`

```console
$ docker pull mariadb@sha256:12b9c4f245768f8da658e6522e997c71a2e552a46706385d506c11f54adef251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:e03977921dd2db626ecaf2b4532d94ad751c9582c414185e50d2bb97384d892d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128170997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:620b63fe38917f03bb4112d5b054b56a6c53c81bac2c9cc97cabdd27b0829ca7`
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
# Fri, 04 Mar 2022 01:31:30 GMT
ARG MARIADB_MAJOR=10.6
# Fri, 04 Mar 2022 01:31:30 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 04 Mar 2022 01:31:30 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 04 Mar 2022 01:31:30 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Fri, 04 Mar 2022 01:31:30 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:31:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:31:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:31:52 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:31:52 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:31:52 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:31:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:31:53 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:31:53 GMT
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
	-	`sha256:826648ee598623517d0d7220f84d08e06083c241d2ed18ec3b2e58a6a65ab139`  
		Last Modified: Fri, 04 Mar 2022 01:37:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a4e8c445a8ab5cc95b8aac3be489186967339b501f008b32ac5e6afe2b5bb2`  
		Last Modified: Fri, 04 Mar 2022 01:37:58 GMT  
		Size: 88.2 MB (88243434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26185829be6c3515418d5d67d4a029d15449a406c1caf040b7fb2b1dabfb9732`  
		Last Modified: Fri, 04 Mar 2022 01:37:45 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fbe2843af9a80080db2616e300901f07b2e316ceae114ef73944b273ef0b78`  
		Last Modified: Fri, 04 Mar 2022 01:37:45 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2e63655d3dcda10398a00fe59c1449639c6d327e874b1b535c38ed96e291cd5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125272295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4becc48f1267a03af39174241e1b363a2751aae95467135aa4272dca37b628`
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
# Thu, 03 Mar 2022 20:40:53 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:40:54 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:40:55 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:40:56 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:40:57 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:40:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:41:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:41:43 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:41:45 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:41:46 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:41:47 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:41:48 GMT
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
	-	`sha256:5e27f8ed6152cf5948fe3a9e969d85b0440accb551ac54d6f0af0ddd93ff2ae0`  
		Last Modified: Thu, 03 Mar 2022 20:48:28 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fffed44945c62c5aa8ea9a28442be6b0d6ce971d64af292d8a32c87d6d29cd`  
		Last Modified: Thu, 03 Mar 2022 20:48:41 GMT  
		Size: 87.2 MB (87193340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f2291bce3188e6f8c5b57f69b0e91a7944464e3aa6788a52a26e4156008151`  
		Last Modified: Thu, 03 Mar 2022 20:48:28 GMT  
		Size: 3.5 KB (3499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3f567c5523a194e3e6a89b6da2722e7b0320de83187349eb59ec0bf85963ae`  
		Last Modified: Thu, 03 Mar 2022 20:48:28 GMT  
		Size: 6.6 KB (6613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f758537ac96c70413a7b1d14fe10304ecddf5b2d0a8538039ecd8c5ec6652892
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138843558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a24184cb912c166a8ad69bb7ca78ec86a2c2f1057e237b2707978a96312c2bf4`
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
# Thu, 03 Mar 2022 22:36:18 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 22:36:20 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 22:36:23 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 22:36:25 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 22:36:26 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:36:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:38:52 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:39:00 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:39:01 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:39:02 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:39:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:39:13 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:39:18 GMT
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
	-	`sha256:71cb363fe09ede4ac2b79683b784ca486daa6e2a04ee625f17b456ac62d12546`  
		Last Modified: Thu, 03 Mar 2022 22:57:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c687de9d44db628292beb2f67ca3a28ef4e33417873895f10fd910aa4083fc`  
		Last Modified: Thu, 03 Mar 2022 22:58:08 GMT  
		Size: 92.6 MB (92627492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58bbd1f4ea5a77ec482b3bc6a9255482bc9965ab89ee911a94521a309f1492d`  
		Last Modified: Thu, 03 Mar 2022 22:57:51 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ad299176fed6dc1af9521a6ac06a6b27fcc1203061ae8c69440ad625128d76`  
		Last Modified: Thu, 03 Mar 2022 22:57:51 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:879031c66c9bd9d8de98d92923bb19d54b0607d95e968738a942b8a936448d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127224463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef9a724a160577a9a2fb30b256b5c70fe9904bba2ee32632646c62c1cd5a15f8`
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
# Thu, 03 Mar 2022 20:27:00 GMT
ARG MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:27:00 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 03 Mar 2022 20:27:00 GMT
ARG MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:27:01 GMT
ENV MARIADB_VERSION=1:10.6.7+maria~focal
# Thu, 03 Mar 2022 20:27:01 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:27:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:27:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.6.7/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:27:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:27:24 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:27:24 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:27:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:27:25 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:27:25 GMT
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
	-	`sha256:abf2eee58f1bbc8fb38adf7d1c9e23cb1e7907e5a9d2d92a8972c5c9a4dc5902`  
		Last Modified: Thu, 03 Mar 2022 20:30:03 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c40cb2a4b9cd0cf70c8910f4c2e49c3ac9c2b4c967fc0b6747a4840c6116866`  
		Last Modified: Thu, 03 Mar 2022 20:30:16 GMT  
		Size: 89.3 MB (89316186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb294697e222af0ffdd191b4feaac5f8594b6122bc5ffd3ae6d8428cab91572`  
		Last Modified: Thu, 03 Mar 2022 20:30:03 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e7c77a9f5f140a834508d363d71ef86a567a96b5d395efca67a62484cff44d`  
		Last Modified: Thu, 03 Mar 2022 20:30:04 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7`

```console
$ docker pull mariadb@sha256:6b27df78e91348af6ac28e120a9d3f2852bb4c17d427365a4dad01b206616271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7` - linux; amd64

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

### `mariadb:10.7` - linux; arm64 variant v8

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

### `mariadb:10.7` - linux; ppc64le

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

### `mariadb:10.7` - linux; s390x

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

## `mariadb:10.7-focal`

```console
$ docker pull mariadb@sha256:6b27df78e91348af6ac28e120a9d3f2852bb4c17d427365a4dad01b206616271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7-focal` - linux; amd64

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

### `mariadb:10.7-focal` - linux; arm64 variant v8

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

### `mariadb:10.7-focal` - linux; ppc64le

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

### `mariadb:10.7-focal` - linux; s390x

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

## `mariadb:10.7.3`

```console
$ docker pull mariadb@sha256:6b27df78e91348af6ac28e120a9d3f2852bb4c17d427365a4dad01b206616271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.3` - linux; amd64

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

### `mariadb:10.7.3` - linux; arm64 variant v8

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

### `mariadb:10.7.3` - linux; ppc64le

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

### `mariadb:10.7.3` - linux; s390x

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

## `mariadb:10.7.3-focal`

```console
$ docker pull mariadb@sha256:6b27df78e91348af6ac28e120a9d3f2852bb4c17d427365a4dad01b206616271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.3-focal` - linux; amd64

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

### `mariadb:10.7.3-focal` - linux; arm64 variant v8

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

### `mariadb:10.7.3-focal` - linux; ppc64le

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

### `mariadb:10.7.3-focal` - linux; s390x

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

## `mariadb:10.8-rc`

```console
$ docker pull mariadb@sha256:8eab9f27188d1e613efa477a9c7025b719d457d80fd73a09cd053489c5b04eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:220bae35dd6770cb268a488960110814b3deb2c818d65f83dcbaf1ba0449aacc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128579619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3808c711286a6fe65a7224cc4303e813787a00ee6108a27831ddd6eb8ff4f0c8`
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
# Fri, 04 Mar 2022 01:30:23 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 04 Mar 2022 01:30:23 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 04 Mar 2022 01:30:23 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 04 Mar 2022 01:30:23 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 04 Mar 2022 01:30:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:30:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:30:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:30:59 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:30:59 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:30:59 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:30:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:30:59 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:30:59 GMT
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
	-	`sha256:8c1f0550683801aa881825c600927a91928ccc575970282cd543ac5bed20d3a4`  
		Last Modified: Fri, 04 Mar 2022 01:36:31 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e44e5bed9927db9168e7f1b5d07a0d779b4a72661472f1136dc1f00dbe799b`  
		Last Modified: Fri, 04 Mar 2022 01:36:44 GMT  
		Size: 88.7 MB (88652047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac1448c13b067ccb5d26f7dd1d0378b3159071054d7760aaafb6db3202abd67`  
		Last Modified: Fri, 04 Mar 2022 01:36:31 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75b107e89292a74fd8e7bf5e377bf08b057a3384a864c334a58c1f34d77ffb5`  
		Last Modified: Fri, 04 Mar 2022 01:36:31 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:fce0df6934e7a27b342669f848a370308230e8fcd776031405fd6996a2945a16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125653276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee9fd0ceee20881cb2f2d85f2b34a4d3931b5077f5d8ed0bc59f5f32be0721c`
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
# Thu, 03 Mar 2022 20:39:02 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:39:03 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:39:04 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:39:05 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:39:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:39:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:39:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:39:38 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:39:40 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:39:41 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:39:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:39:42 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:39:43 GMT
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
	-	`sha256:fb76e878d72903fa1f87e29cc101bf40d4af64d64fc741b5fadfc1448b3ed79c`  
		Last Modified: Thu, 03 Mar 2022 20:47:11 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc8dde71d68c5d7a6217dfd16d452244125cc51bfe60e632c73f0dcaf8b1934`  
		Last Modified: Thu, 03 Mar 2022 20:47:25 GMT  
		Size: 87.6 MB (87574322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3583f4dab72174751865fe88c94ea07b1f3e92bd98c24346bd8804c6f2c5b6`  
		Last Modified: Thu, 03 Mar 2022 20:47:11 GMT  
		Size: 3.5 KB (3498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c13c8d98cec102bcdd41dd21911b79072b04a83e5382c3c37cb35ae0e093bdb`  
		Last Modified: Thu, 03 Mar 2022 20:47:11 GMT  
		Size: 6.6 KB (6612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:83b3e5d13ef8cbfe2072250f8acce71c924bfe5e2060b0e702bb3d4c88a24f5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139622025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f6883935c9460538d1cde2c52a3027d2560820e710049ae54b0e8465e809eec`
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
# Thu, 03 Mar 2022 22:28:30 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 22:28:32 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 22:28:34 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 22:28:38 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 22:28:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:28:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:32:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:32:28 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:32:30 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:32:32 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:32:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:32:38 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:32:43 GMT
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
	-	`sha256:e27bb09eaee81666252b1e9c3e29aef8a1f634fd0fc222d5427dab4b5580c965`  
		Last Modified: Thu, 03 Mar 2022 22:56:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31261ff7a4ccda8ce89970b9d74fa9cae58c8aa4fff74e7f710995c1d0d2c52e`  
		Last Modified: Thu, 03 Mar 2022 22:56:33 GMT  
		Size: 93.4 MB (93405953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04eb87cb05726342287ce945c1a4d2a6e6704bf0c1c99a3dff5a1b23b56b6990`  
		Last Modified: Thu, 03 Mar 2022 22:56:16 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59de5b5b3d65537159500f65dc2fc0c1a2962a023348b762c31f406c037dd31`  
		Last Modified: Thu, 03 Mar 2022 22:56:16 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:aecfd830e8950fe21a8687609da6442161af089b5ca7d6268d38bee69b2c1aef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127688022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774c3da47e87494512f751f2ea706543d04fd29d13b58d2970a05b499df10f4f`
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
# Thu, 03 Mar 2022 20:25:53 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:25:53 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:25:53 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:25:53 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:25:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:25:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:26:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:26:18 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:26:18 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:26:18 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:26:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:26:19 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:26:19 GMT
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
	-	`sha256:5643f0cbb813dafd109d5baf0be157769503974bec4d8b5dd4cd68b30621e316`  
		Last Modified: Thu, 03 Mar 2022 20:28:45 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36078a64e944ddbea6e42aa6442ad94d4b395b8ef521b5dee2bbd11c28b27409`  
		Last Modified: Thu, 03 Mar 2022 20:28:57 GMT  
		Size: 89.8 MB (89779732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f0dd2c26918d37e8cb319e0b3c8f93d643702e26f24a02c5aa328af1833972`  
		Last Modified: Thu, 03 Mar 2022 20:28:45 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712fe50768356efec4449f3e2d95362920797b99e9aeb53fb7e6d94bd55b768a`  
		Last Modified: Thu, 03 Mar 2022 20:28:45 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8-rc-focal`

```console
$ docker pull mariadb@sha256:8eab9f27188d1e613efa477a9c7025b719d457d80fd73a09cd053489c5b04eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-rc-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:220bae35dd6770cb268a488960110814b3deb2c818d65f83dcbaf1ba0449aacc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128579619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3808c711286a6fe65a7224cc4303e813787a00ee6108a27831ddd6eb8ff4f0c8`
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
# Fri, 04 Mar 2022 01:30:23 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 04 Mar 2022 01:30:23 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 04 Mar 2022 01:30:23 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 04 Mar 2022 01:30:23 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 04 Mar 2022 01:30:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:30:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:30:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:30:59 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:30:59 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:30:59 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:30:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:30:59 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:30:59 GMT
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
	-	`sha256:8c1f0550683801aa881825c600927a91928ccc575970282cd543ac5bed20d3a4`  
		Last Modified: Fri, 04 Mar 2022 01:36:31 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e44e5bed9927db9168e7f1b5d07a0d779b4a72661472f1136dc1f00dbe799b`  
		Last Modified: Fri, 04 Mar 2022 01:36:44 GMT  
		Size: 88.7 MB (88652047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac1448c13b067ccb5d26f7dd1d0378b3159071054d7760aaafb6db3202abd67`  
		Last Modified: Fri, 04 Mar 2022 01:36:31 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75b107e89292a74fd8e7bf5e377bf08b057a3384a864c334a58c1f34d77ffb5`  
		Last Modified: Fri, 04 Mar 2022 01:36:31 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:fce0df6934e7a27b342669f848a370308230e8fcd776031405fd6996a2945a16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125653276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee9fd0ceee20881cb2f2d85f2b34a4d3931b5077f5d8ed0bc59f5f32be0721c`
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
# Thu, 03 Mar 2022 20:39:02 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:39:03 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:39:04 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:39:05 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:39:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:39:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:39:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:39:38 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:39:40 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:39:41 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:39:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:39:42 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:39:43 GMT
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
	-	`sha256:fb76e878d72903fa1f87e29cc101bf40d4af64d64fc741b5fadfc1448b3ed79c`  
		Last Modified: Thu, 03 Mar 2022 20:47:11 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc8dde71d68c5d7a6217dfd16d452244125cc51bfe60e632c73f0dcaf8b1934`  
		Last Modified: Thu, 03 Mar 2022 20:47:25 GMT  
		Size: 87.6 MB (87574322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3583f4dab72174751865fe88c94ea07b1f3e92bd98c24346bd8804c6f2c5b6`  
		Last Modified: Thu, 03 Mar 2022 20:47:11 GMT  
		Size: 3.5 KB (3498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c13c8d98cec102bcdd41dd21911b79072b04a83e5382c3c37cb35ae0e093bdb`  
		Last Modified: Thu, 03 Mar 2022 20:47:11 GMT  
		Size: 6.6 KB (6612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:83b3e5d13ef8cbfe2072250f8acce71c924bfe5e2060b0e702bb3d4c88a24f5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139622025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f6883935c9460538d1cde2c52a3027d2560820e710049ae54b0e8465e809eec`
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
# Thu, 03 Mar 2022 22:28:30 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 22:28:32 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 22:28:34 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 22:28:38 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 22:28:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:28:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:32:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:32:28 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:32:30 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:32:32 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:32:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:32:38 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:32:43 GMT
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
	-	`sha256:e27bb09eaee81666252b1e9c3e29aef8a1f634fd0fc222d5427dab4b5580c965`  
		Last Modified: Thu, 03 Mar 2022 22:56:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31261ff7a4ccda8ce89970b9d74fa9cae58c8aa4fff74e7f710995c1d0d2c52e`  
		Last Modified: Thu, 03 Mar 2022 22:56:33 GMT  
		Size: 93.4 MB (93405953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04eb87cb05726342287ce945c1a4d2a6e6704bf0c1c99a3dff5a1b23b56b6990`  
		Last Modified: Thu, 03 Mar 2022 22:56:16 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59de5b5b3d65537159500f65dc2fc0c1a2962a023348b762c31f406c037dd31`  
		Last Modified: Thu, 03 Mar 2022 22:56:16 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:aecfd830e8950fe21a8687609da6442161af089b5ca7d6268d38bee69b2c1aef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127688022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774c3da47e87494512f751f2ea706543d04fd29d13b58d2970a05b499df10f4f`
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
# Thu, 03 Mar 2022 20:25:53 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:25:53 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:25:53 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:25:53 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:25:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:25:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:26:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:26:18 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:26:18 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:26:18 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:26:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:26:19 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:26:19 GMT
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
	-	`sha256:5643f0cbb813dafd109d5baf0be157769503974bec4d8b5dd4cd68b30621e316`  
		Last Modified: Thu, 03 Mar 2022 20:28:45 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36078a64e944ddbea6e42aa6442ad94d4b395b8ef521b5dee2bbd11c28b27409`  
		Last Modified: Thu, 03 Mar 2022 20:28:57 GMT  
		Size: 89.8 MB (89779732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f0dd2c26918d37e8cb319e0b3c8f93d643702e26f24a02c5aa328af1833972`  
		Last Modified: Thu, 03 Mar 2022 20:28:45 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712fe50768356efec4449f3e2d95362920797b99e9aeb53fb7e6d94bd55b768a`  
		Last Modified: Thu, 03 Mar 2022 20:28:45 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.2-rc`

```console
$ docker pull mariadb@sha256:8eab9f27188d1e613efa477a9c7025b719d457d80fd73a09cd053489c5b04eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8.2-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:220bae35dd6770cb268a488960110814b3deb2c818d65f83dcbaf1ba0449aacc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128579619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3808c711286a6fe65a7224cc4303e813787a00ee6108a27831ddd6eb8ff4f0c8`
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
# Fri, 04 Mar 2022 01:30:23 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 04 Mar 2022 01:30:23 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 04 Mar 2022 01:30:23 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 04 Mar 2022 01:30:23 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 04 Mar 2022 01:30:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:30:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:30:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:30:59 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:30:59 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:30:59 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:30:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:30:59 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:30:59 GMT
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
	-	`sha256:8c1f0550683801aa881825c600927a91928ccc575970282cd543ac5bed20d3a4`  
		Last Modified: Fri, 04 Mar 2022 01:36:31 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e44e5bed9927db9168e7f1b5d07a0d779b4a72661472f1136dc1f00dbe799b`  
		Last Modified: Fri, 04 Mar 2022 01:36:44 GMT  
		Size: 88.7 MB (88652047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac1448c13b067ccb5d26f7dd1d0378b3159071054d7760aaafb6db3202abd67`  
		Last Modified: Fri, 04 Mar 2022 01:36:31 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75b107e89292a74fd8e7bf5e377bf08b057a3384a864c334a58c1f34d77ffb5`  
		Last Modified: Fri, 04 Mar 2022 01:36:31 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:fce0df6934e7a27b342669f848a370308230e8fcd776031405fd6996a2945a16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125653276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee9fd0ceee20881cb2f2d85f2b34a4d3931b5077f5d8ed0bc59f5f32be0721c`
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
# Thu, 03 Mar 2022 20:39:02 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:39:03 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:39:04 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:39:05 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:39:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:39:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:39:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:39:38 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:39:40 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:39:41 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:39:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:39:42 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:39:43 GMT
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
	-	`sha256:fb76e878d72903fa1f87e29cc101bf40d4af64d64fc741b5fadfc1448b3ed79c`  
		Last Modified: Thu, 03 Mar 2022 20:47:11 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc8dde71d68c5d7a6217dfd16d452244125cc51bfe60e632c73f0dcaf8b1934`  
		Last Modified: Thu, 03 Mar 2022 20:47:25 GMT  
		Size: 87.6 MB (87574322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3583f4dab72174751865fe88c94ea07b1f3e92bd98c24346bd8804c6f2c5b6`  
		Last Modified: Thu, 03 Mar 2022 20:47:11 GMT  
		Size: 3.5 KB (3498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c13c8d98cec102bcdd41dd21911b79072b04a83e5382c3c37cb35ae0e093bdb`  
		Last Modified: Thu, 03 Mar 2022 20:47:11 GMT  
		Size: 6.6 KB (6612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:83b3e5d13ef8cbfe2072250f8acce71c924bfe5e2060b0e702bb3d4c88a24f5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139622025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f6883935c9460538d1cde2c52a3027d2560820e710049ae54b0e8465e809eec`
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
# Thu, 03 Mar 2022 22:28:30 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 22:28:32 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 22:28:34 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 22:28:38 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 22:28:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:28:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:32:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:32:28 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:32:30 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:32:32 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:32:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:32:38 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:32:43 GMT
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
	-	`sha256:e27bb09eaee81666252b1e9c3e29aef8a1f634fd0fc222d5427dab4b5580c965`  
		Last Modified: Thu, 03 Mar 2022 22:56:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31261ff7a4ccda8ce89970b9d74fa9cae58c8aa4fff74e7f710995c1d0d2c52e`  
		Last Modified: Thu, 03 Mar 2022 22:56:33 GMT  
		Size: 93.4 MB (93405953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04eb87cb05726342287ce945c1a4d2a6e6704bf0c1c99a3dff5a1b23b56b6990`  
		Last Modified: Thu, 03 Mar 2022 22:56:16 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59de5b5b3d65537159500f65dc2fc0c1a2962a023348b762c31f406c037dd31`  
		Last Modified: Thu, 03 Mar 2022 22:56:16 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:aecfd830e8950fe21a8687609da6442161af089b5ca7d6268d38bee69b2c1aef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127688022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774c3da47e87494512f751f2ea706543d04fd29d13b58d2970a05b499df10f4f`
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
# Thu, 03 Mar 2022 20:25:53 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:25:53 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:25:53 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:25:53 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:25:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:25:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:26:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:26:18 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:26:18 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:26:18 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:26:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:26:19 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:26:19 GMT
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
	-	`sha256:5643f0cbb813dafd109d5baf0be157769503974bec4d8b5dd4cd68b30621e316`  
		Last Modified: Thu, 03 Mar 2022 20:28:45 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36078a64e944ddbea6e42aa6442ad94d4b395b8ef521b5dee2bbd11c28b27409`  
		Last Modified: Thu, 03 Mar 2022 20:28:57 GMT  
		Size: 89.8 MB (89779732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f0dd2c26918d37e8cb319e0b3c8f93d643702e26f24a02c5aa328af1833972`  
		Last Modified: Thu, 03 Mar 2022 20:28:45 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712fe50768356efec4449f3e2d95362920797b99e9aeb53fb7e6d94bd55b768a`  
		Last Modified: Thu, 03 Mar 2022 20:28:45 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.2-rc-focal`

```console
$ docker pull mariadb@sha256:8eab9f27188d1e613efa477a9c7025b719d457d80fd73a09cd053489c5b04eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8.2-rc-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:220bae35dd6770cb268a488960110814b3deb2c818d65f83dcbaf1ba0449aacc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128579619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3808c711286a6fe65a7224cc4303e813787a00ee6108a27831ddd6eb8ff4f0c8`
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
# Fri, 04 Mar 2022 01:30:23 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 04 Mar 2022 01:30:23 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 04 Mar 2022 01:30:23 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 04 Mar 2022 01:30:23 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Fri, 04 Mar 2022 01:30:23 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Fri, 04 Mar 2022 01:30:24 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 04 Mar 2022 01:30:58 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 04 Mar 2022 01:30:59 GMT
VOLUME [/var/lib/mysql]
# Fri, 04 Mar 2022 01:30:59 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Fri, 04 Mar 2022 01:30:59 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Fri, 04 Mar 2022 01:30:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Mar 2022 01:30:59 GMT
EXPOSE 3306
# Fri, 04 Mar 2022 01:30:59 GMT
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
	-	`sha256:8c1f0550683801aa881825c600927a91928ccc575970282cd543ac5bed20d3a4`  
		Last Modified: Fri, 04 Mar 2022 01:36:31 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e44e5bed9927db9168e7f1b5d07a0d779b4a72661472f1136dc1f00dbe799b`  
		Last Modified: Fri, 04 Mar 2022 01:36:44 GMT  
		Size: 88.7 MB (88652047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac1448c13b067ccb5d26f7dd1d0378b3159071054d7760aaafb6db3202abd67`  
		Last Modified: Fri, 04 Mar 2022 01:36:31 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75b107e89292a74fd8e7bf5e377bf08b057a3384a864c334a58c1f34d77ffb5`  
		Last Modified: Fri, 04 Mar 2022 01:36:31 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:fce0df6934e7a27b342669f848a370308230e8fcd776031405fd6996a2945a16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125653276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bee9fd0ceee20881cb2f2d85f2b34a4d3931b5077f5d8ed0bc59f5f32be0721c`
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
# Thu, 03 Mar 2022 20:39:02 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:39:03 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:39:04 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:39:05 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:39:06 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:39:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:39:38 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:39:38 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:39:40 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:39:41 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:39:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:39:42 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:39:43 GMT
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
	-	`sha256:fb76e878d72903fa1f87e29cc101bf40d4af64d64fc741b5fadfc1448b3ed79c`  
		Last Modified: Thu, 03 Mar 2022 20:47:11 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc8dde71d68c5d7a6217dfd16d452244125cc51bfe60e632c73f0dcaf8b1934`  
		Last Modified: Thu, 03 Mar 2022 20:47:25 GMT  
		Size: 87.6 MB (87574322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3583f4dab72174751865fe88c94ea07b1f3e92bd98c24346bd8804c6f2c5b6`  
		Last Modified: Thu, 03 Mar 2022 20:47:11 GMT  
		Size: 3.5 KB (3498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c13c8d98cec102bcdd41dd21911b79072b04a83e5382c3c37cb35ae0e093bdb`  
		Last Modified: Thu, 03 Mar 2022 20:47:11 GMT  
		Size: 6.6 KB (6612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:83b3e5d13ef8cbfe2072250f8acce71c924bfe5e2060b0e702bb3d4c88a24f5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139622025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f6883935c9460538d1cde2c52a3027d2560820e710049ae54b0e8465e809eec`
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
# Thu, 03 Mar 2022 22:28:30 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 22:28:32 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 22:28:34 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 22:28:38 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 22:28:39 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 22:28:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 22:32:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 22:32:28 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 22:32:30 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 22:32:32 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 22:32:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 22:32:38 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 22:32:43 GMT
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
	-	`sha256:e27bb09eaee81666252b1e9c3e29aef8a1f634fd0fc222d5427dab4b5580c965`  
		Last Modified: Thu, 03 Mar 2022 22:56:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31261ff7a4ccda8ce89970b9d74fa9cae58c8aa4fff74e7f710995c1d0d2c52e`  
		Last Modified: Thu, 03 Mar 2022 22:56:33 GMT  
		Size: 93.4 MB (93405953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04eb87cb05726342287ce945c1a4d2a6e6704bf0c1c99a3dff5a1b23b56b6990`  
		Last Modified: Thu, 03 Mar 2022 22:56:16 GMT  
		Size: 3.5 KB (3497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59de5b5b3d65537159500f65dc2fc0c1a2962a023348b762c31f406c037dd31`  
		Last Modified: Thu, 03 Mar 2022 22:56:16 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:aecfd830e8950fe21a8687609da6442161af089b5ca7d6268d38bee69b2c1aef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127688022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774c3da47e87494512f751f2ea706543d04fd29d13b58d2970a05b499df10f4f`
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
# Thu, 03 Mar 2022 20:25:53 GMT
ARG MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:25:53 GMT
ENV MARIADB_MAJOR=10.8
# Thu, 03 Mar 2022 20:25:53 GMT
ARG MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:25:53 GMT
ENV MARIADB_VERSION=1:10.8.2+maria~focal
# Thu, 03 Mar 2022 20:25:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
# Thu, 03 Mar 2022 20:25:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 03 Mar 2022 20:26:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.2/repo/ubuntu/ focal main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 03 Mar 2022 20:26:18 GMT
VOLUME [/var/lib/mysql]
# Thu, 03 Mar 2022 20:26:18 GMT
COPY file:0fba56e5dc10e3c33d13bb50fb484703f651fc83023b8cb76587db8c1c297e7f in /usr/local/bin/healthcheck.sh 
# Thu, 03 Mar 2022 20:26:18 GMT
COPY file:b8e07732c3935e7f1f06d41cbbc3bb55a1dfe7cc9488afc1861b4cc1537a564d in /usr/local/bin/ 
# Thu, 03 Mar 2022 20:26:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 20:26:19 GMT
EXPOSE 3306
# Thu, 03 Mar 2022 20:26:19 GMT
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
	-	`sha256:5643f0cbb813dafd109d5baf0be157769503974bec4d8b5dd4cd68b30621e316`  
		Last Modified: Thu, 03 Mar 2022 20:28:45 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36078a64e944ddbea6e42aa6442ad94d4b395b8ef521b5dee2bbd11c28b27409`  
		Last Modified: Thu, 03 Mar 2022 20:28:57 GMT  
		Size: 89.8 MB (89779732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f0dd2c26918d37e8cb319e0b3c8f93d643702e26f24a02c5aa328af1833972`  
		Last Modified: Thu, 03 Mar 2022 20:28:45 GMT  
		Size: 3.5 KB (3496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712fe50768356efec4449f3e2d95362920797b99e9aeb53fb7e6d94bd55b768a`  
		Last Modified: Thu, 03 Mar 2022 20:28:45 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:6b27df78e91348af6ac28e120a9d3f2852bb4c17d427365a4dad01b206616271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

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

### `mariadb:latest` - linux; arm64 variant v8

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

### `mariadb:latest` - linux; ppc64le

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

### `mariadb:latest` - linux; s390x

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
