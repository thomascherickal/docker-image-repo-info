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
$ docker pull mariadb@sha256:736606c3decd9b95dd8c1ee68c3e2b7e53af9e41135f6c833cd69a5eb268355e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:c1988f7cf41786b77bccd23891d1afa2f83c999f4b303bfcd5f333e934b51cc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128669741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5dd1ac0b00e78cf6f5d6152b3d37a6fbb2c9b209ea58f4d205499ed4801f305`
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
# Fri, 11 Mar 2022 01:19:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:46 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:46 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:46 GMT
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
	-	`sha256:621fa3528f37c800eddf5424ae7b35ab6f823af267c6baeb9bb20867600552de`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 3.5 KB (3483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65fa0799f33d7ab55dfbaa9cf8fb881edd3f75a9d4b6f1ad76627416769b1`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:954bc8268e746a9a4b135304d85a60a99e235a79830149f76ef0439f4157a675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125722158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38051c4e5d39b816a571729967488805c4415d7b5460e36f77392cc98a45536c`
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
# Fri, 11 Mar 2022 01:40:12 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:13 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:14 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:15 GMT
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
	-	`sha256:f1d3feb849615542564db737270cb86f87c79472cd92732650492de686bc49e2`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 3.5 KB (3485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666c07e1f7c22ebd3ff693f3a2ec21991f99d923c68a16e7a76bd88947b237b`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d35dfc2be87294ad02c377b285cde99170be7ac251c0021609d702c2a68d5daf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139539786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5bbff5e51ec39ca2817bce7fd70b2384df0a6434a3734d736a877584113f4bc`
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
# Fri, 11 Mar 2022 01:17:39 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:17:42 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:17:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:18:02 GMT
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
	-	`sha256:1f5a705aa51ed4df01e6504a076cb8470714f75d46f7c06c16a34c8e4c3b10b6`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410180f3ffbc90843c959dbca9182e9b4b16783c3e9abf15e90ef46548c09416`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; s390x

```console
$ docker pull mariadb@sha256:f57e663953b1774cf5116c02dd9a4f3b3a9e7f9199296c42fd02e7c94b1efd7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127723395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226ef0fff8e8f22de2ccb61a5a90d170ae551d3d68753c08572781c3d9afdd9b`
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
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:41 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:41 GMT
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
	-	`sha256:56572738f165202d0ca50d879a5b75c73959f04bb1e66d39722a40849517261f`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1c1e0cca65f889f547f42513cc37e2ca3c6a988fef8132fa46bc00c73e0b8a`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:736606c3decd9b95dd8c1ee68c3e2b7e53af9e41135f6c833cd69a5eb268355e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c1988f7cf41786b77bccd23891d1afa2f83c999f4b303bfcd5f333e934b51cc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128669741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5dd1ac0b00e78cf6f5d6152b3d37a6fbb2c9b209ea58f4d205499ed4801f305`
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
# Fri, 11 Mar 2022 01:19:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:46 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:46 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:46 GMT
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
	-	`sha256:621fa3528f37c800eddf5424ae7b35ab6f823af267c6baeb9bb20867600552de`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 3.5 KB (3483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65fa0799f33d7ab55dfbaa9cf8fb881edd3f75a9d4b6f1ad76627416769b1`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:954bc8268e746a9a4b135304d85a60a99e235a79830149f76ef0439f4157a675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125722158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38051c4e5d39b816a571729967488805c4415d7b5460e36f77392cc98a45536c`
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
# Fri, 11 Mar 2022 01:40:12 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:13 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:14 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:15 GMT
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
	-	`sha256:f1d3feb849615542564db737270cb86f87c79472cd92732650492de686bc49e2`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 3.5 KB (3485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666c07e1f7c22ebd3ff693f3a2ec21991f99d923c68a16e7a76bd88947b237b`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d35dfc2be87294ad02c377b285cde99170be7ac251c0021609d702c2a68d5daf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139539786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5bbff5e51ec39ca2817bce7fd70b2384df0a6434a3734d736a877584113f4bc`
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
# Fri, 11 Mar 2022 01:17:39 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:17:42 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:17:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:18:02 GMT
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
	-	`sha256:1f5a705aa51ed4df01e6504a076cb8470714f75d46f7c06c16a34c8e4c3b10b6`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410180f3ffbc90843c959dbca9182e9b4b16783c3e9abf15e90ef46548c09416`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:f57e663953b1774cf5116c02dd9a4f3b3a9e7f9199296c42fd02e7c94b1efd7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127723395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226ef0fff8e8f22de2ccb61a5a90d170ae551d3d68753c08572781c3d9afdd9b`
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
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:41 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:41 GMT
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
	-	`sha256:56572738f165202d0ca50d879a5b75c73959f04bb1e66d39722a40849517261f`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1c1e0cca65f889f547f42513cc37e2ca3c6a988fef8132fa46bc00c73e0b8a`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:a8e6a5565334906f486454cadfc9edaaa6eddb5705737ecb7951004f3d54cbb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:10442f4038d6e85a0a0757ea042984bc03cc9f465fb6c753aa65f8eb39ee6ca4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109315474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af15a0064e3524a121ca64d73426076d6c78f700634780c0009c21492dd5032`
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
# Fri, 11 Mar 2022 01:20:02 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:20:02 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:20:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:20:02 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:20:03 GMT
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
	-	`sha256:33185d1bf3c639c51e4003715d88cc111b3716c7219acd686a882bac929c60d5`  
		Last Modified: Fri, 11 Mar 2022 01:22:23 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5b2016e84c02318a4d9c929cace7a8a780cf7636dda674231c8df75fc26181`  
		Last Modified: Fri, 11 Mar 2022 01:22:23 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5520a6a3f0f5096a6403c77387881d50b6f75c50c496e6178707a7152c6711`  
		Last Modified: Fri, 11 Mar 2022 01:22:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b53d76f255c07d1f0371352c3986c46c145f549930905ce183433ba960a82d18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104250976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99fc385339e2b9e00e28c624474577fbb767d501476ce1593c70ae4d8be716bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 03 Mar 2022 19:40:54 GMT
ADD file:4e0e00a64dd88d531092dae4e900f36acb9c48c652d278ec0cd32aef9fffb42b in / 
# Thu, 03 Mar 2022 19:40:55 GMT
CMD ["bash"]
# Fri, 11 Mar 2022 01:41:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Mar 2022 01:41:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 01:41:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Mar 2022 01:41:36 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Mar 2022 01:41:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Mar 2022 01:41:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 01:41:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Mar 2022 01:42:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 11 Mar 2022 01:42:49 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 11 Mar 2022 01:42:50 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 11 Mar 2022 01:42:51 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 11 Mar 2022 01:42:52 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 11 Mar 2022 01:42:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 11 Mar 2022 01:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Mar 2022 01:43:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 11 Mar 2022 01:43:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Mar 2022 01:43:22 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:43:23 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:43:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:43:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:43:25 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:43:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:20d796c36622ded7b79b53bfa23d7db4140fde7ea3842825f9aca4070b429317`  
		Last Modified: Thu, 03 Mar 2022 19:42:21 GMT  
		Size: 23.7 MB (23729651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3fdb4ddb2ac96f062e0f816dbb92c5a95ca14c81a744844fcadeca6fc7008d`  
		Last Modified: Fri, 11 Mar 2022 01:46:38 GMT  
		Size: 1.9 KB (1860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33f09c738049f5d0e4afa892a6f94d4347f0e2f3a128bfc6cc0aea8051c918d`  
		Last Modified: Fri, 11 Mar 2022 01:46:39 GMT  
		Size: 4.3 MB (4261545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715c624740a169fabf88d3976cd786b460e0c839d1e6e379c3d2cdb0e050c46b`  
		Last Modified: Fri, 11 Mar 2022 01:46:37 GMT  
		Size: 3.2 MB (3207299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a651b0df600d17b8b829bead7ba8c84afed6398e5ad5389a3ab65b2ac94754`  
		Last Modified: Fri, 11 Mar 2022 01:46:36 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67d39c2c797366adcdf384fa181392e23dd05ffd777c24077c130bc35ee2a6`  
		Last Modified: Fri, 11 Mar 2022 01:46:37 GMT  
		Size: 1.5 MB (1529411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1714f24138d75742344057e89b91ffa7be6b488e9c0483265547825a00b2ed27`  
		Last Modified: Fri, 11 Mar 2022 01:46:36 GMT  
		Size: 5.1 KB (5148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f3da2b30b94105adf31e4754832ae489d9f7b31b08eda5d097f675dba70bad`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cfb1d9d1f6adb65659765f8cdd334f28390abe9455ef426e11ff0b06d8e06e`  
		Last Modified: Fri, 11 Mar 2022 01:46:45 GMT  
		Size: 71.5 MB (71505398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113e48fd129071e431fc77b7f16088e780511c8ed533772b20414004ebd894cc`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a85af8aab59f899d1d4b17e79f8d878aa2f002ccdea122c5fea4dcc8e9962`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f197802a0430a7739d201f5f7923f8161e1d39f94e7face7031c60c7fd32fa80`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:b118e6ba1d2136747532bfca6291426b87890bf38a1dbf07162278130359d19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117714552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966137bb7b82865ae69e0b1397697467837ed19945c3458c6094bad941efc093`
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
# Fri, 11 Mar 2022 01:20:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:20:54 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:21:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:21:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:21:18 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:21:22 GMT
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
	-	`sha256:df96256843e965b11b03dbd24f736d5540c868e8f6e5e8d5970677910ebf20a6`  
		Last Modified: Fri, 11 Mar 2022 01:25:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244d1409fce6534691472104c6ee569f998a762a002019b90b7c131f44f9bcd4`  
		Last Modified: Fri, 11 Mar 2022 01:25:16 GMT  
		Size: 6.6 KB (6602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776da122d357e4448808ec9c69842b8f18e1cef970c54a274f4a552359a63da0`  
		Last Modified: Fri, 11 Mar 2022 01:25:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:a8e6a5565334906f486454cadfc9edaaa6eddb5705737ecb7951004f3d54cbb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:10442f4038d6e85a0a0757ea042984bc03cc9f465fb6c753aa65f8eb39ee6ca4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109315474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af15a0064e3524a121ca64d73426076d6c78f700634780c0009c21492dd5032`
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
# Fri, 11 Mar 2022 01:20:02 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:20:02 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:20:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:20:02 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:20:03 GMT
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
	-	`sha256:33185d1bf3c639c51e4003715d88cc111b3716c7219acd686a882bac929c60d5`  
		Last Modified: Fri, 11 Mar 2022 01:22:23 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5b2016e84c02318a4d9c929cace7a8a780cf7636dda674231c8df75fc26181`  
		Last Modified: Fri, 11 Mar 2022 01:22:23 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5520a6a3f0f5096a6403c77387881d50b6f75c50c496e6178707a7152c6711`  
		Last Modified: Fri, 11 Mar 2022 01:22:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b53d76f255c07d1f0371352c3986c46c145f549930905ce183433ba960a82d18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104250976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99fc385339e2b9e00e28c624474577fbb767d501476ce1593c70ae4d8be716bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 03 Mar 2022 19:40:54 GMT
ADD file:4e0e00a64dd88d531092dae4e900f36acb9c48c652d278ec0cd32aef9fffb42b in / 
# Thu, 03 Mar 2022 19:40:55 GMT
CMD ["bash"]
# Fri, 11 Mar 2022 01:41:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Mar 2022 01:41:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 01:41:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Mar 2022 01:41:36 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Mar 2022 01:41:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Mar 2022 01:41:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 01:41:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Mar 2022 01:42:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 11 Mar 2022 01:42:49 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 11 Mar 2022 01:42:50 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 11 Mar 2022 01:42:51 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 11 Mar 2022 01:42:52 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 11 Mar 2022 01:42:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 11 Mar 2022 01:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Mar 2022 01:43:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 11 Mar 2022 01:43:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Mar 2022 01:43:22 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:43:23 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:43:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:43:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:43:25 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:43:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:20d796c36622ded7b79b53bfa23d7db4140fde7ea3842825f9aca4070b429317`  
		Last Modified: Thu, 03 Mar 2022 19:42:21 GMT  
		Size: 23.7 MB (23729651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3fdb4ddb2ac96f062e0f816dbb92c5a95ca14c81a744844fcadeca6fc7008d`  
		Last Modified: Fri, 11 Mar 2022 01:46:38 GMT  
		Size: 1.9 KB (1860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33f09c738049f5d0e4afa892a6f94d4347f0e2f3a128bfc6cc0aea8051c918d`  
		Last Modified: Fri, 11 Mar 2022 01:46:39 GMT  
		Size: 4.3 MB (4261545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715c624740a169fabf88d3976cd786b460e0c839d1e6e379c3d2cdb0e050c46b`  
		Last Modified: Fri, 11 Mar 2022 01:46:37 GMT  
		Size: 3.2 MB (3207299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a651b0df600d17b8b829bead7ba8c84afed6398e5ad5389a3ab65b2ac94754`  
		Last Modified: Fri, 11 Mar 2022 01:46:36 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67d39c2c797366adcdf384fa181392e23dd05ffd777c24077c130bc35ee2a6`  
		Last Modified: Fri, 11 Mar 2022 01:46:37 GMT  
		Size: 1.5 MB (1529411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1714f24138d75742344057e89b91ffa7be6b488e9c0483265547825a00b2ed27`  
		Last Modified: Fri, 11 Mar 2022 01:46:36 GMT  
		Size: 5.1 KB (5148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f3da2b30b94105adf31e4754832ae489d9f7b31b08eda5d097f675dba70bad`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cfb1d9d1f6adb65659765f8cdd334f28390abe9455ef426e11ff0b06d8e06e`  
		Last Modified: Fri, 11 Mar 2022 01:46:45 GMT  
		Size: 71.5 MB (71505398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113e48fd129071e431fc77b7f16088e780511c8ed533772b20414004ebd894cc`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a85af8aab59f899d1d4b17e79f8d878aa2f002ccdea122c5fea4dcc8e9962`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f197802a0430a7739d201f5f7923f8161e1d39f94e7face7031c60c7fd32fa80`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:b118e6ba1d2136747532bfca6291426b87890bf38a1dbf07162278130359d19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117714552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966137bb7b82865ae69e0b1397697467837ed19945c3458c6094bad941efc093`
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
# Fri, 11 Mar 2022 01:20:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:20:54 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:21:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:21:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:21:18 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:21:22 GMT
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
	-	`sha256:df96256843e965b11b03dbd24f736d5540c868e8f6e5e8d5970677910ebf20a6`  
		Last Modified: Fri, 11 Mar 2022 01:25:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244d1409fce6534691472104c6ee569f998a762a002019b90b7c131f44f9bcd4`  
		Last Modified: Fri, 11 Mar 2022 01:25:16 GMT  
		Size: 6.6 KB (6602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776da122d357e4448808ec9c69842b8f18e1cef970c54a274f4a552359a63da0`  
		Last Modified: Fri, 11 Mar 2022 01:25:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.43`

```console
$ docker pull mariadb@sha256:a8e6a5565334906f486454cadfc9edaaa6eddb5705737ecb7951004f3d54cbb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.43` - linux; amd64

```console
$ docker pull mariadb@sha256:10442f4038d6e85a0a0757ea042984bc03cc9f465fb6c753aa65f8eb39ee6ca4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109315474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af15a0064e3524a121ca64d73426076d6c78f700634780c0009c21492dd5032`
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
# Fri, 11 Mar 2022 01:20:02 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:20:02 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:20:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:20:02 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:20:03 GMT
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
	-	`sha256:33185d1bf3c639c51e4003715d88cc111b3716c7219acd686a882bac929c60d5`  
		Last Modified: Fri, 11 Mar 2022 01:22:23 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5b2016e84c02318a4d9c929cace7a8a780cf7636dda674231c8df75fc26181`  
		Last Modified: Fri, 11 Mar 2022 01:22:23 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5520a6a3f0f5096a6403c77387881d50b6f75c50c496e6178707a7152c6711`  
		Last Modified: Fri, 11 Mar 2022 01:22:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b53d76f255c07d1f0371352c3986c46c145f549930905ce183433ba960a82d18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104250976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99fc385339e2b9e00e28c624474577fbb767d501476ce1593c70ae4d8be716bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 03 Mar 2022 19:40:54 GMT
ADD file:4e0e00a64dd88d531092dae4e900f36acb9c48c652d278ec0cd32aef9fffb42b in / 
# Thu, 03 Mar 2022 19:40:55 GMT
CMD ["bash"]
# Fri, 11 Mar 2022 01:41:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Mar 2022 01:41:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 01:41:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Mar 2022 01:41:36 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Mar 2022 01:41:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Mar 2022 01:41:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 01:41:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Mar 2022 01:42:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 11 Mar 2022 01:42:49 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 11 Mar 2022 01:42:50 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 11 Mar 2022 01:42:51 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 11 Mar 2022 01:42:52 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 11 Mar 2022 01:42:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 11 Mar 2022 01:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Mar 2022 01:43:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 11 Mar 2022 01:43:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Mar 2022 01:43:22 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:43:23 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:43:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:43:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:43:25 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:43:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:20d796c36622ded7b79b53bfa23d7db4140fde7ea3842825f9aca4070b429317`  
		Last Modified: Thu, 03 Mar 2022 19:42:21 GMT  
		Size: 23.7 MB (23729651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3fdb4ddb2ac96f062e0f816dbb92c5a95ca14c81a744844fcadeca6fc7008d`  
		Last Modified: Fri, 11 Mar 2022 01:46:38 GMT  
		Size: 1.9 KB (1860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33f09c738049f5d0e4afa892a6f94d4347f0e2f3a128bfc6cc0aea8051c918d`  
		Last Modified: Fri, 11 Mar 2022 01:46:39 GMT  
		Size: 4.3 MB (4261545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715c624740a169fabf88d3976cd786b460e0c839d1e6e379c3d2cdb0e050c46b`  
		Last Modified: Fri, 11 Mar 2022 01:46:37 GMT  
		Size: 3.2 MB (3207299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a651b0df600d17b8b829bead7ba8c84afed6398e5ad5389a3ab65b2ac94754`  
		Last Modified: Fri, 11 Mar 2022 01:46:36 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67d39c2c797366adcdf384fa181392e23dd05ffd777c24077c130bc35ee2a6`  
		Last Modified: Fri, 11 Mar 2022 01:46:37 GMT  
		Size: 1.5 MB (1529411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1714f24138d75742344057e89b91ffa7be6b488e9c0483265547825a00b2ed27`  
		Last Modified: Fri, 11 Mar 2022 01:46:36 GMT  
		Size: 5.1 KB (5148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f3da2b30b94105adf31e4754832ae489d9f7b31b08eda5d097f675dba70bad`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cfb1d9d1f6adb65659765f8cdd334f28390abe9455ef426e11ff0b06d8e06e`  
		Last Modified: Fri, 11 Mar 2022 01:46:45 GMT  
		Size: 71.5 MB (71505398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113e48fd129071e431fc77b7f16088e780511c8ed533772b20414004ebd894cc`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a85af8aab59f899d1d4b17e79f8d878aa2f002ccdea122c5fea4dcc8e9962`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f197802a0430a7739d201f5f7923f8161e1d39f94e7face7031c60c7fd32fa80`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43` - linux; ppc64le

```console
$ docker pull mariadb@sha256:b118e6ba1d2136747532bfca6291426b87890bf38a1dbf07162278130359d19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117714552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966137bb7b82865ae69e0b1397697467837ed19945c3458c6094bad941efc093`
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
# Fri, 11 Mar 2022 01:20:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:20:54 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:21:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:21:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:21:18 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:21:22 GMT
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
	-	`sha256:df96256843e965b11b03dbd24f736d5540c868e8f6e5e8d5970677910ebf20a6`  
		Last Modified: Fri, 11 Mar 2022 01:25:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244d1409fce6534691472104c6ee569f998a762a002019b90b7c131f44f9bcd4`  
		Last Modified: Fri, 11 Mar 2022 01:25:16 GMT  
		Size: 6.6 KB (6602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776da122d357e4448808ec9c69842b8f18e1cef970c54a274f4a552359a63da0`  
		Last Modified: Fri, 11 Mar 2022 01:25:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.43-bionic`

```console
$ docker pull mariadb@sha256:a8e6a5565334906f486454cadfc9edaaa6eddb5705737ecb7951004f3d54cbb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.43-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:10442f4038d6e85a0a0757ea042984bc03cc9f465fb6c753aa65f8eb39ee6ca4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109315474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af15a0064e3524a121ca64d73426076d6c78f700634780c0009c21492dd5032`
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
# Fri, 11 Mar 2022 01:20:02 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:20:02 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:20:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:20:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:20:02 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:20:03 GMT
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
	-	`sha256:33185d1bf3c639c51e4003715d88cc111b3716c7219acd686a882bac929c60d5`  
		Last Modified: Fri, 11 Mar 2022 01:22:23 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5b2016e84c02318a4d9c929cace7a8a780cf7636dda674231c8df75fc26181`  
		Last Modified: Fri, 11 Mar 2022 01:22:23 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5520a6a3f0f5096a6403c77387881d50b6f75c50c496e6178707a7152c6711`  
		Last Modified: Fri, 11 Mar 2022 01:22:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b53d76f255c07d1f0371352c3986c46c145f549930905ce183433ba960a82d18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104250976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99fc385339e2b9e00e28c624474577fbb767d501476ce1593c70ae4d8be716bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 03 Mar 2022 19:40:54 GMT
ADD file:4e0e00a64dd88d531092dae4e900f36acb9c48c652d278ec0cd32aef9fffb42b in / 
# Thu, 03 Mar 2022 19:40:55 GMT
CMD ["bash"]
# Fri, 11 Mar 2022 01:41:06 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 11 Mar 2022 01:41:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 01:41:19 GMT
ENV GOSU_VERSION=1.14
# Fri, 11 Mar 2022 01:41:36 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Mar 2022 01:41:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 11 Mar 2022 01:41:46 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Mar 2022 01:41:47 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 11 Mar 2022 01:42:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 11 Mar 2022 01:42:49 GMT
ARG MARIADB_MAJOR=10.2
# Fri, 11 Mar 2022 01:42:50 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 11 Mar 2022 01:42:51 GMT
ARG MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 11 Mar 2022 01:42:52 GMT
ENV MARIADB_VERSION=1:10.2.43+maria~bionic
# Fri, 11 Mar 2022 01:42:53 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
# Fri, 11 Mar 2022 01:42:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 11 Mar 2022 01:43:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	sed --follow-symlinks -i -e 's/--loose-disable-plugin-file-key-management//' /usr/bin/mysql_install_db ; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 11 Mar 2022 01:43:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 11 Mar 2022 01:43:22 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:43:23 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:43:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:43:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:43:25 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:43:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:20d796c36622ded7b79b53bfa23d7db4140fde7ea3842825f9aca4070b429317`  
		Last Modified: Thu, 03 Mar 2022 19:42:21 GMT  
		Size: 23.7 MB (23729651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3fdb4ddb2ac96f062e0f816dbb92c5a95ca14c81a744844fcadeca6fc7008d`  
		Last Modified: Fri, 11 Mar 2022 01:46:38 GMT  
		Size: 1.9 KB (1860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33f09c738049f5d0e4afa892a6f94d4347f0e2f3a128bfc6cc0aea8051c918d`  
		Last Modified: Fri, 11 Mar 2022 01:46:39 GMT  
		Size: 4.3 MB (4261545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715c624740a169fabf88d3976cd786b460e0c839d1e6e379c3d2cdb0e050c46b`  
		Last Modified: Fri, 11 Mar 2022 01:46:37 GMT  
		Size: 3.2 MB (3207299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a651b0df600d17b8b829bead7ba8c84afed6398e5ad5389a3ab65b2ac94754`  
		Last Modified: Fri, 11 Mar 2022 01:46:36 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67d39c2c797366adcdf384fa181392e23dd05ffd777c24077c130bc35ee2a6`  
		Last Modified: Fri, 11 Mar 2022 01:46:37 GMT  
		Size: 1.5 MB (1529411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1714f24138d75742344057e89b91ffa7be6b488e9c0483265547825a00b2ed27`  
		Last Modified: Fri, 11 Mar 2022 01:46:36 GMT  
		Size: 5.1 KB (5148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f3da2b30b94105adf31e4754832ae489d9f7b31b08eda5d097f675dba70bad`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cfb1d9d1f6adb65659765f8cdd334f28390abe9455ef426e11ff0b06d8e06e`  
		Last Modified: Fri, 11 Mar 2022 01:46:45 GMT  
		Size: 71.5 MB (71505398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113e48fd129071e431fc77b7f16088e780511c8ed533772b20414004ebd894cc`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224a85af8aab59f899d1d4b17e79f8d878aa2f002ccdea122c5fea4dcc8e9962`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 6.6 KB (6607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f197802a0430a7739d201f5f7923f8161e1d39f94e7face7031c60c7fd32fa80`  
		Last Modified: Fri, 11 Mar 2022 01:46:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.43-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:b118e6ba1d2136747532bfca6291426b87890bf38a1dbf07162278130359d19e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117714552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966137bb7b82865ae69e0b1397697467837ed19945c3458c6094bad941efc093`
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
# Fri, 11 Mar 2022 01:20:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:20:54 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:21:05 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.2.43/repo/ubuntu/ bionic main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:21:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:21:18 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:21:22 GMT
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
	-	`sha256:df96256843e965b11b03dbd24f736d5540c868e8f6e5e8d5970677910ebf20a6`  
		Last Modified: Fri, 11 Mar 2022 01:25:16 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244d1409fce6534691472104c6ee569f998a762a002019b90b7c131f44f9bcd4`  
		Last Modified: Fri, 11 Mar 2022 01:25:16 GMT  
		Size: 6.6 KB (6602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776da122d357e4448808ec9c69842b8f18e1cef970c54a274f4a552359a63da0`  
		Last Modified: Fri, 11 Mar 2022 01:25:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:18718232933258e16405a98244448ae705734d76a146b0adb29908c63f5a05b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:e233a8bcc31e211b2f36df5466327837efb4f84b4960c32c37fe34fccf19b5be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120118792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf85b1958f3e3576dafaadeca0f950be5964b4f8f6b26a862cd8bfbf01de350`
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
# Fri, 11 Mar 2022 01:19:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:58 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:19:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:59 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:59 GMT
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
	-	`sha256:926bc1f886785ed141439a4c116ec02de74ad0ea91b2f755cb45b72a0ea6d8ec`  
		Last Modified: Fri, 11 Mar 2022 01:22:07 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d88b50be23abc722fc0886a5d9f8e6111f8b85e72b9cc8ba91e7b9b78d2464d`  
		Last Modified: Fri, 11 Mar 2022 01:22:07 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e68f04384b2f894e6faa7a13069915d5e06d9345247da557f3d61c5e84e81ba`  
		Last Modified: Fri, 11 Mar 2022 01:22:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b27983dfb4d6ce9c42dd758e64d41d91d978c6ac8f64f9045cb2fc193da440bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117609966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86095b2d41657bbaa5599ed5b3cc71b6ebaa126c7eb115570bf02b8ed031519e`
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
# Fri, 11 Mar 2022 01:40:55 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:56 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:40:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:59 GMT
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
	-	`sha256:2be6d06b4ccf2a0acca64caccab7b00904bc0c65dfcd71145de93bc2730195bc`  
		Last Modified: Fri, 11 Mar 2022 01:46:16 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363ca18db9f47f952c3a6087cf32f3a0d3eb597fe142cf3f9b31b427e4add06c`  
		Last Modified: Fri, 11 Mar 2022 01:46:16 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d333503501ff899366e81effec4aec158bd1595d487a01b689c8807bbe8246`  
		Last Modified: Fri, 11 Mar 2022 01:46:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0b1ca4564fa935dd8f0218e80d8f110a78aca93a2a30762c832d0fd1c53d1360
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131007911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b382499dc1a640c01f7c912d24f2856fed0ec8bb3d2715a75a92ffa3cf476c`
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
# Fri, 11 Mar 2022 01:20:10 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:20:12 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:20:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:20:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:20:29 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:20:36 GMT
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
	-	`sha256:8f7575d8222cf86419775532f8796b39824149ba2cdb4a644d3a56f10ed49c09`  
		Last Modified: Fri, 11 Mar 2022 01:24:55 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2a1440ee8c28120946b088744b305c8e323be6b1f6eae4e5c20737c5c29a79`  
		Last Modified: Fri, 11 Mar 2022 01:24:55 GMT  
		Size: 6.6 KB (6602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c39c32126b5e07a6d86a70a967ce9a911eb3ebc8f36b188d3e93ba449a3df70`  
		Last Modified: Fri, 11 Mar 2022 01:24:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:18718232933258e16405a98244448ae705734d76a146b0adb29908c63f5a05b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:e233a8bcc31e211b2f36df5466327837efb4f84b4960c32c37fe34fccf19b5be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120118792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf85b1958f3e3576dafaadeca0f950be5964b4f8f6b26a862cd8bfbf01de350`
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
# Fri, 11 Mar 2022 01:19:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:58 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:19:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:59 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:59 GMT
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
	-	`sha256:926bc1f886785ed141439a4c116ec02de74ad0ea91b2f755cb45b72a0ea6d8ec`  
		Last Modified: Fri, 11 Mar 2022 01:22:07 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d88b50be23abc722fc0886a5d9f8e6111f8b85e72b9cc8ba91e7b9b78d2464d`  
		Last Modified: Fri, 11 Mar 2022 01:22:07 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e68f04384b2f894e6faa7a13069915d5e06d9345247da557f3d61c5e84e81ba`  
		Last Modified: Fri, 11 Mar 2022 01:22:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b27983dfb4d6ce9c42dd758e64d41d91d978c6ac8f64f9045cb2fc193da440bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117609966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86095b2d41657bbaa5599ed5b3cc71b6ebaa126c7eb115570bf02b8ed031519e`
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
# Fri, 11 Mar 2022 01:40:55 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:56 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:40:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:59 GMT
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
	-	`sha256:2be6d06b4ccf2a0acca64caccab7b00904bc0c65dfcd71145de93bc2730195bc`  
		Last Modified: Fri, 11 Mar 2022 01:46:16 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363ca18db9f47f952c3a6087cf32f3a0d3eb597fe142cf3f9b31b427e4add06c`  
		Last Modified: Fri, 11 Mar 2022 01:46:16 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d333503501ff899366e81effec4aec158bd1595d487a01b689c8807bbe8246`  
		Last Modified: Fri, 11 Mar 2022 01:46:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0b1ca4564fa935dd8f0218e80d8f110a78aca93a2a30762c832d0fd1c53d1360
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131007911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b382499dc1a640c01f7c912d24f2856fed0ec8bb3d2715a75a92ffa3cf476c`
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
# Fri, 11 Mar 2022 01:20:10 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:20:12 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:20:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:20:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:20:29 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:20:36 GMT
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
	-	`sha256:8f7575d8222cf86419775532f8796b39824149ba2cdb4a644d3a56f10ed49c09`  
		Last Modified: Fri, 11 Mar 2022 01:24:55 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2a1440ee8c28120946b088744b305c8e323be6b1f6eae4e5c20737c5c29a79`  
		Last Modified: Fri, 11 Mar 2022 01:24:55 GMT  
		Size: 6.6 KB (6602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c39c32126b5e07a6d86a70a967ce9a911eb3ebc8f36b188d3e93ba449a3df70`  
		Last Modified: Fri, 11 Mar 2022 01:24:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.34`

```console
$ docker pull mariadb@sha256:18718232933258e16405a98244448ae705734d76a146b0adb29908c63f5a05b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.34` - linux; amd64

```console
$ docker pull mariadb@sha256:e233a8bcc31e211b2f36df5466327837efb4f84b4960c32c37fe34fccf19b5be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120118792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf85b1958f3e3576dafaadeca0f950be5964b4f8f6b26a862cd8bfbf01de350`
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
# Fri, 11 Mar 2022 01:19:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:58 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:19:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:59 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:59 GMT
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
	-	`sha256:926bc1f886785ed141439a4c116ec02de74ad0ea91b2f755cb45b72a0ea6d8ec`  
		Last Modified: Fri, 11 Mar 2022 01:22:07 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d88b50be23abc722fc0886a5d9f8e6111f8b85e72b9cc8ba91e7b9b78d2464d`  
		Last Modified: Fri, 11 Mar 2022 01:22:07 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e68f04384b2f894e6faa7a13069915d5e06d9345247da557f3d61c5e84e81ba`  
		Last Modified: Fri, 11 Mar 2022 01:22:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b27983dfb4d6ce9c42dd758e64d41d91d978c6ac8f64f9045cb2fc193da440bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117609966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86095b2d41657bbaa5599ed5b3cc71b6ebaa126c7eb115570bf02b8ed031519e`
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
# Fri, 11 Mar 2022 01:40:55 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:56 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:40:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:59 GMT
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
	-	`sha256:2be6d06b4ccf2a0acca64caccab7b00904bc0c65dfcd71145de93bc2730195bc`  
		Last Modified: Fri, 11 Mar 2022 01:46:16 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363ca18db9f47f952c3a6087cf32f3a0d3eb597fe142cf3f9b31b427e4add06c`  
		Last Modified: Fri, 11 Mar 2022 01:46:16 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d333503501ff899366e81effec4aec158bd1595d487a01b689c8807bbe8246`  
		Last Modified: Fri, 11 Mar 2022 01:46:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0b1ca4564fa935dd8f0218e80d8f110a78aca93a2a30762c832d0fd1c53d1360
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131007911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b382499dc1a640c01f7c912d24f2856fed0ec8bb3d2715a75a92ffa3cf476c`
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
# Fri, 11 Mar 2022 01:20:10 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:20:12 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:20:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:20:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:20:29 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:20:36 GMT
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
	-	`sha256:8f7575d8222cf86419775532f8796b39824149ba2cdb4a644d3a56f10ed49c09`  
		Last Modified: Fri, 11 Mar 2022 01:24:55 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2a1440ee8c28120946b088744b305c8e323be6b1f6eae4e5c20737c5c29a79`  
		Last Modified: Fri, 11 Mar 2022 01:24:55 GMT  
		Size: 6.6 KB (6602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c39c32126b5e07a6d86a70a967ce9a911eb3ebc8f36b188d3e93ba449a3df70`  
		Last Modified: Fri, 11 Mar 2022 01:24:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.34-focal`

```console
$ docker pull mariadb@sha256:18718232933258e16405a98244448ae705734d76a146b0adb29908c63f5a05b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.34-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:e233a8bcc31e211b2f36df5466327837efb4f84b4960c32c37fe34fccf19b5be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120118792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf85b1958f3e3576dafaadeca0f950be5964b4f8f6b26a862cd8bfbf01de350`
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
# Fri, 11 Mar 2022 01:19:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:58 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:59 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:19:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:59 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:59 GMT
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
	-	`sha256:926bc1f886785ed141439a4c116ec02de74ad0ea91b2f755cb45b72a0ea6d8ec`  
		Last Modified: Fri, 11 Mar 2022 01:22:07 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d88b50be23abc722fc0886a5d9f8e6111f8b85e72b9cc8ba91e7b9b78d2464d`  
		Last Modified: Fri, 11 Mar 2022 01:22:07 GMT  
		Size: 6.6 KB (6598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e68f04384b2f894e6faa7a13069915d5e06d9345247da557f3d61c5e84e81ba`  
		Last Modified: Fri, 11 Mar 2022 01:22:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b27983dfb4d6ce9c42dd758e64d41d91d978c6ac8f64f9045cb2fc193da440bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117609966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86095b2d41657bbaa5599ed5b3cc71b6ebaa126c7eb115570bf02b8ed031519e`
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
# Fri, 11 Mar 2022 01:40:55 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:56 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:56 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:40:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:59 GMT
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
	-	`sha256:2be6d06b4ccf2a0acca64caccab7b00904bc0c65dfcd71145de93bc2730195bc`  
		Last Modified: Fri, 11 Mar 2022 01:46:16 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363ca18db9f47f952c3a6087cf32f3a0d3eb597fe142cf3f9b31b427e4add06c`  
		Last Modified: Fri, 11 Mar 2022 01:46:16 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d333503501ff899366e81effec4aec158bd1595d487a01b689c8807bbe8246`  
		Last Modified: Fri, 11 Mar 2022 01:46:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.34-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:0b1ca4564fa935dd8f0218e80d8f110a78aca93a2a30762c832d0fd1c53d1360
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131007911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b382499dc1a640c01f7c912d24f2856fed0ec8bb3d2715a75a92ffa3cf476c`
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
# Fri, 11 Mar 2022 01:20:10 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:20:12 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:20:19 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.3.34/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:20:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:20:29 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:20:36 GMT
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
	-	`sha256:8f7575d8222cf86419775532f8796b39824149ba2cdb4a644d3a56f10ed49c09`  
		Last Modified: Fri, 11 Mar 2022 01:24:55 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2a1440ee8c28120946b088744b305c8e323be6b1f6eae4e5c20737c5c29a79`  
		Last Modified: Fri, 11 Mar 2022 01:24:55 GMT  
		Size: 6.6 KB (6602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c39c32126b5e07a6d86a70a967ce9a911eb3ebc8f36b188d3e93ba449a3df70`  
		Last Modified: Fri, 11 Mar 2022 01:24:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:65bc4d6acb5a5ba08f69654b727afca9057c8f66528f90e1f3f9544213343e4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:9082c559f2e3e582b35582c5b5e259ca9c4237219aabee51eae636e8dc00e911
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125680333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fab64ba115d1ad0ede48f65ede54e10bbe3f72970bf3afe11be6e3de6ecbe5`
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
# Fri, 11 Mar 2022 01:19:55 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:55 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:55 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:56 GMT
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
	-	`sha256:eb2a5e8f6ae43ddec8710950b73a5e2f4c86bd04d705dcd7ddd7969d175aa39c`  
		Last Modified: Fri, 11 Mar 2022 01:21:51 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691854f7300c7e1c9a48cbd66f91ce7f0fd1b74531951b51187c538df84a049f`  
		Last Modified: Fri, 11 Mar 2022 01:21:51 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1479d8719b8c480d4bb08970f0e36f7167fe7bec3820504e9b208532ca73ad9`  
		Last Modified: Fri, 11 Mar 2022 01:21:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1f0ceea8c14c17fee52cdbe03a751ace674f01ab93587adbab87b075ff44ccfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123004812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c563f0637efb118872c69265661422af08cbf9bd59d66bf05f1adf1e6855ff0`
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
# Fri, 11 Mar 2022 01:40:44 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:45 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:40:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:47 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:48 GMT
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
	-	`sha256:ba7418bd4a80bd5e5f9b31430eeb335cc3295df6547dcb53f68d415e7d2a16fc`  
		Last Modified: Fri, 11 Mar 2022 01:45:57 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20596863a9b6e75cf8a11a64163df54a226fd5fdddb5d1845debd92b7fc11f51`  
		Last Modified: Fri, 11 Mar 2022 01:45:57 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efe1da115837720b902fc86e3e183e29f39ee9b3d5ffe70ede594e0b4f24f0e`  
		Last Modified: Fri, 11 Mar 2022 01:45:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4e0c3bf0e87363fbcc603f20cc6b5744f22c52b7c476076546293565e62c725f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136562216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c765fa755a1c9a14517a2d4237d40c3e3f918d30b07db1c68e77fb8a5ef86d93`
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
# Fri, 11 Mar 2022 01:19:30 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:32 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:53 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:57 GMT
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
	-	`sha256:42c342ce2822718aac12e64bcb686dd687d39c4bf3be0df2f663ad59311b6442`  
		Last Modified: Fri, 11 Mar 2022 01:24:33 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1606d38719b289358ab38e3184a49552cfedce0c0e98dfecf8e547805cf329ab`  
		Last Modified: Fri, 11 Mar 2022 01:24:33 GMT  
		Size: 6.6 KB (6602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e449d1d2e45971ae9a9b272897ce77d3c6b640810cfb656333f919329ca098`  
		Last Modified: Fri, 11 Mar 2022 01:24:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:65bc4d6acb5a5ba08f69654b727afca9057c8f66528f90e1f3f9544213343e4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:9082c559f2e3e582b35582c5b5e259ca9c4237219aabee51eae636e8dc00e911
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125680333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fab64ba115d1ad0ede48f65ede54e10bbe3f72970bf3afe11be6e3de6ecbe5`
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
# Fri, 11 Mar 2022 01:19:55 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:55 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:55 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:56 GMT
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
	-	`sha256:eb2a5e8f6ae43ddec8710950b73a5e2f4c86bd04d705dcd7ddd7969d175aa39c`  
		Last Modified: Fri, 11 Mar 2022 01:21:51 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691854f7300c7e1c9a48cbd66f91ce7f0fd1b74531951b51187c538df84a049f`  
		Last Modified: Fri, 11 Mar 2022 01:21:51 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1479d8719b8c480d4bb08970f0e36f7167fe7bec3820504e9b208532ca73ad9`  
		Last Modified: Fri, 11 Mar 2022 01:21:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1f0ceea8c14c17fee52cdbe03a751ace674f01ab93587adbab87b075ff44ccfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123004812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c563f0637efb118872c69265661422af08cbf9bd59d66bf05f1adf1e6855ff0`
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
# Fri, 11 Mar 2022 01:40:44 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:45 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:40:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:47 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:48 GMT
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
	-	`sha256:ba7418bd4a80bd5e5f9b31430eeb335cc3295df6547dcb53f68d415e7d2a16fc`  
		Last Modified: Fri, 11 Mar 2022 01:45:57 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20596863a9b6e75cf8a11a64163df54a226fd5fdddb5d1845debd92b7fc11f51`  
		Last Modified: Fri, 11 Mar 2022 01:45:57 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efe1da115837720b902fc86e3e183e29f39ee9b3d5ffe70ede594e0b4f24f0e`  
		Last Modified: Fri, 11 Mar 2022 01:45:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4e0c3bf0e87363fbcc603f20cc6b5744f22c52b7c476076546293565e62c725f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136562216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c765fa755a1c9a14517a2d4237d40c3e3f918d30b07db1c68e77fb8a5ef86d93`
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
# Fri, 11 Mar 2022 01:19:30 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:32 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:53 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:57 GMT
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
	-	`sha256:42c342ce2822718aac12e64bcb686dd687d39c4bf3be0df2f663ad59311b6442`  
		Last Modified: Fri, 11 Mar 2022 01:24:33 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1606d38719b289358ab38e3184a49552cfedce0c0e98dfecf8e547805cf329ab`  
		Last Modified: Fri, 11 Mar 2022 01:24:33 GMT  
		Size: 6.6 KB (6602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e449d1d2e45971ae9a9b272897ce77d3c6b640810cfb656333f919329ca098`  
		Last Modified: Fri, 11 Mar 2022 01:24:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.24`

```console
$ docker pull mariadb@sha256:65bc4d6acb5a5ba08f69654b727afca9057c8f66528f90e1f3f9544213343e4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.24` - linux; amd64

```console
$ docker pull mariadb@sha256:9082c559f2e3e582b35582c5b5e259ca9c4237219aabee51eae636e8dc00e911
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125680333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fab64ba115d1ad0ede48f65ede54e10bbe3f72970bf3afe11be6e3de6ecbe5`
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
# Fri, 11 Mar 2022 01:19:55 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:55 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:55 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:56 GMT
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
	-	`sha256:eb2a5e8f6ae43ddec8710950b73a5e2f4c86bd04d705dcd7ddd7969d175aa39c`  
		Last Modified: Fri, 11 Mar 2022 01:21:51 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691854f7300c7e1c9a48cbd66f91ce7f0fd1b74531951b51187c538df84a049f`  
		Last Modified: Fri, 11 Mar 2022 01:21:51 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1479d8719b8c480d4bb08970f0e36f7167fe7bec3820504e9b208532ca73ad9`  
		Last Modified: Fri, 11 Mar 2022 01:21:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1f0ceea8c14c17fee52cdbe03a751ace674f01ab93587adbab87b075ff44ccfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123004812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c563f0637efb118872c69265661422af08cbf9bd59d66bf05f1adf1e6855ff0`
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
# Fri, 11 Mar 2022 01:40:44 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:45 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:40:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:47 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:48 GMT
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
	-	`sha256:ba7418bd4a80bd5e5f9b31430eeb335cc3295df6547dcb53f68d415e7d2a16fc`  
		Last Modified: Fri, 11 Mar 2022 01:45:57 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20596863a9b6e75cf8a11a64163df54a226fd5fdddb5d1845debd92b7fc11f51`  
		Last Modified: Fri, 11 Mar 2022 01:45:57 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efe1da115837720b902fc86e3e183e29f39ee9b3d5ffe70ede594e0b4f24f0e`  
		Last Modified: Fri, 11 Mar 2022 01:45:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4e0c3bf0e87363fbcc603f20cc6b5744f22c52b7c476076546293565e62c725f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136562216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c765fa755a1c9a14517a2d4237d40c3e3f918d30b07db1c68e77fb8a5ef86d93`
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
# Fri, 11 Mar 2022 01:19:30 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:32 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:53 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:57 GMT
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
	-	`sha256:42c342ce2822718aac12e64bcb686dd687d39c4bf3be0df2f663ad59311b6442`  
		Last Modified: Fri, 11 Mar 2022 01:24:33 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1606d38719b289358ab38e3184a49552cfedce0c0e98dfecf8e547805cf329ab`  
		Last Modified: Fri, 11 Mar 2022 01:24:33 GMT  
		Size: 6.6 KB (6602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e449d1d2e45971ae9a9b272897ce77d3c6b640810cfb656333f919329ca098`  
		Last Modified: Fri, 11 Mar 2022 01:24:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.24-focal`

```console
$ docker pull mariadb@sha256:65bc4d6acb5a5ba08f69654b727afca9057c8f66528f90e1f3f9544213343e4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.24-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:9082c559f2e3e582b35582c5b5e259ca9c4237219aabee51eae636e8dc00e911
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125680333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fab64ba115d1ad0ede48f65ede54e10bbe3f72970bf3afe11be6e3de6ecbe5`
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
# Fri, 11 Mar 2022 01:19:55 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:55 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:55 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:56 GMT
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
	-	`sha256:eb2a5e8f6ae43ddec8710950b73a5e2f4c86bd04d705dcd7ddd7969d175aa39c`  
		Last Modified: Fri, 11 Mar 2022 01:21:51 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691854f7300c7e1c9a48cbd66f91ce7f0fd1b74531951b51187c538df84a049f`  
		Last Modified: Fri, 11 Mar 2022 01:21:51 GMT  
		Size: 6.6 KB (6601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1479d8719b8c480d4bb08970f0e36f7167fe7bec3820504e9b208532ca73ad9`  
		Last Modified: Fri, 11 Mar 2022 01:21:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1f0ceea8c14c17fee52cdbe03a751ace674f01ab93587adbab87b075ff44ccfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123004812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c563f0637efb118872c69265661422af08cbf9bd59d66bf05f1adf1e6855ff0`
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
# Fri, 11 Mar 2022 01:40:44 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:45 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:40:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:47 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:48 GMT
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
	-	`sha256:ba7418bd4a80bd5e5f9b31430eeb335cc3295df6547dcb53f68d415e7d2a16fc`  
		Last Modified: Fri, 11 Mar 2022 01:45:57 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20596863a9b6e75cf8a11a64163df54a226fd5fdddb5d1845debd92b7fc11f51`  
		Last Modified: Fri, 11 Mar 2022 01:45:57 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efe1da115837720b902fc86e3e183e29f39ee9b3d5ffe70ede594e0b4f24f0e`  
		Last Modified: Fri, 11 Mar 2022 01:45:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.24-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4e0c3bf0e87363fbcc603f20cc6b5744f22c52b7c476076546293565e62c725f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136562216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c765fa755a1c9a14517a2d4237d40c3e3f918d30b07db1c68e77fb8a5ef86d93`
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
# Fri, 11 Mar 2022 01:19:30 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:32 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.4.24/repo/ubuntu/ focal main
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 11 Mar 2022 01:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:53 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:57 GMT
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
	-	`sha256:42c342ce2822718aac12e64bcb686dd687d39c4bf3be0df2f663ad59311b6442`  
		Last Modified: Fri, 11 Mar 2022 01:24:33 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1606d38719b289358ab38e3184a49552cfedce0c0e98dfecf8e547805cf329ab`  
		Last Modified: Fri, 11 Mar 2022 01:24:33 GMT  
		Size: 6.6 KB (6602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e449d1d2e45971ae9a9b272897ce77d3c6b640810cfb656333f919329ca098`  
		Last Modified: Fri, 11 Mar 2022 01:24:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:c42d3644894f7439c682f66100573e32656df7021a4b87cc0e6962f172b11c4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:223494f1d9b4a7bcc19c8ae4e45628d303be36ed711a967f0720465f8615d324
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127924070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c3e204aa8a08c13b36415c670ef20228b6c39a61746526597fa04eb290994ee`
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
# Fri, 11 Mar 2022 01:19:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:52 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:52 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:52 GMT
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
	-	`sha256:5bcc81803c2ad0e2a3ce6a2ee587979714e46e5d2ad6bf64b00ec4788e6a5611`  
		Last Modified: Fri, 11 Mar 2022 01:21:35 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666b5e5eb25702e178cb64947f4675e54d41c4fe0693d06c76c500857518735f`  
		Last Modified: Fri, 11 Mar 2022 01:21:35 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1beb26dbab93d93d296806135884a053d99ce77e4e54ee42ef13afcef7b3fba9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125188377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfbc38faa626d23b727d6ed530d7753b81df5329d9013a71929aa0c888446500`
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
# Fri, 11 Mar 2022 01:40:34 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:35 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:36 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:37 GMT
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
	-	`sha256:a8444d8727338c5a505d2d3f74f27dc756b6cf13d96ad9dc56787ee7751456e7`  
		Last Modified: Fri, 11 Mar 2022 01:45:39 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8191c954bfe995d68c8866e280e6ba8403b1fee1a6756ca08f5688edd513c6c9`  
		Last Modified: Fri, 11 Mar 2022 01:45:38 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ec42b3ba6df501c09571e70c9a529529f4d7fc67e33a57ca75a8a036b8f563a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138783485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c19f23c290beb2682489aad41c34afd1b8338d46b67e49b528395188ff7a0608`
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
# Fri, 11 Mar 2022 01:18:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:00 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:16 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:21 GMT
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
	-	`sha256:69fb57a70b38aa22de52a3e042e03f44097248303b9da579acdeb67be6186668`  
		Last Modified: Fri, 11 Mar 2022 01:24:11 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09250efde7b71948954cbe92d241e2decb58d938d75e630c5476c34d7d7badf5`  
		Last Modified: Fri, 11 Mar 2022 01:24:10 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; s390x

```console
$ docker pull mariadb@sha256:f598bbc890b43df4ba4d7e98aeaf50a4130d8914a44d66845a488cd62dd186eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127198285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5979ac6c5ffcc4cb78378681e00680f2111741ee5d300218acca8b188c714b6`
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
# Fri, 11 Mar 2022 00:41:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:58 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:58 GMT
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
	-	`sha256:2f2929054126aed2ab06172531c12abf924521c377dec96f7968a747cc21cef1`  
		Last Modified: Fri, 11 Mar 2022 00:43:29 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f468c5ee1dca9451f4d66ec2d5dbca7b7512eae98bd4e9d53caf3e5afa1a5fc`  
		Last Modified: Fri, 11 Mar 2022 00:43:30 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:c42d3644894f7439c682f66100573e32656df7021a4b87cc0e6962f172b11c4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:223494f1d9b4a7bcc19c8ae4e45628d303be36ed711a967f0720465f8615d324
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127924070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c3e204aa8a08c13b36415c670ef20228b6c39a61746526597fa04eb290994ee`
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
# Fri, 11 Mar 2022 01:19:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:52 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:52 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:52 GMT
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
	-	`sha256:5bcc81803c2ad0e2a3ce6a2ee587979714e46e5d2ad6bf64b00ec4788e6a5611`  
		Last Modified: Fri, 11 Mar 2022 01:21:35 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666b5e5eb25702e178cb64947f4675e54d41c4fe0693d06c76c500857518735f`  
		Last Modified: Fri, 11 Mar 2022 01:21:35 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1beb26dbab93d93d296806135884a053d99ce77e4e54ee42ef13afcef7b3fba9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125188377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfbc38faa626d23b727d6ed530d7753b81df5329d9013a71929aa0c888446500`
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
# Fri, 11 Mar 2022 01:40:34 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:35 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:36 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:37 GMT
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
	-	`sha256:a8444d8727338c5a505d2d3f74f27dc756b6cf13d96ad9dc56787ee7751456e7`  
		Last Modified: Fri, 11 Mar 2022 01:45:39 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8191c954bfe995d68c8866e280e6ba8403b1fee1a6756ca08f5688edd513c6c9`  
		Last Modified: Fri, 11 Mar 2022 01:45:38 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ec42b3ba6df501c09571e70c9a529529f4d7fc67e33a57ca75a8a036b8f563a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138783485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c19f23c290beb2682489aad41c34afd1b8338d46b67e49b528395188ff7a0608`
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
# Fri, 11 Mar 2022 01:18:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:00 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:16 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:21 GMT
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
	-	`sha256:69fb57a70b38aa22de52a3e042e03f44097248303b9da579acdeb67be6186668`  
		Last Modified: Fri, 11 Mar 2022 01:24:11 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09250efde7b71948954cbe92d241e2decb58d938d75e630c5476c34d7d7badf5`  
		Last Modified: Fri, 11 Mar 2022 01:24:10 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:f598bbc890b43df4ba4d7e98aeaf50a4130d8914a44d66845a488cd62dd186eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127198285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5979ac6c5ffcc4cb78378681e00680f2111741ee5d300218acca8b188c714b6`
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
# Fri, 11 Mar 2022 00:41:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:58 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:58 GMT
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
	-	`sha256:2f2929054126aed2ab06172531c12abf924521c377dec96f7968a747cc21cef1`  
		Last Modified: Fri, 11 Mar 2022 00:43:29 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f468c5ee1dca9451f4d66ec2d5dbca7b7512eae98bd4e9d53caf3e5afa1a5fc`  
		Last Modified: Fri, 11 Mar 2022 00:43:30 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.15`

```console
$ docker pull mariadb@sha256:c42d3644894f7439c682f66100573e32656df7021a4b87cc0e6962f172b11c4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.15` - linux; amd64

```console
$ docker pull mariadb@sha256:223494f1d9b4a7bcc19c8ae4e45628d303be36ed711a967f0720465f8615d324
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127924070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c3e204aa8a08c13b36415c670ef20228b6c39a61746526597fa04eb290994ee`
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
# Fri, 11 Mar 2022 01:19:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:52 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:52 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:52 GMT
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
	-	`sha256:5bcc81803c2ad0e2a3ce6a2ee587979714e46e5d2ad6bf64b00ec4788e6a5611`  
		Last Modified: Fri, 11 Mar 2022 01:21:35 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666b5e5eb25702e178cb64947f4675e54d41c4fe0693d06c76c500857518735f`  
		Last Modified: Fri, 11 Mar 2022 01:21:35 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1beb26dbab93d93d296806135884a053d99ce77e4e54ee42ef13afcef7b3fba9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125188377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfbc38faa626d23b727d6ed530d7753b81df5329d9013a71929aa0c888446500`
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
# Fri, 11 Mar 2022 01:40:34 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:35 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:36 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:37 GMT
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
	-	`sha256:a8444d8727338c5a505d2d3f74f27dc756b6cf13d96ad9dc56787ee7751456e7`  
		Last Modified: Fri, 11 Mar 2022 01:45:39 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8191c954bfe995d68c8866e280e6ba8403b1fee1a6756ca08f5688edd513c6c9`  
		Last Modified: Fri, 11 Mar 2022 01:45:38 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ec42b3ba6df501c09571e70c9a529529f4d7fc67e33a57ca75a8a036b8f563a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138783485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c19f23c290beb2682489aad41c34afd1b8338d46b67e49b528395188ff7a0608`
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
# Fri, 11 Mar 2022 01:18:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:00 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:16 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:21 GMT
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
	-	`sha256:69fb57a70b38aa22de52a3e042e03f44097248303b9da579acdeb67be6186668`  
		Last Modified: Fri, 11 Mar 2022 01:24:11 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09250efde7b71948954cbe92d241e2decb58d938d75e630c5476c34d7d7badf5`  
		Last Modified: Fri, 11 Mar 2022 01:24:10 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15` - linux; s390x

```console
$ docker pull mariadb@sha256:f598bbc890b43df4ba4d7e98aeaf50a4130d8914a44d66845a488cd62dd186eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127198285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5979ac6c5ffcc4cb78378681e00680f2111741ee5d300218acca8b188c714b6`
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
# Fri, 11 Mar 2022 00:41:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:58 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:58 GMT
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
	-	`sha256:2f2929054126aed2ab06172531c12abf924521c377dec96f7968a747cc21cef1`  
		Last Modified: Fri, 11 Mar 2022 00:43:29 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f468c5ee1dca9451f4d66ec2d5dbca7b7512eae98bd4e9d53caf3e5afa1a5fc`  
		Last Modified: Fri, 11 Mar 2022 00:43:30 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.15-focal`

```console
$ docker pull mariadb@sha256:c42d3644894f7439c682f66100573e32656df7021a4b87cc0e6962f172b11c4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.5.15-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:223494f1d9b4a7bcc19c8ae4e45628d303be36ed711a967f0720465f8615d324
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127924070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c3e204aa8a08c13b36415c670ef20228b6c39a61746526597fa04eb290994ee`
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
# Fri, 11 Mar 2022 01:19:52 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:52 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:52 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:52 GMT
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
	-	`sha256:5bcc81803c2ad0e2a3ce6a2ee587979714e46e5d2ad6bf64b00ec4788e6a5611`  
		Last Modified: Fri, 11 Mar 2022 01:21:35 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666b5e5eb25702e178cb64947f4675e54d41c4fe0693d06c76c500857518735f`  
		Last Modified: Fri, 11 Mar 2022 01:21:35 GMT  
		Size: 6.6 KB (6599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:1beb26dbab93d93d296806135884a053d99ce77e4e54ee42ef13afcef7b3fba9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125188377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfbc38faa626d23b727d6ed530d7753b81df5329d9013a71929aa0c888446500`
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
# Fri, 11 Mar 2022 01:40:34 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:35 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:36 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:37 GMT
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
	-	`sha256:a8444d8727338c5a505d2d3f74f27dc756b6cf13d96ad9dc56787ee7751456e7`  
		Last Modified: Fri, 11 Mar 2022 01:45:39 GMT  
		Size: 3.5 KB (3495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8191c954bfe995d68c8866e280e6ba8403b1fee1a6756ca08f5688edd513c6c9`  
		Last Modified: Fri, 11 Mar 2022 01:45:38 GMT  
		Size: 6.6 KB (6605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:ec42b3ba6df501c09571e70c9a529529f4d7fc67e33a57ca75a8a036b8f563a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138783485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c19f23c290beb2682489aad41c34afd1b8338d46b67e49b528395188ff7a0608`
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
# Fri, 11 Mar 2022 01:18:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:00 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:16 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:21 GMT
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
	-	`sha256:69fb57a70b38aa22de52a3e042e03f44097248303b9da579acdeb67be6186668`  
		Last Modified: Fri, 11 Mar 2022 01:24:11 GMT  
		Size: 3.5 KB (3491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09250efde7b71948954cbe92d241e2decb58d938d75e630c5476c34d7d7badf5`  
		Last Modified: Fri, 11 Mar 2022 01:24:10 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.15-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:f598bbc890b43df4ba4d7e98aeaf50a4130d8914a44d66845a488cd62dd186eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127198285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5979ac6c5ffcc4cb78378681e00680f2111741ee5d300218acca8b188c714b6`
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
# Fri, 11 Mar 2022 00:41:58 GMT
COPY file:64ef9edc0b6d64f19618d1f2ffc8c4cc3c2a1e0e90591a283cdeda8bbe9f9a14 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:58 GMT
COPY file:e72c712eebf14292d0fd72b8da0ba253af0c5757248c6dab17a29322f07d9458 in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:58 GMT
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
	-	`sha256:2f2929054126aed2ab06172531c12abf924521c377dec96f7968a747cc21cef1`  
		Last Modified: Fri, 11 Mar 2022 00:43:29 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f468c5ee1dca9451f4d66ec2d5dbca7b7512eae98bd4e9d53caf3e5afa1a5fc`  
		Last Modified: Fri, 11 Mar 2022 00:43:30 GMT  
		Size: 6.6 KB (6603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:4e8af11e77a6bf2a8407262964baf7f9e0f25963ad8e696b83169176169c9053
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:2c837199234076a5b4ec9dded3d53580ea26ab1fcb7be722350967d5accfe07d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128170981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a670b82df1f69043ae85e6d87806ea2e03c17c69d4e4b2880d3a7c8ff6ff8515`
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
# Fri, 11 Mar 2022 01:19:49 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:49 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:49 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:49 GMT
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
	-	`sha256:c96b1cf971c6a8fec98480268923d24ad07770d46aa37533451fc96a7944f114`  
		Last Modified: Fri, 11 Mar 2022 01:21:19 GMT  
		Size: 3.5 KB (3482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490f49b6e28bb243133ceffef81bd9d667c9c5522c328696ec487a2ef69c8bc7`  
		Last Modified: Fri, 11 Mar 2022 01:21:19 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bf75f3fe1854ec5d2fb5a26c849a8c38cdf4dc54de08708d8307f4c4bb2e88ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125272276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ea4756d8818752cd44bfb64d9a47d67a39f420411bfa1a948c2012ee0510d4`
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
# Fri, 11 Mar 2022 01:40:24 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:25 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:26 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:27 GMT
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
	-	`sha256:9350dc6f7ba94bca743049d0e0c5f13710093ab6913826f6c0ab7cf101af1c83`  
		Last Modified: Fri, 11 Mar 2022 01:45:20 GMT  
		Size: 3.5 KB (3483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b3d9398899f254aeb2e421e2527a6ed6395f1802598e42446c43bd16e4f99b`  
		Last Modified: Fri, 11 Mar 2022 01:45:20 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c44b94effdf1410fac1394602b8ba07ecf3eedbd85b72081f34f96845d44a4a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138843552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ee27e6be8a98a66e0e6204c417bb19f74b95e3b0e5b5824de702f3d7d10e9a8`
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
# Fri, 11 Mar 2022 01:18:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:18:21 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:18:33 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:18:43 GMT
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
	-	`sha256:53c9a122b15ae7aefcfbb3b6b6ffd49d1c95e0e0b59f6044eee5f43c5bb182dc`  
		Last Modified: Fri, 11 Mar 2022 01:23:50 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e3aed20e83b1f8b1c92f3851d4998c1b20957a9e3434e09d2c079e9c5c434f`  
		Last Modified: Fri, 11 Mar 2022 01:23:50 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; s390x

```console
$ docker pull mariadb@sha256:5b5983a52ebf77c3a258e331930caaf8a680c707e9657647346387443abcc0e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127224455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a91cf542d833c9850e532e30f6bf785a1e51090ccf4cdc90c481553f584af7`
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
# Fri, 11 Mar 2022 00:41:50 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:50 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:51 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:51 GMT
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
	-	`sha256:793b084b900358546cab6a5f1084dd9022d7d89d2b6983a42b692e4702e2f626`  
		Last Modified: Fri, 11 Mar 2022 00:43:19 GMT  
		Size: 3.5 KB (3485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892c7ac5a93c20f16a5628ab27a3c75062e8cf43b0dada8984d31383c923e2cc`  
		Last Modified: Fri, 11 Mar 2022 00:43:19 GMT  
		Size: 6.6 KB (6606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:4e8af11e77a6bf2a8407262964baf7f9e0f25963ad8e696b83169176169c9053
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:2c837199234076a5b4ec9dded3d53580ea26ab1fcb7be722350967d5accfe07d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128170981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a670b82df1f69043ae85e6d87806ea2e03c17c69d4e4b2880d3a7c8ff6ff8515`
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
# Fri, 11 Mar 2022 01:19:49 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:49 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:49 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:49 GMT
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
	-	`sha256:c96b1cf971c6a8fec98480268923d24ad07770d46aa37533451fc96a7944f114`  
		Last Modified: Fri, 11 Mar 2022 01:21:19 GMT  
		Size: 3.5 KB (3482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490f49b6e28bb243133ceffef81bd9d667c9c5522c328696ec487a2ef69c8bc7`  
		Last Modified: Fri, 11 Mar 2022 01:21:19 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bf75f3fe1854ec5d2fb5a26c849a8c38cdf4dc54de08708d8307f4c4bb2e88ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125272276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ea4756d8818752cd44bfb64d9a47d67a39f420411bfa1a948c2012ee0510d4`
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
# Fri, 11 Mar 2022 01:40:24 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:25 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:26 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:27 GMT
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
	-	`sha256:9350dc6f7ba94bca743049d0e0c5f13710093ab6913826f6c0ab7cf101af1c83`  
		Last Modified: Fri, 11 Mar 2022 01:45:20 GMT  
		Size: 3.5 KB (3483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b3d9398899f254aeb2e421e2527a6ed6395f1802598e42446c43bd16e4f99b`  
		Last Modified: Fri, 11 Mar 2022 01:45:20 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c44b94effdf1410fac1394602b8ba07ecf3eedbd85b72081f34f96845d44a4a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138843552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ee27e6be8a98a66e0e6204c417bb19f74b95e3b0e5b5824de702f3d7d10e9a8`
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
# Fri, 11 Mar 2022 01:18:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:18:21 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:18:33 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:18:43 GMT
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
	-	`sha256:53c9a122b15ae7aefcfbb3b6b6ffd49d1c95e0e0b59f6044eee5f43c5bb182dc`  
		Last Modified: Fri, 11 Mar 2022 01:23:50 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e3aed20e83b1f8b1c92f3851d4998c1b20957a9e3434e09d2c079e9c5c434f`  
		Last Modified: Fri, 11 Mar 2022 01:23:50 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:5b5983a52ebf77c3a258e331930caaf8a680c707e9657647346387443abcc0e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127224455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a91cf542d833c9850e532e30f6bf785a1e51090ccf4cdc90c481553f584af7`
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
# Fri, 11 Mar 2022 00:41:50 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:50 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:51 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:51 GMT
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
	-	`sha256:793b084b900358546cab6a5f1084dd9022d7d89d2b6983a42b692e4702e2f626`  
		Last Modified: Fri, 11 Mar 2022 00:43:19 GMT  
		Size: 3.5 KB (3485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892c7ac5a93c20f16a5628ab27a3c75062e8cf43b0dada8984d31383c923e2cc`  
		Last Modified: Fri, 11 Mar 2022 00:43:19 GMT  
		Size: 6.6 KB (6606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.7`

```console
$ docker pull mariadb@sha256:4e8af11e77a6bf2a8407262964baf7f9e0f25963ad8e696b83169176169c9053
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.7` - linux; amd64

```console
$ docker pull mariadb@sha256:2c837199234076a5b4ec9dded3d53580ea26ab1fcb7be722350967d5accfe07d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128170981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a670b82df1f69043ae85e6d87806ea2e03c17c69d4e4b2880d3a7c8ff6ff8515`
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
# Fri, 11 Mar 2022 01:19:49 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:49 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:49 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:49 GMT
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
	-	`sha256:c96b1cf971c6a8fec98480268923d24ad07770d46aa37533451fc96a7944f114`  
		Last Modified: Fri, 11 Mar 2022 01:21:19 GMT  
		Size: 3.5 KB (3482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490f49b6e28bb243133ceffef81bd9d667c9c5522c328696ec487a2ef69c8bc7`  
		Last Modified: Fri, 11 Mar 2022 01:21:19 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bf75f3fe1854ec5d2fb5a26c849a8c38cdf4dc54de08708d8307f4c4bb2e88ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125272276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ea4756d8818752cd44bfb64d9a47d67a39f420411bfa1a948c2012ee0510d4`
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
# Fri, 11 Mar 2022 01:40:24 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:25 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:26 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:27 GMT
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
	-	`sha256:9350dc6f7ba94bca743049d0e0c5f13710093ab6913826f6c0ab7cf101af1c83`  
		Last Modified: Fri, 11 Mar 2022 01:45:20 GMT  
		Size: 3.5 KB (3483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b3d9398899f254aeb2e421e2527a6ed6395f1802598e42446c43bd16e4f99b`  
		Last Modified: Fri, 11 Mar 2022 01:45:20 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c44b94effdf1410fac1394602b8ba07ecf3eedbd85b72081f34f96845d44a4a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138843552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ee27e6be8a98a66e0e6204c417bb19f74b95e3b0e5b5824de702f3d7d10e9a8`
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
# Fri, 11 Mar 2022 01:18:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:18:21 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:18:33 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:18:43 GMT
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
	-	`sha256:53c9a122b15ae7aefcfbb3b6b6ffd49d1c95e0e0b59f6044eee5f43c5bb182dc`  
		Last Modified: Fri, 11 Mar 2022 01:23:50 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e3aed20e83b1f8b1c92f3851d4998c1b20957a9e3434e09d2c079e9c5c434f`  
		Last Modified: Fri, 11 Mar 2022 01:23:50 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7` - linux; s390x

```console
$ docker pull mariadb@sha256:5b5983a52ebf77c3a258e331930caaf8a680c707e9657647346387443abcc0e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127224455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a91cf542d833c9850e532e30f6bf785a1e51090ccf4cdc90c481553f584af7`
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
# Fri, 11 Mar 2022 00:41:50 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:50 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:51 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:51 GMT
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
	-	`sha256:793b084b900358546cab6a5f1084dd9022d7d89d2b6983a42b692e4702e2f626`  
		Last Modified: Fri, 11 Mar 2022 00:43:19 GMT  
		Size: 3.5 KB (3485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892c7ac5a93c20f16a5628ab27a3c75062e8cf43b0dada8984d31383c923e2cc`  
		Last Modified: Fri, 11 Mar 2022 00:43:19 GMT  
		Size: 6.6 KB (6606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.7-focal`

```console
$ docker pull mariadb@sha256:4e8af11e77a6bf2a8407262964baf7f9e0f25963ad8e696b83169176169c9053
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.6.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:2c837199234076a5b4ec9dded3d53580ea26ab1fcb7be722350967d5accfe07d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128170981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a670b82df1f69043ae85e6d87806ea2e03c17c69d4e4b2880d3a7c8ff6ff8515`
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
# Fri, 11 Mar 2022 01:19:49 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:49 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:49 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:49 GMT
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
	-	`sha256:c96b1cf971c6a8fec98480268923d24ad07770d46aa37533451fc96a7944f114`  
		Last Modified: Fri, 11 Mar 2022 01:21:19 GMT  
		Size: 3.5 KB (3482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490f49b6e28bb243133ceffef81bd9d667c9c5522c328696ec487a2ef69c8bc7`  
		Last Modified: Fri, 11 Mar 2022 01:21:19 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bf75f3fe1854ec5d2fb5a26c849a8c38cdf4dc54de08708d8307f4c4bb2e88ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125272276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ea4756d8818752cd44bfb64d9a47d67a39f420411bfa1a948c2012ee0510d4`
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
# Fri, 11 Mar 2022 01:40:24 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:25 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:26 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:27 GMT
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
	-	`sha256:9350dc6f7ba94bca743049d0e0c5f13710093ab6913826f6c0ab7cf101af1c83`  
		Last Modified: Fri, 11 Mar 2022 01:45:20 GMT  
		Size: 3.5 KB (3483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b3d9398899f254aeb2e421e2527a6ed6395f1802598e42446c43bd16e4f99b`  
		Last Modified: Fri, 11 Mar 2022 01:45:20 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c44b94effdf1410fac1394602b8ba07ecf3eedbd85b72081f34f96845d44a4a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138843552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ee27e6be8a98a66e0e6204c417bb19f74b95e3b0e5b5824de702f3d7d10e9a8`
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
# Fri, 11 Mar 2022 01:18:19 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:18:21 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:18:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:18:33 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:18:43 GMT
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
	-	`sha256:53c9a122b15ae7aefcfbb3b6b6ffd49d1c95e0e0b59f6044eee5f43c5bb182dc`  
		Last Modified: Fri, 11 Mar 2022 01:23:50 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e3aed20e83b1f8b1c92f3851d4998c1b20957a9e3434e09d2c079e9c5c434f`  
		Last Modified: Fri, 11 Mar 2022 01:23:50 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:5b5983a52ebf77c3a258e331930caaf8a680c707e9657647346387443abcc0e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127224455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a91cf542d833c9850e532e30f6bf785a1e51090ccf4cdc90c481553f584af7`
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
# Fri, 11 Mar 2022 00:41:50 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:50 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:51 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:51 GMT
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
	-	`sha256:793b084b900358546cab6a5f1084dd9022d7d89d2b6983a42b692e4702e2f626`  
		Last Modified: Fri, 11 Mar 2022 00:43:19 GMT  
		Size: 3.5 KB (3485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892c7ac5a93c20f16a5628ab27a3c75062e8cf43b0dada8984d31383c923e2cc`  
		Last Modified: Fri, 11 Mar 2022 00:43:19 GMT  
		Size: 6.6 KB (6606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7`

```console
$ docker pull mariadb@sha256:736606c3decd9b95dd8c1ee68c3e2b7e53af9e41135f6c833cd69a5eb268355e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7` - linux; amd64

```console
$ docker pull mariadb@sha256:c1988f7cf41786b77bccd23891d1afa2f83c999f4b303bfcd5f333e934b51cc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128669741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5dd1ac0b00e78cf6f5d6152b3d37a6fbb2c9b209ea58f4d205499ed4801f305`
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
# Fri, 11 Mar 2022 01:19:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:46 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:46 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:46 GMT
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
	-	`sha256:621fa3528f37c800eddf5424ae7b35ab6f823af267c6baeb9bb20867600552de`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 3.5 KB (3483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65fa0799f33d7ab55dfbaa9cf8fb881edd3f75a9d4b6f1ad76627416769b1`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:954bc8268e746a9a4b135304d85a60a99e235a79830149f76ef0439f4157a675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125722158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38051c4e5d39b816a571729967488805c4415d7b5460e36f77392cc98a45536c`
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
# Fri, 11 Mar 2022 01:40:12 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:13 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:14 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:15 GMT
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
	-	`sha256:f1d3feb849615542564db737270cb86f87c79472cd92732650492de686bc49e2`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 3.5 KB (3485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666c07e1f7c22ebd3ff693f3a2ec21991f99d923c68a16e7a76bd88947b237b`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d35dfc2be87294ad02c377b285cde99170be7ac251c0021609d702c2a68d5daf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139539786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5bbff5e51ec39ca2817bce7fd70b2384df0a6434a3734d736a877584113f4bc`
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
# Fri, 11 Mar 2022 01:17:39 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:17:42 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:17:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:18:02 GMT
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
	-	`sha256:1f5a705aa51ed4df01e6504a076cb8470714f75d46f7c06c16a34c8e4c3b10b6`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410180f3ffbc90843c959dbca9182e9b4b16783c3e9abf15e90ef46548c09416`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7` - linux; s390x

```console
$ docker pull mariadb@sha256:f57e663953b1774cf5116c02dd9a4f3b3a9e7f9199296c42fd02e7c94b1efd7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127723395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226ef0fff8e8f22de2ccb61a5a90d170ae551d3d68753c08572781c3d9afdd9b`
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
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:41 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:41 GMT
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
	-	`sha256:56572738f165202d0ca50d879a5b75c73959f04bb1e66d39722a40849517261f`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1c1e0cca65f889f547f42513cc37e2ca3c6a988fef8132fa46bc00c73e0b8a`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7-focal`

```console
$ docker pull mariadb@sha256:736606c3decd9b95dd8c1ee68c3e2b7e53af9e41135f6c833cd69a5eb268355e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c1988f7cf41786b77bccd23891d1afa2f83c999f4b303bfcd5f333e934b51cc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128669741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5dd1ac0b00e78cf6f5d6152b3d37a6fbb2c9b209ea58f4d205499ed4801f305`
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
# Fri, 11 Mar 2022 01:19:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:46 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:46 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:46 GMT
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
	-	`sha256:621fa3528f37c800eddf5424ae7b35ab6f823af267c6baeb9bb20867600552de`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 3.5 KB (3483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65fa0799f33d7ab55dfbaa9cf8fb881edd3f75a9d4b6f1ad76627416769b1`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:954bc8268e746a9a4b135304d85a60a99e235a79830149f76ef0439f4157a675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125722158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38051c4e5d39b816a571729967488805c4415d7b5460e36f77392cc98a45536c`
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
# Fri, 11 Mar 2022 01:40:12 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:13 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:14 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:15 GMT
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
	-	`sha256:f1d3feb849615542564db737270cb86f87c79472cd92732650492de686bc49e2`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 3.5 KB (3485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666c07e1f7c22ebd3ff693f3a2ec21991f99d923c68a16e7a76bd88947b237b`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d35dfc2be87294ad02c377b285cde99170be7ac251c0021609d702c2a68d5daf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139539786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5bbff5e51ec39ca2817bce7fd70b2384df0a6434a3734d736a877584113f4bc`
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
# Fri, 11 Mar 2022 01:17:39 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:17:42 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:17:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:18:02 GMT
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
	-	`sha256:1f5a705aa51ed4df01e6504a076cb8470714f75d46f7c06c16a34c8e4c3b10b6`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410180f3ffbc90843c959dbca9182e9b4b16783c3e9abf15e90ef46548c09416`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:f57e663953b1774cf5116c02dd9a4f3b3a9e7f9199296c42fd02e7c94b1efd7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127723395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226ef0fff8e8f22de2ccb61a5a90d170ae551d3d68753c08572781c3d9afdd9b`
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
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:41 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:41 GMT
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
	-	`sha256:56572738f165202d0ca50d879a5b75c73959f04bb1e66d39722a40849517261f`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1c1e0cca65f889f547f42513cc37e2ca3c6a988fef8132fa46bc00c73e0b8a`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.3`

```console
$ docker pull mariadb@sha256:736606c3decd9b95dd8c1ee68c3e2b7e53af9e41135f6c833cd69a5eb268355e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.3` - linux; amd64

```console
$ docker pull mariadb@sha256:c1988f7cf41786b77bccd23891d1afa2f83c999f4b303bfcd5f333e934b51cc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128669741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5dd1ac0b00e78cf6f5d6152b3d37a6fbb2c9b209ea58f4d205499ed4801f305`
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
# Fri, 11 Mar 2022 01:19:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:46 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:46 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:46 GMT
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
	-	`sha256:621fa3528f37c800eddf5424ae7b35ab6f823af267c6baeb9bb20867600552de`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 3.5 KB (3483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65fa0799f33d7ab55dfbaa9cf8fb881edd3f75a9d4b6f1ad76627416769b1`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:954bc8268e746a9a4b135304d85a60a99e235a79830149f76ef0439f4157a675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125722158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38051c4e5d39b816a571729967488805c4415d7b5460e36f77392cc98a45536c`
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
# Fri, 11 Mar 2022 01:40:12 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:13 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:14 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:15 GMT
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
	-	`sha256:f1d3feb849615542564db737270cb86f87c79472cd92732650492de686bc49e2`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 3.5 KB (3485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666c07e1f7c22ebd3ff693f3a2ec21991f99d923c68a16e7a76bd88947b237b`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d35dfc2be87294ad02c377b285cde99170be7ac251c0021609d702c2a68d5daf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139539786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5bbff5e51ec39ca2817bce7fd70b2384df0a6434a3734d736a877584113f4bc`
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
# Fri, 11 Mar 2022 01:17:39 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:17:42 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:17:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:18:02 GMT
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
	-	`sha256:1f5a705aa51ed4df01e6504a076cb8470714f75d46f7c06c16a34c8e4c3b10b6`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410180f3ffbc90843c959dbca9182e9b4b16783c3e9abf15e90ef46548c09416`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3` - linux; s390x

```console
$ docker pull mariadb@sha256:f57e663953b1774cf5116c02dd9a4f3b3a9e7f9199296c42fd02e7c94b1efd7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127723395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226ef0fff8e8f22de2ccb61a5a90d170ae551d3d68753c08572781c3d9afdd9b`
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
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:41 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:41 GMT
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
	-	`sha256:56572738f165202d0ca50d879a5b75c73959f04bb1e66d39722a40849517261f`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1c1e0cca65f889f547f42513cc37e2ca3c6a988fef8132fa46bc00c73e0b8a`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.7.3-focal`

```console
$ docker pull mariadb@sha256:736606c3decd9b95dd8c1ee68c3e2b7e53af9e41135f6c833cd69a5eb268355e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.7.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c1988f7cf41786b77bccd23891d1afa2f83c999f4b303bfcd5f333e934b51cc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128669741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5dd1ac0b00e78cf6f5d6152b3d37a6fbb2c9b209ea58f4d205499ed4801f305`
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
# Fri, 11 Mar 2022 01:19:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:46 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:46 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:46 GMT
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
	-	`sha256:621fa3528f37c800eddf5424ae7b35ab6f823af267c6baeb9bb20867600552de`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 3.5 KB (3483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65fa0799f33d7ab55dfbaa9cf8fb881edd3f75a9d4b6f1ad76627416769b1`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:954bc8268e746a9a4b135304d85a60a99e235a79830149f76ef0439f4157a675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125722158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38051c4e5d39b816a571729967488805c4415d7b5460e36f77392cc98a45536c`
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
# Fri, 11 Mar 2022 01:40:12 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:13 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:14 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:15 GMT
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
	-	`sha256:f1d3feb849615542564db737270cb86f87c79472cd92732650492de686bc49e2`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 3.5 KB (3485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666c07e1f7c22ebd3ff693f3a2ec21991f99d923c68a16e7a76bd88947b237b`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d35dfc2be87294ad02c377b285cde99170be7ac251c0021609d702c2a68d5daf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139539786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5bbff5e51ec39ca2817bce7fd70b2384df0a6434a3734d736a877584113f4bc`
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
# Fri, 11 Mar 2022 01:17:39 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:17:42 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:17:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:18:02 GMT
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
	-	`sha256:1f5a705aa51ed4df01e6504a076cb8470714f75d46f7c06c16a34c8e4c3b10b6`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410180f3ffbc90843c959dbca9182e9b4b16783c3e9abf15e90ef46548c09416`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.7.3-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:f57e663953b1774cf5116c02dd9a4f3b3a9e7f9199296c42fd02e7c94b1efd7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127723395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226ef0fff8e8f22de2ccb61a5a90d170ae551d3d68753c08572781c3d9afdd9b`
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
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:41 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:41 GMT
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
	-	`sha256:56572738f165202d0ca50d879a5b75c73959f04bb1e66d39722a40849517261f`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1c1e0cca65f889f547f42513cc37e2ca3c6a988fef8132fa46bc00c73e0b8a`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8-rc`

```console
$ docker pull mariadb@sha256:ca5c3b079c5692dac7e28b378a95acef02df934004bf6379aff9cebdf6ca8359
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:b82fe107c8317aa03b87e30caf45453266dbdbbf54a488706e7661a98c40a054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128579598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19060cfc0fda93917faf594988bc544889cd727b8284e3174ec17d52115666ed`
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
# Fri, 11 Mar 2022 01:19:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:43 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:43 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:43 GMT
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
	-	`sha256:c12d41077524a3c495250dd259a0e95e2ff901432cb1a880f7ac83cb84ccf687`  
		Last Modified: Fri, 11 Mar 2022 01:20:36 GMT  
		Size: 3.5 KB (3482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f598f32e5ec75c4ebefbf9c5f5c7ca8899ddd449679ceebc82e62323afa5847`  
		Last Modified: Fri, 11 Mar 2022 01:20:36 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:16f2ed81ce8652e33785b7047e21d2175b8362d13b52b842a8db950f94faf72f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125653262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47ee2e1d34e81670dff8fc73abe02f9d061ddebd2f674daab048513a6e45ad94`
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
# Fri, 11 Mar 2022 01:40:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:03 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:04 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:05 GMT
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
	-	`sha256:f3fdf302acfcb08391bbf4148316e40381cc5887c38f20f2cf9e8a4ddf57b38d`  
		Last Modified: Fri, 11 Mar 2022 01:44:30 GMT  
		Size: 3.5 KB (3486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4623a9a008ea67a14f101ace4fccc054dba48ac54dd6647a8d45cf741cef5d6c`  
		Last Modified: Fri, 11 Mar 2022 01:44:30 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:82b14dad2c02fb6b4e989a0d1b45e6b2cecb6672b01c055407cc1c52138695ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139622015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65074644ddf3d765ba23a1d52c7b39c70db5503ab3008e4bceb9f59ca6bec207`
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
# Fri, 11 Mar 2022 01:16:59 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:17:01 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:17:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:17:14 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:17:22 GMT
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
	-	`sha256:0803f70e4a7b9d678a26db21defccbaf848e9821ba9273b771b09cf2cb9ba6b7`  
		Last Modified: Fri, 11 Mar 2022 01:22:51 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508417a0638a97a111ce300a430612018a9d14acf46cebdd668bf3973b8005f3`  
		Last Modified: Fri, 11 Mar 2022 01:22:51 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:5198280ae34c2cd20bc45ee73e0b634418ba548692cac4fcdb5f9baa30d6c40e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127688007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f371c38a5139c23dc3062cd9c0bae757101b4d648e893d3a964da4e964b662e`
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
# Fri, 11 Mar 2022 00:41:33 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:33 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:33 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:33 GMT
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
	-	`sha256:b5cb7c2c2a7d570a43e161df06a8115d2023faa173c62ed233d42fe6ac82b39d`  
		Last Modified: Fri, 11 Mar 2022 00:42:49 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c406a4a03e2af0d6722d2a61e6c55b05efb56fcd43ee81aa1c51019c328b019`  
		Last Modified: Fri, 11 Mar 2022 00:42:49 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8-rc-focal`

```console
$ docker pull mariadb@sha256:ca5c3b079c5692dac7e28b378a95acef02df934004bf6379aff9cebdf6ca8359
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8-rc-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:b82fe107c8317aa03b87e30caf45453266dbdbbf54a488706e7661a98c40a054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128579598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19060cfc0fda93917faf594988bc544889cd727b8284e3174ec17d52115666ed`
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
# Fri, 11 Mar 2022 01:19:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:43 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:43 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:43 GMT
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
	-	`sha256:c12d41077524a3c495250dd259a0e95e2ff901432cb1a880f7ac83cb84ccf687`  
		Last Modified: Fri, 11 Mar 2022 01:20:36 GMT  
		Size: 3.5 KB (3482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f598f32e5ec75c4ebefbf9c5f5c7ca8899ddd449679ceebc82e62323afa5847`  
		Last Modified: Fri, 11 Mar 2022 01:20:36 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:16f2ed81ce8652e33785b7047e21d2175b8362d13b52b842a8db950f94faf72f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125653262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47ee2e1d34e81670dff8fc73abe02f9d061ddebd2f674daab048513a6e45ad94`
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
# Fri, 11 Mar 2022 01:40:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:03 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:04 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:05 GMT
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
	-	`sha256:f3fdf302acfcb08391bbf4148316e40381cc5887c38f20f2cf9e8a4ddf57b38d`  
		Last Modified: Fri, 11 Mar 2022 01:44:30 GMT  
		Size: 3.5 KB (3486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4623a9a008ea67a14f101ace4fccc054dba48ac54dd6647a8d45cf741cef5d6c`  
		Last Modified: Fri, 11 Mar 2022 01:44:30 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:82b14dad2c02fb6b4e989a0d1b45e6b2cecb6672b01c055407cc1c52138695ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139622015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65074644ddf3d765ba23a1d52c7b39c70db5503ab3008e4bceb9f59ca6bec207`
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
# Fri, 11 Mar 2022 01:16:59 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:17:01 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:17:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:17:14 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:17:22 GMT
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
	-	`sha256:0803f70e4a7b9d678a26db21defccbaf848e9821ba9273b771b09cf2cb9ba6b7`  
		Last Modified: Fri, 11 Mar 2022 01:22:51 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508417a0638a97a111ce300a430612018a9d14acf46cebdd668bf3973b8005f3`  
		Last Modified: Fri, 11 Mar 2022 01:22:51 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8-rc-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:5198280ae34c2cd20bc45ee73e0b634418ba548692cac4fcdb5f9baa30d6c40e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127688007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f371c38a5139c23dc3062cd9c0bae757101b4d648e893d3a964da4e964b662e`
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
# Fri, 11 Mar 2022 00:41:33 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:33 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:33 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:33 GMT
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
	-	`sha256:b5cb7c2c2a7d570a43e161df06a8115d2023faa173c62ed233d42fe6ac82b39d`  
		Last Modified: Fri, 11 Mar 2022 00:42:49 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c406a4a03e2af0d6722d2a61e6c55b05efb56fcd43ee81aa1c51019c328b019`  
		Last Modified: Fri, 11 Mar 2022 00:42:49 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.2-rc`

```console
$ docker pull mariadb@sha256:ca5c3b079c5692dac7e28b378a95acef02df934004bf6379aff9cebdf6ca8359
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8.2-rc` - linux; amd64

```console
$ docker pull mariadb@sha256:b82fe107c8317aa03b87e30caf45453266dbdbbf54a488706e7661a98c40a054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128579598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19060cfc0fda93917faf594988bc544889cd727b8284e3174ec17d52115666ed`
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
# Fri, 11 Mar 2022 01:19:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:43 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:43 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:43 GMT
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
	-	`sha256:c12d41077524a3c495250dd259a0e95e2ff901432cb1a880f7ac83cb84ccf687`  
		Last Modified: Fri, 11 Mar 2022 01:20:36 GMT  
		Size: 3.5 KB (3482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f598f32e5ec75c4ebefbf9c5f5c7ca8899ddd449679ceebc82e62323afa5847`  
		Last Modified: Fri, 11 Mar 2022 01:20:36 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:16f2ed81ce8652e33785b7047e21d2175b8362d13b52b842a8db950f94faf72f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125653262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47ee2e1d34e81670dff8fc73abe02f9d061ddebd2f674daab048513a6e45ad94`
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
# Fri, 11 Mar 2022 01:40:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:03 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:04 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:05 GMT
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
	-	`sha256:f3fdf302acfcb08391bbf4148316e40381cc5887c38f20f2cf9e8a4ddf57b38d`  
		Last Modified: Fri, 11 Mar 2022 01:44:30 GMT  
		Size: 3.5 KB (3486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4623a9a008ea67a14f101ace4fccc054dba48ac54dd6647a8d45cf741cef5d6c`  
		Last Modified: Fri, 11 Mar 2022 01:44:30 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:82b14dad2c02fb6b4e989a0d1b45e6b2cecb6672b01c055407cc1c52138695ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139622015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65074644ddf3d765ba23a1d52c7b39c70db5503ab3008e4bceb9f59ca6bec207`
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
# Fri, 11 Mar 2022 01:16:59 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:17:01 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:17:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:17:14 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:17:22 GMT
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
	-	`sha256:0803f70e4a7b9d678a26db21defccbaf848e9821ba9273b771b09cf2cb9ba6b7`  
		Last Modified: Fri, 11 Mar 2022 01:22:51 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508417a0638a97a111ce300a430612018a9d14acf46cebdd668bf3973b8005f3`  
		Last Modified: Fri, 11 Mar 2022 01:22:51 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc` - linux; s390x

```console
$ docker pull mariadb@sha256:5198280ae34c2cd20bc45ee73e0b634418ba548692cac4fcdb5f9baa30d6c40e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127688007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f371c38a5139c23dc3062cd9c0bae757101b4d648e893d3a964da4e964b662e`
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
# Fri, 11 Mar 2022 00:41:33 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:33 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:33 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:33 GMT
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
	-	`sha256:b5cb7c2c2a7d570a43e161df06a8115d2023faa173c62ed233d42fe6ac82b39d`  
		Last Modified: Fri, 11 Mar 2022 00:42:49 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c406a4a03e2af0d6722d2a61e6c55b05efb56fcd43ee81aa1c51019c328b019`  
		Last Modified: Fri, 11 Mar 2022 00:42:49 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.8.2-rc-focal`

```console
$ docker pull mariadb@sha256:ca5c3b079c5692dac7e28b378a95acef02df934004bf6379aff9cebdf6ca8359
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10.8.2-rc-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:b82fe107c8317aa03b87e30caf45453266dbdbbf54a488706e7661a98c40a054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128579598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19060cfc0fda93917faf594988bc544889cd727b8284e3174ec17d52115666ed`
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
# Fri, 11 Mar 2022 01:19:42 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:43 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:43 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:43 GMT
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
	-	`sha256:c12d41077524a3c495250dd259a0e95e2ff901432cb1a880f7ac83cb84ccf687`  
		Last Modified: Fri, 11 Mar 2022 01:20:36 GMT  
		Size: 3.5 KB (3482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f598f32e5ec75c4ebefbf9c5f5c7ca8899ddd449679ceebc82e62323afa5847`  
		Last Modified: Fri, 11 Mar 2022 01:20:36 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:16f2ed81ce8652e33785b7047e21d2175b8362d13b52b842a8db950f94faf72f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125653262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47ee2e1d34e81670dff8fc73abe02f9d061ddebd2f674daab048513a6e45ad94`
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
# Fri, 11 Mar 2022 01:40:02 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:03 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:04 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:05 GMT
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
	-	`sha256:f3fdf302acfcb08391bbf4148316e40381cc5887c38f20f2cf9e8a4ddf57b38d`  
		Last Modified: Fri, 11 Mar 2022 01:44:30 GMT  
		Size: 3.5 KB (3486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4623a9a008ea67a14f101ace4fccc054dba48ac54dd6647a8d45cf741cef5d6c`  
		Last Modified: Fri, 11 Mar 2022 01:44:30 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:82b14dad2c02fb6b4e989a0d1b45e6b2cecb6672b01c055407cc1c52138695ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139622015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65074644ddf3d765ba23a1d52c7b39c70db5503ab3008e4bceb9f59ca6bec207`
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
# Fri, 11 Mar 2022 01:16:59 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:17:01 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:17:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:17:14 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:17:22 GMT
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
	-	`sha256:0803f70e4a7b9d678a26db21defccbaf848e9821ba9273b771b09cf2cb9ba6b7`  
		Last Modified: Fri, 11 Mar 2022 01:22:51 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508417a0638a97a111ce300a430612018a9d14acf46cebdd668bf3973b8005f3`  
		Last Modified: Fri, 11 Mar 2022 01:22:51 GMT  
		Size: 6.6 KB (6609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.8.2-rc-focal` - linux; s390x

```console
$ docker pull mariadb@sha256:5198280ae34c2cd20bc45ee73e0b634418ba548692cac4fcdb5f9baa30d6c40e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127688007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f371c38a5139c23dc3062cd9c0bae757101b4d648e893d3a964da4e964b662e`
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
# Fri, 11 Mar 2022 00:41:33 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:33 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:33 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:33 GMT
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
	-	`sha256:b5cb7c2c2a7d570a43e161df06a8115d2023faa173c62ed233d42fe6ac82b39d`  
		Last Modified: Fri, 11 Mar 2022 00:42:49 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c406a4a03e2af0d6722d2a61e6c55b05efb56fcd43ee81aa1c51019c328b019`  
		Last Modified: Fri, 11 Mar 2022 00:42:49 GMT  
		Size: 6.6 KB (6604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:736606c3decd9b95dd8c1ee68c3e2b7e53af9e41135f6c833cd69a5eb268355e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c1988f7cf41786b77bccd23891d1afa2f83c999f4b303bfcd5f333e934b51cc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128669741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5dd1ac0b00e78cf6f5d6152b3d37a6fbb2c9b209ea58f4d205499ed4801f305`
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
# Fri, 11 Mar 2022 01:19:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:46 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:46 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:46 GMT
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
	-	`sha256:621fa3528f37c800eddf5424ae7b35ab6f823af267c6baeb9bb20867600552de`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 3.5 KB (3483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65fa0799f33d7ab55dfbaa9cf8fb881edd3f75a9d4b6f1ad76627416769b1`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:954bc8268e746a9a4b135304d85a60a99e235a79830149f76ef0439f4157a675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125722158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38051c4e5d39b816a571729967488805c4415d7b5460e36f77392cc98a45536c`
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
# Fri, 11 Mar 2022 01:40:12 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:13 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:14 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:15 GMT
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
	-	`sha256:f1d3feb849615542564db737270cb86f87c79472cd92732650492de686bc49e2`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 3.5 KB (3485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666c07e1f7c22ebd3ff693f3a2ec21991f99d923c68a16e7a76bd88947b237b`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d35dfc2be87294ad02c377b285cde99170be7ac251c0021609d702c2a68d5daf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139539786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5bbff5e51ec39ca2817bce7fd70b2384df0a6434a3734d736a877584113f4bc`
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
# Fri, 11 Mar 2022 01:17:39 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:17:42 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:17:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:18:02 GMT
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
	-	`sha256:1f5a705aa51ed4df01e6504a076cb8470714f75d46f7c06c16a34c8e4c3b10b6`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410180f3ffbc90843c959dbca9182e9b4b16783c3e9abf15e90ef46548c09416`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; s390x

```console
$ docker pull mariadb@sha256:f57e663953b1774cf5116c02dd9a4f3b3a9e7f9199296c42fd02e7c94b1efd7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127723395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226ef0fff8e8f22de2ccb61a5a90d170ae551d3d68753c08572781c3d9afdd9b`
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
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:41 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:41 GMT
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
	-	`sha256:56572738f165202d0ca50d879a5b75c73959f04bb1e66d39722a40849517261f`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1c1e0cca65f889f547f42513cc37e2ca3c6a988fef8132fa46bc00c73e0b8a`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:736606c3decd9b95dd8c1ee68c3e2b7e53af9e41135f6c833cd69a5eb268355e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:c1988f7cf41786b77bccd23891d1afa2f83c999f4b303bfcd5f333e934b51cc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128669741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5dd1ac0b00e78cf6f5d6152b3d37a6fbb2c9b209ea58f4d205499ed4801f305`
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
# Fri, 11 Mar 2022 01:19:45 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:19:46 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:19:46 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:19:46 GMT
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
	-	`sha256:621fa3528f37c800eddf5424ae7b35ab6f823af267c6baeb9bb20867600552de`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 3.5 KB (3483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65fa0799f33d7ab55dfbaa9cf8fb881edd3f75a9d4b6f1ad76627416769b1`  
		Last Modified: Fri, 11 Mar 2022 01:20:52 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:954bc8268e746a9a4b135304d85a60a99e235a79830149f76ef0439f4157a675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125722158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38051c4e5d39b816a571729967488805c4415d7b5460e36f77392cc98a45536c`
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
# Fri, 11 Mar 2022 01:40:12 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:40:13 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:40:14 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:40:15 GMT
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
	-	`sha256:f1d3feb849615542564db737270cb86f87c79472cd92732650492de686bc49e2`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 3.5 KB (3485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666c07e1f7c22ebd3ff693f3a2ec21991f99d923c68a16e7a76bd88947b237b`  
		Last Modified: Fri, 11 Mar 2022 01:44:48 GMT  
		Size: 6.6 KB (6610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d35dfc2be87294ad02c377b285cde99170be7ac251c0021609d702c2a68d5daf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139539786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5bbff5e51ec39ca2817bce7fd70b2384df0a6434a3734d736a877584113f4bc`
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
# Fri, 11 Mar 2022 01:17:39 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 01:17:42 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 01:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 01:17:58 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 01:18:02 GMT
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
	-	`sha256:1f5a705aa51ed4df01e6504a076cb8470714f75d46f7c06c16a34c8e4c3b10b6`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 3.5 KB (3488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410180f3ffbc90843c959dbca9182e9b4b16783c3e9abf15e90ef46548c09416`  
		Last Modified: Fri, 11 Mar 2022 01:23:13 GMT  
		Size: 6.6 KB (6611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:f57e663953b1774cf5116c02dd9a4f3b3a9e7f9199296c42fd02e7c94b1efd7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127723395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226ef0fff8e8f22de2ccb61a5a90d170ae551d3d68753c08572781c3d9afdd9b`
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
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 11 Mar 2022 00:41:41 GMT
COPY file:f2963d0597f75d9f9864729b9913cc598ff5f7cab4b2bb4fadf52d21300b4f1d in /usr/local/bin/ 
# Fri, 11 Mar 2022 00:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Mar 2022 00:41:41 GMT
EXPOSE 3306
# Fri, 11 Mar 2022 00:41:41 GMT
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
	-	`sha256:56572738f165202d0ca50d879a5b75c73959f04bb1e66d39722a40849517261f`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 3.5 KB (3487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1c1e0cca65f889f547f42513cc37e2ca3c6a988fef8132fa46bc00c73e0b8a`  
		Last Modified: Fri, 11 Mar 2022 00:43:01 GMT  
		Size: 6.6 KB (6608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
