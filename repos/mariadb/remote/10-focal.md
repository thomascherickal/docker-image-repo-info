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
