<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10-focal`](#mariadb10-focal)
-	[`mariadb:10.2`](#mariadb102)
-	[`mariadb:10.2-bionic`](#mariadb102-bionic)
-	[`mariadb:10.2.39`](#mariadb10239)
-	[`mariadb:10.2.39-bionic`](#mariadb10239-bionic)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.3.30`](#mariadb10330)
-	[`mariadb:10.3.30-focal`](#mariadb10330-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.4.20`](#mariadb10420)
-	[`mariadb:10.4.20-focal`](#mariadb10420-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10.5.11`](#mariadb10511)
-	[`mariadb:10.5.11-focal`](#mariadb10511-focal)
-	[`mariadb:10.6`](#mariadb106)
-	[`mariadb:10.6-focal`](#mariadb106-focal)
-	[`mariadb:10.6.2`](#mariadb1062)
-	[`mariadb:10.6.2-focal`](#mariadb1062-focal)
-	[`mariadb:focal`](#mariadbfocal)
-	[`mariadb:latest`](#mariadblatest)
-	[`mariadb:rc`](#mariadbrc)
-	[`mariadb:rc-focal`](#mariadbrc-focal)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:e42a43b7912f941d61641f5e326e66e6a73e5d3ecbb36e225f44e0fae86abaeb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:0dacf119003824f9fb12d82c019195050f1d68c2266e8a884513c2cc82615051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126881550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:104f4e7cbe8335d5a59bf4e85abe94402c46898ac01ba76f54e12350b077409b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:20:55 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 18 Jun 2021 20:20:55 GMT
ENV MARIADB_VERSION=1:10.5.10+maria~focal
# Fri, 18 Jun 2021 20:20:56 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:21:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:21:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:21:16 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:21:17 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:21:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc09fec0bce19701fafca0528b5b09a1559a67156fbdc04a5424395c24b676d3`  
		Last Modified: Fri, 18 Jun 2021 20:24:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9b9043bdda0e2583685296da540210290363752743edfd54bd88fae50d104c`  
		Last Modified: Fri, 18 Jun 2021 20:24:48 GMT  
		Size: 86.9 MB (86938711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e596ee38c508da37313418760e43b1e20273d93de33bf8d544da5845d9be5a`  
		Last Modified: Fri, 18 Jun 2021 20:24:34 GMT  
		Size: 5.6 KB (5561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:54b51624f0f714e43cc58f982b525f3a8088b0f4da13b800b3c47a078806da2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124329014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e57d78eb4a332152d529b6ba2af0d085fe4ffbe9a38fd957c1f612c52fba82d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Thu, 24 Jun 2021 01:33:35 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:34:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:34:14 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:34:15 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:34:15 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:34:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16178d1583fbf0339abc345a26f507e8a48e182309e515331c40256d4a05857`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537120db29a4871816e11bfa94ce0bfbcbc843cafcafbaa75a251e73a2eb62d8`  
		Last Modified: Thu, 24 Jun 2021 01:38:38 GMT  
		Size: 86.1 MB (86092192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cd5495defa6104e2de9f25e839f70d94c3f7d9d1483c96e4715a0b5e174051`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 5.6 KB (5557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7486c3648f7981d487c319e9f2b49e67c2afc3ac328cf02f883afa530140b7ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137575866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82eca8349acd403244c99ccbe1a3e521d344e936ce5f652565474fe2e7eff326`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:24:08 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 18 Jun 2021 20:24:17 GMT
ENV MARIADB_VERSION=1:10.5.10+maria~focal
# Fri, 18 Jun 2021 20:24:24 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:27:21 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:27:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:27:37 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:27:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:27:56 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:28:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8532e19b2d04c2f706f2ac99f0bb3668325be370240666551599d45bb235be`  
		Last Modified: Fri, 18 Jun 2021 20:43:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0073b8bf118bde577f45635ca2f109e22354e72c15b6bf19551790da0db0ddb2`  
		Last Modified: Fri, 18 Jun 2021 20:44:08 GMT  
		Size: 91.3 MB (91323812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a383425a57e912232095db76f4b2a86b914621e7b899c6549dc1e9415d686e`  
		Last Modified: Fri, 18 Jun 2021 20:43:44 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:e42a43b7912f941d61641f5e326e66e6a73e5d3ecbb36e225f44e0fae86abaeb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:0dacf119003824f9fb12d82c019195050f1d68c2266e8a884513c2cc82615051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126881550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:104f4e7cbe8335d5a59bf4e85abe94402c46898ac01ba76f54e12350b077409b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:20:55 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 18 Jun 2021 20:20:55 GMT
ENV MARIADB_VERSION=1:10.5.10+maria~focal
# Fri, 18 Jun 2021 20:20:56 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:21:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:21:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:21:16 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:21:17 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:21:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc09fec0bce19701fafca0528b5b09a1559a67156fbdc04a5424395c24b676d3`  
		Last Modified: Fri, 18 Jun 2021 20:24:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9b9043bdda0e2583685296da540210290363752743edfd54bd88fae50d104c`  
		Last Modified: Fri, 18 Jun 2021 20:24:48 GMT  
		Size: 86.9 MB (86938711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e596ee38c508da37313418760e43b1e20273d93de33bf8d544da5845d9be5a`  
		Last Modified: Fri, 18 Jun 2021 20:24:34 GMT  
		Size: 5.6 KB (5561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:54b51624f0f714e43cc58f982b525f3a8088b0f4da13b800b3c47a078806da2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124329014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e57d78eb4a332152d529b6ba2af0d085fe4ffbe9a38fd957c1f612c52fba82d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Thu, 24 Jun 2021 01:33:35 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:34:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:34:14 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:34:15 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:34:15 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:34:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16178d1583fbf0339abc345a26f507e8a48e182309e515331c40256d4a05857`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537120db29a4871816e11bfa94ce0bfbcbc843cafcafbaa75a251e73a2eb62d8`  
		Last Modified: Thu, 24 Jun 2021 01:38:38 GMT  
		Size: 86.1 MB (86092192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cd5495defa6104e2de9f25e839f70d94c3f7d9d1483c96e4715a0b5e174051`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 5.6 KB (5557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7486c3648f7981d487c319e9f2b49e67c2afc3ac328cf02f883afa530140b7ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137575866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82eca8349acd403244c99ccbe1a3e521d344e936ce5f652565474fe2e7eff326`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:24:08 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 18 Jun 2021 20:24:17 GMT
ENV MARIADB_VERSION=1:10.5.10+maria~focal
# Fri, 18 Jun 2021 20:24:24 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:27:21 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:27:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:27:37 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:27:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:27:56 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:28:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8532e19b2d04c2f706f2ac99f0bb3668325be370240666551599d45bb235be`  
		Last Modified: Fri, 18 Jun 2021 20:43:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0073b8bf118bde577f45635ca2f109e22354e72c15b6bf19551790da0db0ddb2`  
		Last Modified: Fri, 18 Jun 2021 20:44:08 GMT  
		Size: 91.3 MB (91323812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a383425a57e912232095db76f4b2a86b914621e7b899c6549dc1e9415d686e`  
		Last Modified: Fri, 18 Jun 2021 20:43:44 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:702ac647422c6bd46c30562d93457260f31b58a7b8524d2be695c227b7e9bedb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:517105250b4981243a9556e3e7f4576ed47446eb3d4bcd88371dc65e412917ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109325069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce70749d4561f75f75fe135e165faa56c41be3fa1f0c12e2e97c86feb6920b24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:59:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:59:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:59:44 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:59:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:59:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:22:49 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:22:49 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:22:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:22:51 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 18 Jun 2021 20:22:51 GMT
ENV MARIADB_VERSION=1:10.2.38+maria~bionic
# Fri, 18 Jun 2021 20:22:52 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:23:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:23:25 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:23:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:23:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 18 Jun 2021 20:23:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:23:27 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:23:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d7f527a85d567884b86652e590f5d484b9ab84b150e4925b7d87699f93fea1`  
		Last Modified: Fri, 18 Jun 2021 05:03:42 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ffc1a82bccd839baf9aee65bea12f39144d2f71d17f7a478729e5033a3483e`  
		Last Modified: Fri, 18 Jun 2021 05:03:41 GMT  
		Size: 4.8 MB (4813831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499ae120a92cf69045b499c6e9acb4746dd8021ca8ad5f655d75ba962e197ae7`  
		Last Modified: Fri, 18 Jun 2021 05:03:41 GMT  
		Size: 3.6 MB (3586283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1026105733a2b0dd715260634aaa9732338ff49ff7893ebb9f536c4a0426cf9`  
		Last Modified: Fri, 18 Jun 2021 05:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93078b4478c302f44f6e3f3db323104db146f67306b0fea97064b88b91e1375`  
		Last Modified: Fri, 18 Jun 2021 20:26:20 GMT  
		Size: 1.6 MB (1586353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafd08f8c0253feeb1e6a13569bea574b2fc83c9c089412e0fa15a0e60fa6128`  
		Last Modified: Fri, 18 Jun 2021 20:26:17 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25dd530577f8df00a2dea84507666c0865b849e2dd311756879b78df4e0c3509`  
		Last Modified: Fri, 18 Jun 2021 20:26:17 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea3241729e674368252b8f25cba1481423a2f8bab4e3f11fb978915671e3fb4`  
		Last Modified: Fri, 18 Jun 2021 20:26:28 GMT  
		Size: 72.6 MB (72624693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f489e9c74b8eafe948baf6297b64bfed3b692912670068d08fc0b09bbfc1454e`  
		Last Modified: Fri, 18 Jun 2021 20:26:17 GMT  
		Size: 5.6 KB (5559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3a9c186264af9aaf4c0dd4414790cc7414c2886d7f2c66a417804cd96aea90`  
		Last Modified: Fri, 18 Jun 2021 20:26:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:9152c567b87c51d8989f3e81a0e03344db14667ab0d0741dccb144059db54574
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104353503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55439c2d032a568cc9ec3ad7d70852b25789ae5b781bc18dfea818c3798ab253`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:48:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:49:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:49:06 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:49:20 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:49:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:42:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:42:44 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:36:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:36:07 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 24 Jun 2021 01:36:07 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Thu, 24 Jun 2021 01:36:08 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:36:31 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:36:31 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:36:32 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:36:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 24 Jun 2021 01:36:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:36:33 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:36:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203d37d33072a857afa7a7c06848aba6896f13885f8f60b3288503be9131f7d1`  
		Last Modified: Fri, 18 Jun 2021 00:54:00 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5240ac600f4c5cb6f6e1e67752ff54f6ea68150858733712e557f7769cf0ec94`  
		Last Modified: Fri, 18 Jun 2021 00:53:58 GMT  
		Size: 4.4 MB (4395498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400e9bdca319f24e8555f3cc5cb0acb5431f17160b3f7d1ace9bc0d7d2dd080c`  
		Last Modified: Fri, 18 Jun 2021 00:53:58 GMT  
		Size: 3.2 MB (3247122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ae8ab6f6a79453a733f4e0dd53ce34be50da7dff4919815b2649f1b095974e`  
		Last Modified: Fri, 18 Jun 2021 00:53:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caa1cc8ad57c9128e008118895f64a57e1f3c88aa5362b1aeed8088587f1b82`  
		Last Modified: Fri, 18 Jun 2021 20:47:18 GMT  
		Size: 1.5 MB (1532395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c7aabdcb80d3cc781b905baf83e440ee9be62371e3652becb69d743e16342e`  
		Last Modified: Thu, 24 Jun 2021 01:40:27 GMT  
		Size: 5.2 KB (5170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553615cc0e3d62da6cd1c9006d34760c776acb5da45ca0d7d6d9e8244c61787a`  
		Last Modified: Thu, 24 Jun 2021 01:40:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83b0185d04034b7cde291373eb25862e35c6398df0b4d586355951508a3a257`  
		Last Modified: Thu, 24 Jun 2021 01:40:39 GMT  
		Size: 71.4 MB (71437103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ff7474a593bb3b98b6f3df0bacd33d59082d8126742016d8e4e9dfec6ae247`  
		Last Modified: Thu, 24 Jun 2021 01:40:27 GMT  
		Size: 5.6 KB (5562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141bad04f905809f6a93fa22615f920c02f13b5dadcd9a1e30b8a3169cdd9837`  
		Last Modified: Thu, 24 Jun 2021 01:40:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a22b9704a9339ffc5a0a3cd4c1a8e144568cb33611d8e212e8254b04eb3f7aff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117672795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c8a733228352adbf7125efbc6fa2e2866b95bf83d5e035a8423b944d0388246`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:54:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:56:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:56:15 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:56:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:38:08 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:38:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:38:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:38:51 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 18 Jun 2021 20:38:55 GMT
ENV MARIADB_VERSION=1:10.2.38+maria~bionic
# Fri, 18 Jun 2021 20:39:04 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:41:30 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:41:43 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:41:46 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:41:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 18 Jun 2021 20:42:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:42:11 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:42:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b3af44a6beabcd2b603da746b157e55dee62f2a14b730d5e5148d32525712b`  
		Last Modified: Fri, 18 Jun 2021 03:05:56 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be2226c864d17eb448038b50b60568b10f6aaece2f78d586761d64da019d7f`  
		Last Modified: Fri, 18 Jun 2021 03:05:54 GMT  
		Size: 5.6 MB (5630493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fa716ade46f6351173d6e4409bcfd8d66b20a1afe34a6fad238320e5216104`  
		Last Modified: Fri, 18 Jun 2021 03:05:53 GMT  
		Size: 3.6 MB (3584735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c3777fff0af4d7e256e3c0ef6f069b23fbe190464ab5be5f5a00cc41d15797`  
		Last Modified: Fri, 18 Jun 2021 03:05:52 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ce52b06df2818b3ac1faf875d32c5e24441b13c054a6e85fe8c65ad2d29e15`  
		Last Modified: Fri, 18 Jun 2021 20:45:49 GMT  
		Size: 1.9 MB (1938757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889f569faca7aa3791667d15b22023d6aaa847c082438430d6691e426c0e5a30`  
		Last Modified: Fri, 18 Jun 2021 20:45:45 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d215c344e8a65574ad91298ddec5b369af9f6ce6b2ba359ec410dd2744a4be0a`  
		Last Modified: Fri, 18 Jun 2021 20:45:45 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf6387fe104e2a2b6cbe523bec98130f3e680a54592a54698b7c2ed6186ceac`  
		Last Modified: Fri, 18 Jun 2021 20:46:01 GMT  
		Size: 76.1 MB (76080244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341219650b21e6b1d039dc1aee1a9e6bc866e32ab426ee4445c0379c51659a37`  
		Last Modified: Fri, 18 Jun 2021 20:45:46 GMT  
		Size: 5.6 KB (5562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a890cb2c0f515443e638a86fc9b72409f7805c8595d2acd161ab4ace7df19f9e`  
		Last Modified: Fri, 18 Jun 2021 20:45:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:702ac647422c6bd46c30562d93457260f31b58a7b8524d2be695c227b7e9bedb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:517105250b4981243a9556e3e7f4576ed47446eb3d4bcd88371dc65e412917ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109325069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce70749d4561f75f75fe135e165faa56c41be3fa1f0c12e2e97c86feb6920b24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:59:29 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:59:44 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:59:44 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:59:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:59:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:22:49 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:22:49 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:22:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:22:51 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 18 Jun 2021 20:22:51 GMT
ENV MARIADB_VERSION=1:10.2.38+maria~bionic
# Fri, 18 Jun 2021 20:22:52 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:23:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:23:25 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:23:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:23:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 18 Jun 2021 20:23:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:23:27 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:23:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d7f527a85d567884b86652e590f5d484b9ab84b150e4925b7d87699f93fea1`  
		Last Modified: Fri, 18 Jun 2021 05:03:42 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ffc1a82bccd839baf9aee65bea12f39144d2f71d17f7a478729e5033a3483e`  
		Last Modified: Fri, 18 Jun 2021 05:03:41 GMT  
		Size: 4.8 MB (4813831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499ae120a92cf69045b499c6e9acb4746dd8021ca8ad5f655d75ba962e197ae7`  
		Last Modified: Fri, 18 Jun 2021 05:03:41 GMT  
		Size: 3.6 MB (3586283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1026105733a2b0dd715260634aaa9732338ff49ff7893ebb9f536c4a0426cf9`  
		Last Modified: Fri, 18 Jun 2021 05:03:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93078b4478c302f44f6e3f3db323104db146f67306b0fea97064b88b91e1375`  
		Last Modified: Fri, 18 Jun 2021 20:26:20 GMT  
		Size: 1.6 MB (1586353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafd08f8c0253feeb1e6a13569bea574b2fc83c9c089412e0fa15a0e60fa6128`  
		Last Modified: Fri, 18 Jun 2021 20:26:17 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25dd530577f8df00a2dea84507666c0865b849e2dd311756879b78df4e0c3509`  
		Last Modified: Fri, 18 Jun 2021 20:26:17 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea3241729e674368252b8f25cba1481423a2f8bab4e3f11fb978915671e3fb4`  
		Last Modified: Fri, 18 Jun 2021 20:26:28 GMT  
		Size: 72.6 MB (72624693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f489e9c74b8eafe948baf6297b64bfed3b692912670068d08fc0b09bbfc1454e`  
		Last Modified: Fri, 18 Jun 2021 20:26:17 GMT  
		Size: 5.6 KB (5559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3a9c186264af9aaf4c0dd4414790cc7414c2886d7f2c66a417804cd96aea90`  
		Last Modified: Fri, 18 Jun 2021 20:26:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:9152c567b87c51d8989f3e81a0e03344db14667ab0d0741dccb144059db54574
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104353503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55439c2d032a568cc9ec3ad7d70852b25789ae5b781bc18dfea818c3798ab253`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:48:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:49:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:49:06 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:49:20 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:49:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:42:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:42:44 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:36:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:36:07 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 24 Jun 2021 01:36:07 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Thu, 24 Jun 2021 01:36:08 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:36:31 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:36:31 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:36:32 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:36:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 24 Jun 2021 01:36:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:36:33 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:36:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203d37d33072a857afa7a7c06848aba6896f13885f8f60b3288503be9131f7d1`  
		Last Modified: Fri, 18 Jun 2021 00:54:00 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5240ac600f4c5cb6f6e1e67752ff54f6ea68150858733712e557f7769cf0ec94`  
		Last Modified: Fri, 18 Jun 2021 00:53:58 GMT  
		Size: 4.4 MB (4395498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400e9bdca319f24e8555f3cc5cb0acb5431f17160b3f7d1ace9bc0d7d2dd080c`  
		Last Modified: Fri, 18 Jun 2021 00:53:58 GMT  
		Size: 3.2 MB (3247122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ae8ab6f6a79453a733f4e0dd53ce34be50da7dff4919815b2649f1b095974e`  
		Last Modified: Fri, 18 Jun 2021 00:53:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caa1cc8ad57c9128e008118895f64a57e1f3c88aa5362b1aeed8088587f1b82`  
		Last Modified: Fri, 18 Jun 2021 20:47:18 GMT  
		Size: 1.5 MB (1532395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c7aabdcb80d3cc781b905baf83e440ee9be62371e3652becb69d743e16342e`  
		Last Modified: Thu, 24 Jun 2021 01:40:27 GMT  
		Size: 5.2 KB (5170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553615cc0e3d62da6cd1c9006d34760c776acb5da45ca0d7d6d9e8244c61787a`  
		Last Modified: Thu, 24 Jun 2021 01:40:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83b0185d04034b7cde291373eb25862e35c6398df0b4d586355951508a3a257`  
		Last Modified: Thu, 24 Jun 2021 01:40:39 GMT  
		Size: 71.4 MB (71437103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ff7474a593bb3b98b6f3df0bacd33d59082d8126742016d8e4e9dfec6ae247`  
		Last Modified: Thu, 24 Jun 2021 01:40:27 GMT  
		Size: 5.6 KB (5562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141bad04f905809f6a93fa22615f920c02f13b5dadcd9a1e30b8a3169cdd9837`  
		Last Modified: Thu, 24 Jun 2021 01:40:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a22b9704a9339ffc5a0a3cd4c1a8e144568cb33611d8e212e8254b04eb3f7aff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117672795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c8a733228352adbf7125efbc6fa2e2866b95bf83d5e035a8423b944d0388246`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:24:58 GMT
ADD file:33bc9edd94d5731da919e83ed38bd4aa7daffcb5f629d93bbde112a795c79d48 in / 
# Thu, 17 Jun 2021 23:25:03 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:54:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:56:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:56:15 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:56:57 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:38:08 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:38:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:38:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:38:51 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 18 Jun 2021 20:38:55 GMT
ENV MARIADB_VERSION=1:10.2.38+maria~bionic
# Fri, 18 Jun 2021 20:39:04 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:41:30 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:41:43 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:41:46 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:41:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 18 Jun 2021 20:42:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:42:11 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:42:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4e37c2419ee7d7e826be5c6ee69243351aaf456d6527714660cf7e7015491051`  
		Last Modified: Thu, 17 Jun 2021 23:28:22 GMT  
		Size: 30.4 MB (30425356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b3af44a6beabcd2b603da746b157e55dee62f2a14b730d5e5148d32525712b`  
		Last Modified: Fri, 18 Jun 2021 03:05:56 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be2226c864d17eb448038b50b60568b10f6aaece2f78d586761d64da019d7f`  
		Last Modified: Fri, 18 Jun 2021 03:05:54 GMT  
		Size: 5.6 MB (5630493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fa716ade46f6351173d6e4409bcfd8d66b20a1afe34a6fad238320e5216104`  
		Last Modified: Fri, 18 Jun 2021 03:05:53 GMT  
		Size: 3.6 MB (3584735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c3777fff0af4d7e256e3c0ef6f069b23fbe190464ab5be5f5a00cc41d15797`  
		Last Modified: Fri, 18 Jun 2021 03:05:52 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ce52b06df2818b3ac1faf875d32c5e24441b13c054a6e85fe8c65ad2d29e15`  
		Last Modified: Fri, 18 Jun 2021 20:45:49 GMT  
		Size: 1.9 MB (1938757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889f569faca7aa3791667d15b22023d6aaa847c082438430d6691e426c0e5a30`  
		Last Modified: Fri, 18 Jun 2021 20:45:45 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d215c344e8a65574ad91298ddec5b369af9f6ce6b2ba359ec410dd2744a4be0a`  
		Last Modified: Fri, 18 Jun 2021 20:45:45 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf6387fe104e2a2b6cbe523bec98130f3e680a54592a54698b7c2ed6186ceac`  
		Last Modified: Fri, 18 Jun 2021 20:46:01 GMT  
		Size: 76.1 MB (76080244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341219650b21e6b1d039dc1aee1a9e6bc866e32ab426ee4445c0379c51659a37`  
		Last Modified: Fri, 18 Jun 2021 20:45:46 GMT  
		Size: 5.6 KB (5562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a890cb2c0f515443e638a86fc9b72409f7805c8595d2acd161ab4ace7df19f9e`  
		Last Modified: Fri, 18 Jun 2021 20:45:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.39`

```console
$ docker pull mariadb@sha256:92987138ab9eb12a171ae14bc623cd4f2684bfaeda0ffd902792ae15d4566368
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `mariadb:10.2.39` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:9152c567b87c51d8989f3e81a0e03344db14667ab0d0741dccb144059db54574
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104353503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55439c2d032a568cc9ec3ad7d70852b25789ae5b781bc18dfea818c3798ab253`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:48:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:49:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:49:06 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:49:20 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:49:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:42:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:42:44 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:36:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:36:07 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 24 Jun 2021 01:36:07 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Thu, 24 Jun 2021 01:36:08 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:36:31 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:36:31 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:36:32 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:36:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 24 Jun 2021 01:36:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:36:33 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:36:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203d37d33072a857afa7a7c06848aba6896f13885f8f60b3288503be9131f7d1`  
		Last Modified: Fri, 18 Jun 2021 00:54:00 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5240ac600f4c5cb6f6e1e67752ff54f6ea68150858733712e557f7769cf0ec94`  
		Last Modified: Fri, 18 Jun 2021 00:53:58 GMT  
		Size: 4.4 MB (4395498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400e9bdca319f24e8555f3cc5cb0acb5431f17160b3f7d1ace9bc0d7d2dd080c`  
		Last Modified: Fri, 18 Jun 2021 00:53:58 GMT  
		Size: 3.2 MB (3247122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ae8ab6f6a79453a733f4e0dd53ce34be50da7dff4919815b2649f1b095974e`  
		Last Modified: Fri, 18 Jun 2021 00:53:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caa1cc8ad57c9128e008118895f64a57e1f3c88aa5362b1aeed8088587f1b82`  
		Last Modified: Fri, 18 Jun 2021 20:47:18 GMT  
		Size: 1.5 MB (1532395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c7aabdcb80d3cc781b905baf83e440ee9be62371e3652becb69d743e16342e`  
		Last Modified: Thu, 24 Jun 2021 01:40:27 GMT  
		Size: 5.2 KB (5170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553615cc0e3d62da6cd1c9006d34760c776acb5da45ca0d7d6d9e8244c61787a`  
		Last Modified: Thu, 24 Jun 2021 01:40:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83b0185d04034b7cde291373eb25862e35c6398df0b4d586355951508a3a257`  
		Last Modified: Thu, 24 Jun 2021 01:40:39 GMT  
		Size: 71.4 MB (71437103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ff7474a593bb3b98b6f3df0bacd33d59082d8126742016d8e4e9dfec6ae247`  
		Last Modified: Thu, 24 Jun 2021 01:40:27 GMT  
		Size: 5.6 KB (5562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141bad04f905809f6a93fa22615f920c02f13b5dadcd9a1e30b8a3169cdd9837`  
		Last Modified: Thu, 24 Jun 2021 01:40:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.39-bionic`

```console
$ docker pull mariadb@sha256:92987138ab9eb12a171ae14bc623cd4f2684bfaeda0ffd902792ae15d4566368
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `mariadb:10.2.39-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:9152c567b87c51d8989f3e81a0e03344db14667ab0d0741dccb144059db54574
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104353503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55439c2d032a568cc9ec3ad7d70852b25789ae5b781bc18dfea818c3798ab253`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:48:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:49:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:49:06 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:49:20 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:49:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:42:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc1 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:42:44 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:36:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:36:07 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 24 Jun 2021 01:36:07 GMT
ENV MARIADB_VERSION=1:10.2.39+maria~bionic
# Thu, 24 Jun 2021 01:36:08 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:36:31 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:36:31 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:36:32 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:36:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 24 Jun 2021 01:36:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:36:33 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:36:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203d37d33072a857afa7a7c06848aba6896f13885f8f60b3288503be9131f7d1`  
		Last Modified: Fri, 18 Jun 2021 00:54:00 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5240ac600f4c5cb6f6e1e67752ff54f6ea68150858733712e557f7769cf0ec94`  
		Last Modified: Fri, 18 Jun 2021 00:53:58 GMT  
		Size: 4.4 MB (4395498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400e9bdca319f24e8555f3cc5cb0acb5431f17160b3f7d1ace9bc0d7d2dd080c`  
		Last Modified: Fri, 18 Jun 2021 00:53:58 GMT  
		Size: 3.2 MB (3247122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ae8ab6f6a79453a733f4e0dd53ce34be50da7dff4919815b2649f1b095974e`  
		Last Modified: Fri, 18 Jun 2021 00:53:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caa1cc8ad57c9128e008118895f64a57e1f3c88aa5362b1aeed8088587f1b82`  
		Last Modified: Fri, 18 Jun 2021 20:47:18 GMT  
		Size: 1.5 MB (1532395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c7aabdcb80d3cc781b905baf83e440ee9be62371e3652becb69d743e16342e`  
		Last Modified: Thu, 24 Jun 2021 01:40:27 GMT  
		Size: 5.2 KB (5170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553615cc0e3d62da6cd1c9006d34760c776acb5da45ca0d7d6d9e8244c61787a`  
		Last Modified: Thu, 24 Jun 2021 01:40:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83b0185d04034b7cde291373eb25862e35c6398df0b4d586355951508a3a257`  
		Last Modified: Thu, 24 Jun 2021 01:40:39 GMT  
		Size: 71.4 MB (71437103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ff7474a593bb3b98b6f3df0bacd33d59082d8126742016d8e4e9dfec6ae247`  
		Last Modified: Thu, 24 Jun 2021 01:40:27 GMT  
		Size: 5.6 KB (5562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141bad04f905809f6a93fa22615f920c02f13b5dadcd9a1e30b8a3169cdd9837`  
		Last Modified: Thu, 24 Jun 2021 01:40:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:4d291e1bd9f2495c0ea4e365325ecc0b19f0ae7fd512e7ea431497341035b754
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:61fd7d14169c60b4eaaf7bcdb8a37ee563c5f21fbd667bb5a52e809dd4ffbd6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120022873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772692a075b3f5154b383f7ddf69ddb77d32e4a44bf5d29a33fc0c697af11ae1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:22:04 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 18 Jun 2021 20:22:04 GMT
ENV MARIADB_VERSION=1:10.3.29+maria~focal
# Fri, 18 Jun 2021 20:22:05 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:22:30 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:22:30 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:22:31 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:22:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 18 Jun 2021 20:22:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:22:32 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:22:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48f0076dd2456df4b19ab340bfff8f8f0b12da00b32712f2cfad4a914ef033b`  
		Last Modified: Fri, 18 Jun 2021 20:25:47 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097b3ccf889223f4f2689e840940bb05334d526979c78f7f5829a4b3c1da4d60`  
		Last Modified: Fri, 18 Jun 2021 20:26:00 GMT  
		Size: 80.1 MB (80079913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328e05206b581856a194d0e305aff1323251eaf190b992e9ff52d8feb844283a`  
		Last Modified: Fri, 18 Jun 2021 20:25:47 GMT  
		Size: 5.6 KB (5562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bb19b0bf1e564a45c9009b4e24508be60f713dd59d0041785c844742194aaf`  
		Last Modified: Fri, 18 Jun 2021 20:25:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:4fb5b7bbf976b8e7113b267aa140f8ee88911e63cf349816df8899ca3ee894d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117633818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6892a68bf6ab4d0a3e360feb25868b62c322c7ba054d3e4b0581aaea19cbcf59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:35:20 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 24 Jun 2021 01:35:20 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Thu, 24 Jun 2021 01:35:21 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:35:57 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:35:58 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:35:58 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:35:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 24 Jun 2021 01:35:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:35:59 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:35:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b10920c7f04435e4d41ef4a671ae4db6a95202819f47efa863cff3418be8094`  
		Last Modified: Thu, 24 Jun 2021 01:39:51 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd61b379e0feafb3c2c3c865d9d434ce8b050a62bfe2616f856a7f4b8d88067`  
		Last Modified: Thu, 24 Jun 2021 01:40:06 GMT  
		Size: 79.4 MB (79396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93af836706e834d6a026e0670d0e3f644c65ca4245a97dea67fba39b339a43a`  
		Last Modified: Thu, 24 Jun 2021 01:39:51 GMT  
		Size: 5.6 KB (5558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bcd1470031941c3a8388185ee62560c1309bbc1eabd7464e2e4390b857b0d14`  
		Last Modified: Thu, 24 Jun 2021 01:39:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:466e4a3621d3a6f63f5047aaa556374173837e0db476f41c72c55ea48b7af114
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130902736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cddafb544048cb4a90fbbef0ab8d6c87d416b9f738a14a3a625d83b6d7d2ee6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:32:38 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 18 Jun 2021 20:32:47 GMT
ENV MARIADB_VERSION=1:10.3.29+maria~focal
# Fri, 18 Jun 2021 20:32:57 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:35:45 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:35:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:35:56 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:36:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 18 Jun 2021 20:36:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:36:16 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:36:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6db71d7ed35828e6264ee23b99e9980f62f3c17ba0db4296c95089784b6a9a`  
		Last Modified: Fri, 18 Jun 2021 20:45:11 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cc7125b1a436144cb5cfebcdbdc2ebb4f7f2634452da4260d6617167138c76`  
		Last Modified: Fri, 18 Jun 2021 20:45:29 GMT  
		Size: 84.7 MB (84650560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805c89284561f95226030054bebe774f4a65b2535f4eca9ce9c5f7b14d5db867`  
		Last Modified: Fri, 18 Jun 2021 20:45:11 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb8047448fa54cda041676a7545556511b0756e10b0258ba282500fdef575d8`  
		Last Modified: Fri, 18 Jun 2021 20:45:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:4d291e1bd9f2495c0ea4e365325ecc0b19f0ae7fd512e7ea431497341035b754
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:61fd7d14169c60b4eaaf7bcdb8a37ee563c5f21fbd667bb5a52e809dd4ffbd6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120022873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772692a075b3f5154b383f7ddf69ddb77d32e4a44bf5d29a33fc0c697af11ae1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:22:04 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 18 Jun 2021 20:22:04 GMT
ENV MARIADB_VERSION=1:10.3.29+maria~focal
# Fri, 18 Jun 2021 20:22:05 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:22:30 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:22:30 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:22:31 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:22:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 18 Jun 2021 20:22:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:22:32 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:22:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48f0076dd2456df4b19ab340bfff8f8f0b12da00b32712f2cfad4a914ef033b`  
		Last Modified: Fri, 18 Jun 2021 20:25:47 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097b3ccf889223f4f2689e840940bb05334d526979c78f7f5829a4b3c1da4d60`  
		Last Modified: Fri, 18 Jun 2021 20:26:00 GMT  
		Size: 80.1 MB (80079913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328e05206b581856a194d0e305aff1323251eaf190b992e9ff52d8feb844283a`  
		Last Modified: Fri, 18 Jun 2021 20:25:47 GMT  
		Size: 5.6 KB (5562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bb19b0bf1e564a45c9009b4e24508be60f713dd59d0041785c844742194aaf`  
		Last Modified: Fri, 18 Jun 2021 20:25:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:4fb5b7bbf976b8e7113b267aa140f8ee88911e63cf349816df8899ca3ee894d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117633818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6892a68bf6ab4d0a3e360feb25868b62c322c7ba054d3e4b0581aaea19cbcf59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:35:20 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 24 Jun 2021 01:35:20 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Thu, 24 Jun 2021 01:35:21 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:35:57 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:35:58 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:35:58 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:35:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 24 Jun 2021 01:35:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:35:59 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:35:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b10920c7f04435e4d41ef4a671ae4db6a95202819f47efa863cff3418be8094`  
		Last Modified: Thu, 24 Jun 2021 01:39:51 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd61b379e0feafb3c2c3c865d9d434ce8b050a62bfe2616f856a7f4b8d88067`  
		Last Modified: Thu, 24 Jun 2021 01:40:06 GMT  
		Size: 79.4 MB (79396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93af836706e834d6a026e0670d0e3f644c65ca4245a97dea67fba39b339a43a`  
		Last Modified: Thu, 24 Jun 2021 01:39:51 GMT  
		Size: 5.6 KB (5558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bcd1470031941c3a8388185ee62560c1309bbc1eabd7464e2e4390b857b0d14`  
		Last Modified: Thu, 24 Jun 2021 01:39:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:466e4a3621d3a6f63f5047aaa556374173837e0db476f41c72c55ea48b7af114
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130902736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cddafb544048cb4a90fbbef0ab8d6c87d416b9f738a14a3a625d83b6d7d2ee6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:32:38 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 18 Jun 2021 20:32:47 GMT
ENV MARIADB_VERSION=1:10.3.29+maria~focal
# Fri, 18 Jun 2021 20:32:57 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:35:45 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:35:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:35:56 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:36:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 18 Jun 2021 20:36:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:36:16 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:36:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6db71d7ed35828e6264ee23b99e9980f62f3c17ba0db4296c95089784b6a9a`  
		Last Modified: Fri, 18 Jun 2021 20:45:11 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cc7125b1a436144cb5cfebcdbdc2ebb4f7f2634452da4260d6617167138c76`  
		Last Modified: Fri, 18 Jun 2021 20:45:29 GMT  
		Size: 84.7 MB (84650560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805c89284561f95226030054bebe774f4a65b2535f4eca9ce9c5f7b14d5db867`  
		Last Modified: Fri, 18 Jun 2021 20:45:11 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb8047448fa54cda041676a7545556511b0756e10b0258ba282500fdef575d8`  
		Last Modified: Fri, 18 Jun 2021 20:45:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.30`

```console
$ docker pull mariadb@sha256:77482b7d47d396c897635636c03f723e70712e8b0a07e4a296ccb266166534a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `mariadb:10.3.30` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:4fb5b7bbf976b8e7113b267aa140f8ee88911e63cf349816df8899ca3ee894d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117633818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6892a68bf6ab4d0a3e360feb25868b62c322c7ba054d3e4b0581aaea19cbcf59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:35:20 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 24 Jun 2021 01:35:20 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Thu, 24 Jun 2021 01:35:21 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:35:57 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:35:58 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:35:58 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:35:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 24 Jun 2021 01:35:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:35:59 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:35:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b10920c7f04435e4d41ef4a671ae4db6a95202819f47efa863cff3418be8094`  
		Last Modified: Thu, 24 Jun 2021 01:39:51 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd61b379e0feafb3c2c3c865d9d434ce8b050a62bfe2616f856a7f4b8d88067`  
		Last Modified: Thu, 24 Jun 2021 01:40:06 GMT  
		Size: 79.4 MB (79396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93af836706e834d6a026e0670d0e3f644c65ca4245a97dea67fba39b339a43a`  
		Last Modified: Thu, 24 Jun 2021 01:39:51 GMT  
		Size: 5.6 KB (5558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bcd1470031941c3a8388185ee62560c1309bbc1eabd7464e2e4390b857b0d14`  
		Last Modified: Thu, 24 Jun 2021 01:39:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.30-focal`

```console
$ docker pull mariadb@sha256:77482b7d47d396c897635636c03f723e70712e8b0a07e4a296ccb266166534a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `mariadb:10.3.30-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:4fb5b7bbf976b8e7113b267aa140f8ee88911e63cf349816df8899ca3ee894d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117633818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6892a68bf6ab4d0a3e360feb25868b62c322c7ba054d3e4b0581aaea19cbcf59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:35:20 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 24 Jun 2021 01:35:20 GMT
ENV MARIADB_VERSION=1:10.3.30+maria~focal
# Thu, 24 Jun 2021 01:35:21 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:35:57 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:35:58 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:35:58 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:35:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 24 Jun 2021 01:35:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:35:59 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:35:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b10920c7f04435e4d41ef4a671ae4db6a95202819f47efa863cff3418be8094`  
		Last Modified: Thu, 24 Jun 2021 01:39:51 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd61b379e0feafb3c2c3c865d9d434ce8b050a62bfe2616f856a7f4b8d88067`  
		Last Modified: Thu, 24 Jun 2021 01:40:06 GMT  
		Size: 79.4 MB (79396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93af836706e834d6a026e0670d0e3f644c65ca4245a97dea67fba39b339a43a`  
		Last Modified: Thu, 24 Jun 2021 01:39:51 GMT  
		Size: 5.6 KB (5558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bcd1470031941c3a8388185ee62560c1309bbc1eabd7464e2e4390b857b0d14`  
		Last Modified: Thu, 24 Jun 2021 01:39:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:b3a6838af9049f0389645ec10472ec34b571282edeea68ed1d275b537cea48b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:5a54b5ce2c0480ec779c7a33a16e5d7ea293eb55e9145133fc6099e78c883c84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124705063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53c9c3918004e5f21f2b8cf32b170bd7323b4ae7a59174060111a1d369ca1ffd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:21:21 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 18 Jun 2021 20:21:21 GMT
ENV MARIADB_VERSION=1:10.4.19+maria~focal
# Fri, 18 Jun 2021 20:21:22 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:21:53 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:21:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:21:54 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:21:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 18 Jun 2021 20:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:21:56 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:21:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f258b4cef7b898ee6baa2c568159ee16baf1b1abd14dc3365ad39894972eb0`  
		Last Modified: Fri, 18 Jun 2021 20:25:16 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafdc7ecf92371f5cf119f0f08dbab150ca141a16bf60e7092b5e7be696ccad8`  
		Last Modified: Fri, 18 Jun 2021 20:25:29 GMT  
		Size: 84.8 MB (84762104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd292b20bdce73d281b4ff34af82d1f4d0778804d9a80784be4a41218a4442d`  
		Last Modified: Fri, 18 Jun 2021 20:25:16 GMT  
		Size: 5.6 KB (5561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374711163344a6b9d4f5fcd44a24880fc636b2894b672fecced00872ccc975d9`  
		Last Modified: Fri, 18 Jun 2021 20:25:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d38cffda69cbf2f0ddd0f1a54e336bfe60d37dfe84e6bfd23cd132fbfb0c8056
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122243814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04cd0faba145023bcd942627307fc69e10a2f4ad04e1687533f5e39b82e0d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:34:26 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 24 Jun 2021 01:34:26 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Thu, 24 Jun 2021 01:34:27 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:35:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:35:12 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:35:12 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:35:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 24 Jun 2021 01:35:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:35:13 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:35:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af65c4382344251378a286fafc4a08eb31435b364f79ef2e0ff2bdc929c764b`  
		Last Modified: Thu, 24 Jun 2021 01:39:11 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddde6670e77d0dbb384a3a49e945ab9b0af0c924be0d88a19ea3f33d2d34231`  
		Last Modified: Thu, 24 Jun 2021 01:39:27 GMT  
		Size: 84.0 MB (84006863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfd34f31d23bbd399297e7f2ad383e3fbe56db2536070f0adf46064127ebab1`  
		Last Modified: Thu, 24 Jun 2021 01:39:12 GMT  
		Size: 5.6 KB (5562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8943345c97bded91d9bf450345724f6df8e01afb018cb7260404147e69eb17e3`  
		Last Modified: Thu, 24 Jun 2021 01:39:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7852dbc52213375debfa9f86ada235315310415436f6908ffa707ad2b029f355
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135481200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87d98d3c7f7d1574b809bd4211c42d5b3b1e55c38bb0b7d51e53a8b7e5d385ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:28:22 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 18 Jun 2021 20:28:25 GMT
ENV MARIADB_VERSION=1:10.4.19+maria~focal
# Fri, 18 Jun 2021 20:28:43 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:31:35 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:31:40 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:31:43 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:31:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 18 Jun 2021 20:32:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:32:08 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:32:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0d4a97a38c708c1f71aaff81282b1923bbe58aefed855bf23d58cf5605b497`  
		Last Modified: Fri, 18 Jun 2021 20:44:33 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25dbf89fc0163ba94e6b525ab0d62916b8ec863ee352439cae71b1c190bba601`  
		Last Modified: Fri, 18 Jun 2021 20:44:51 GMT  
		Size: 89.2 MB (89229023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4debf788b00e4bcd953a43abf11fc302d32f7d8759766e77620300beb4c45285`  
		Last Modified: Fri, 18 Jun 2021 20:44:33 GMT  
		Size: 5.6 KB (5561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255868f7c20a304794e96186bcca70186e3da495f89d805354779648a33ed135`  
		Last Modified: Fri, 18 Jun 2021 20:44:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:b3a6838af9049f0389645ec10472ec34b571282edeea68ed1d275b537cea48b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:5a54b5ce2c0480ec779c7a33a16e5d7ea293eb55e9145133fc6099e78c883c84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124705063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53c9c3918004e5f21f2b8cf32b170bd7323b4ae7a59174060111a1d369ca1ffd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:21:21 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 18 Jun 2021 20:21:21 GMT
ENV MARIADB_VERSION=1:10.4.19+maria~focal
# Fri, 18 Jun 2021 20:21:22 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:21:53 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:21:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:21:54 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:21:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 18 Jun 2021 20:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:21:56 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:21:56 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f258b4cef7b898ee6baa2c568159ee16baf1b1abd14dc3365ad39894972eb0`  
		Last Modified: Fri, 18 Jun 2021 20:25:16 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafdc7ecf92371f5cf119f0f08dbab150ca141a16bf60e7092b5e7be696ccad8`  
		Last Modified: Fri, 18 Jun 2021 20:25:29 GMT  
		Size: 84.8 MB (84762104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd292b20bdce73d281b4ff34af82d1f4d0778804d9a80784be4a41218a4442d`  
		Last Modified: Fri, 18 Jun 2021 20:25:16 GMT  
		Size: 5.6 KB (5561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374711163344a6b9d4f5fcd44a24880fc636b2894b672fecced00872ccc975d9`  
		Last Modified: Fri, 18 Jun 2021 20:25:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d38cffda69cbf2f0ddd0f1a54e336bfe60d37dfe84e6bfd23cd132fbfb0c8056
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122243814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04cd0faba145023bcd942627307fc69e10a2f4ad04e1687533f5e39b82e0d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:34:26 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 24 Jun 2021 01:34:26 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Thu, 24 Jun 2021 01:34:27 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:35:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:35:12 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:35:12 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:35:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 24 Jun 2021 01:35:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:35:13 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:35:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af65c4382344251378a286fafc4a08eb31435b364f79ef2e0ff2bdc929c764b`  
		Last Modified: Thu, 24 Jun 2021 01:39:11 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddde6670e77d0dbb384a3a49e945ab9b0af0c924be0d88a19ea3f33d2d34231`  
		Last Modified: Thu, 24 Jun 2021 01:39:27 GMT  
		Size: 84.0 MB (84006863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfd34f31d23bbd399297e7f2ad383e3fbe56db2536070f0adf46064127ebab1`  
		Last Modified: Thu, 24 Jun 2021 01:39:12 GMT  
		Size: 5.6 KB (5562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8943345c97bded91d9bf450345724f6df8e01afb018cb7260404147e69eb17e3`  
		Last Modified: Thu, 24 Jun 2021 01:39:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7852dbc52213375debfa9f86ada235315310415436f6908ffa707ad2b029f355
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135481200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87d98d3c7f7d1574b809bd4211c42d5b3b1e55c38bb0b7d51e53a8b7e5d385ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:28:22 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 18 Jun 2021 20:28:25 GMT
ENV MARIADB_VERSION=1:10.4.19+maria~focal
# Fri, 18 Jun 2021 20:28:43 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:31:35 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:31:40 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:31:43 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:31:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 18 Jun 2021 20:32:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:32:08 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:32:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0d4a97a38c708c1f71aaff81282b1923bbe58aefed855bf23d58cf5605b497`  
		Last Modified: Fri, 18 Jun 2021 20:44:33 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25dbf89fc0163ba94e6b525ab0d62916b8ec863ee352439cae71b1c190bba601`  
		Last Modified: Fri, 18 Jun 2021 20:44:51 GMT  
		Size: 89.2 MB (89229023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4debf788b00e4bcd953a43abf11fc302d32f7d8759766e77620300beb4c45285`  
		Last Modified: Fri, 18 Jun 2021 20:44:33 GMT  
		Size: 5.6 KB (5561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255868f7c20a304794e96186bcca70186e3da495f89d805354779648a33ed135`  
		Last Modified: Fri, 18 Jun 2021 20:44:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.20`

```console
$ docker pull mariadb@sha256:b7813876396d34287602d5dff145d99140ec1b081f795f889cb9f5bfbd729dad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `mariadb:10.4.20` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d38cffda69cbf2f0ddd0f1a54e336bfe60d37dfe84e6bfd23cd132fbfb0c8056
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122243814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04cd0faba145023bcd942627307fc69e10a2f4ad04e1687533f5e39b82e0d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:34:26 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 24 Jun 2021 01:34:26 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Thu, 24 Jun 2021 01:34:27 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:35:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:35:12 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:35:12 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:35:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 24 Jun 2021 01:35:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:35:13 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:35:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af65c4382344251378a286fafc4a08eb31435b364f79ef2e0ff2bdc929c764b`  
		Last Modified: Thu, 24 Jun 2021 01:39:11 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddde6670e77d0dbb384a3a49e945ab9b0af0c924be0d88a19ea3f33d2d34231`  
		Last Modified: Thu, 24 Jun 2021 01:39:27 GMT  
		Size: 84.0 MB (84006863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfd34f31d23bbd399297e7f2ad383e3fbe56db2536070f0adf46064127ebab1`  
		Last Modified: Thu, 24 Jun 2021 01:39:12 GMT  
		Size: 5.6 KB (5562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8943345c97bded91d9bf450345724f6df8e01afb018cb7260404147e69eb17e3`  
		Last Modified: Thu, 24 Jun 2021 01:39:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.20-focal`

```console
$ docker pull mariadb@sha256:b7813876396d34287602d5dff145d99140ec1b081f795f889cb9f5bfbd729dad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `mariadb:10.4.20-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:d38cffda69cbf2f0ddd0f1a54e336bfe60d37dfe84e6bfd23cd132fbfb0c8056
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122243814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04cd0faba145023bcd942627307fc69e10a2f4ad04e1687533f5e39b82e0d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:34:26 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 24 Jun 2021 01:34:26 GMT
ENV MARIADB_VERSION=1:10.4.20+maria~focal
# Thu, 24 Jun 2021 01:34:27 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:35:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:35:12 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:35:12 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:35:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 24 Jun 2021 01:35:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:35:13 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:35:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af65c4382344251378a286fafc4a08eb31435b364f79ef2e0ff2bdc929c764b`  
		Last Modified: Thu, 24 Jun 2021 01:39:11 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddde6670e77d0dbb384a3a49e945ab9b0af0c924be0d88a19ea3f33d2d34231`  
		Last Modified: Thu, 24 Jun 2021 01:39:27 GMT  
		Size: 84.0 MB (84006863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfd34f31d23bbd399297e7f2ad383e3fbe56db2536070f0adf46064127ebab1`  
		Last Modified: Thu, 24 Jun 2021 01:39:12 GMT  
		Size: 5.6 KB (5562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8943345c97bded91d9bf450345724f6df8e01afb018cb7260404147e69eb17e3`  
		Last Modified: Thu, 24 Jun 2021 01:39:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:e42a43b7912f941d61641f5e326e66e6a73e5d3ecbb36e225f44e0fae86abaeb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:0dacf119003824f9fb12d82c019195050f1d68c2266e8a884513c2cc82615051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126881550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:104f4e7cbe8335d5a59bf4e85abe94402c46898ac01ba76f54e12350b077409b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:20:55 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 18 Jun 2021 20:20:55 GMT
ENV MARIADB_VERSION=1:10.5.10+maria~focal
# Fri, 18 Jun 2021 20:20:56 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:21:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:21:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:21:16 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:21:17 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:21:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc09fec0bce19701fafca0528b5b09a1559a67156fbdc04a5424395c24b676d3`  
		Last Modified: Fri, 18 Jun 2021 20:24:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9b9043bdda0e2583685296da540210290363752743edfd54bd88fae50d104c`  
		Last Modified: Fri, 18 Jun 2021 20:24:48 GMT  
		Size: 86.9 MB (86938711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e596ee38c508da37313418760e43b1e20273d93de33bf8d544da5845d9be5a`  
		Last Modified: Fri, 18 Jun 2021 20:24:34 GMT  
		Size: 5.6 KB (5561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:54b51624f0f714e43cc58f982b525f3a8088b0f4da13b800b3c47a078806da2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124329014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e57d78eb4a332152d529b6ba2af0d085fe4ffbe9a38fd957c1f612c52fba82d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Thu, 24 Jun 2021 01:33:35 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:34:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:34:14 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:34:15 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:34:15 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:34:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16178d1583fbf0339abc345a26f507e8a48e182309e515331c40256d4a05857`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537120db29a4871816e11bfa94ce0bfbcbc843cafcafbaa75a251e73a2eb62d8`  
		Last Modified: Thu, 24 Jun 2021 01:38:38 GMT  
		Size: 86.1 MB (86092192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cd5495defa6104e2de9f25e839f70d94c3f7d9d1483c96e4715a0b5e174051`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 5.6 KB (5557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7486c3648f7981d487c319e9f2b49e67c2afc3ac328cf02f883afa530140b7ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137575866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82eca8349acd403244c99ccbe1a3e521d344e936ce5f652565474fe2e7eff326`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:24:08 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 18 Jun 2021 20:24:17 GMT
ENV MARIADB_VERSION=1:10.5.10+maria~focal
# Fri, 18 Jun 2021 20:24:24 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:27:21 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:27:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:27:37 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:27:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:27:56 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:28:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8532e19b2d04c2f706f2ac99f0bb3668325be370240666551599d45bb235be`  
		Last Modified: Fri, 18 Jun 2021 20:43:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0073b8bf118bde577f45635ca2f109e22354e72c15b6bf19551790da0db0ddb2`  
		Last Modified: Fri, 18 Jun 2021 20:44:08 GMT  
		Size: 91.3 MB (91323812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a383425a57e912232095db76f4b2a86b914621e7b899c6549dc1e9415d686e`  
		Last Modified: Fri, 18 Jun 2021 20:43:44 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:e42a43b7912f941d61641f5e326e66e6a73e5d3ecbb36e225f44e0fae86abaeb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:0dacf119003824f9fb12d82c019195050f1d68c2266e8a884513c2cc82615051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126881550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:104f4e7cbe8335d5a59bf4e85abe94402c46898ac01ba76f54e12350b077409b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:20:55 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 18 Jun 2021 20:20:55 GMT
ENV MARIADB_VERSION=1:10.5.10+maria~focal
# Fri, 18 Jun 2021 20:20:56 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:21:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:21:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:21:16 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:21:17 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:21:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc09fec0bce19701fafca0528b5b09a1559a67156fbdc04a5424395c24b676d3`  
		Last Modified: Fri, 18 Jun 2021 20:24:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9b9043bdda0e2583685296da540210290363752743edfd54bd88fae50d104c`  
		Last Modified: Fri, 18 Jun 2021 20:24:48 GMT  
		Size: 86.9 MB (86938711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e596ee38c508da37313418760e43b1e20273d93de33bf8d544da5845d9be5a`  
		Last Modified: Fri, 18 Jun 2021 20:24:34 GMT  
		Size: 5.6 KB (5561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:54b51624f0f714e43cc58f982b525f3a8088b0f4da13b800b3c47a078806da2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124329014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e57d78eb4a332152d529b6ba2af0d085fe4ffbe9a38fd957c1f612c52fba82d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Thu, 24 Jun 2021 01:33:35 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:34:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:34:14 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:34:15 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:34:15 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:34:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16178d1583fbf0339abc345a26f507e8a48e182309e515331c40256d4a05857`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537120db29a4871816e11bfa94ce0bfbcbc843cafcafbaa75a251e73a2eb62d8`  
		Last Modified: Thu, 24 Jun 2021 01:38:38 GMT  
		Size: 86.1 MB (86092192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cd5495defa6104e2de9f25e839f70d94c3f7d9d1483c96e4715a0b5e174051`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 5.6 KB (5557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7486c3648f7981d487c319e9f2b49e67c2afc3ac328cf02f883afa530140b7ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137575866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82eca8349acd403244c99ccbe1a3e521d344e936ce5f652565474fe2e7eff326`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:24:08 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 18 Jun 2021 20:24:17 GMT
ENV MARIADB_VERSION=1:10.5.10+maria~focal
# Fri, 18 Jun 2021 20:24:24 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:27:21 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:27:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:27:37 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:27:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:27:56 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:28:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8532e19b2d04c2f706f2ac99f0bb3668325be370240666551599d45bb235be`  
		Last Modified: Fri, 18 Jun 2021 20:43:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0073b8bf118bde577f45635ca2f109e22354e72c15b6bf19551790da0db0ddb2`  
		Last Modified: Fri, 18 Jun 2021 20:44:08 GMT  
		Size: 91.3 MB (91323812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a383425a57e912232095db76f4b2a86b914621e7b899c6549dc1e9415d686e`  
		Last Modified: Fri, 18 Jun 2021 20:43:44 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.11`

```console
$ docker pull mariadb@sha256:c43a865a08486da444c66f9489137a44e6310489b62818db335b2bb3e1367281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `mariadb:10.5.11` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:54b51624f0f714e43cc58f982b525f3a8088b0f4da13b800b3c47a078806da2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124329014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e57d78eb4a332152d529b6ba2af0d085fe4ffbe9a38fd957c1f612c52fba82d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Thu, 24 Jun 2021 01:33:35 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:34:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:34:14 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:34:15 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:34:15 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:34:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16178d1583fbf0339abc345a26f507e8a48e182309e515331c40256d4a05857`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537120db29a4871816e11bfa94ce0bfbcbc843cafcafbaa75a251e73a2eb62d8`  
		Last Modified: Thu, 24 Jun 2021 01:38:38 GMT  
		Size: 86.1 MB (86092192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cd5495defa6104e2de9f25e839f70d94c3f7d9d1483c96e4715a0b5e174051`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 5.6 KB (5557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.11-focal`

```console
$ docker pull mariadb@sha256:c43a865a08486da444c66f9489137a44e6310489b62818db335b2bb3e1367281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `mariadb:10.5.11-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:54b51624f0f714e43cc58f982b525f3a8088b0f4da13b800b3c47a078806da2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124329014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e57d78eb4a332152d529b6ba2af0d085fe4ffbe9a38fd957c1f612c52fba82d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Thu, 24 Jun 2021 01:33:35 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:34:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:34:14 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:34:15 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:34:15 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:34:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16178d1583fbf0339abc345a26f507e8a48e182309e515331c40256d4a05857`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537120db29a4871816e11bfa94ce0bfbcbc843cafcafbaa75a251e73a2eb62d8`  
		Last Modified: Thu, 24 Jun 2021 01:38:38 GMT  
		Size: 86.1 MB (86092192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cd5495defa6104e2de9f25e839f70d94c3f7d9d1483c96e4715a0b5e174051`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 5.6 KB (5557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6`

```console
$ docker pull mariadb@sha256:e94cab21b4854a22eadc9f47041d75cf0a32c6bd27eade0e023e4087dd2ca659
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.6` - linux; amd64

```console
$ docker pull mariadb@sha256:8a70e1ff827c1a5265dc5059565211895d08c9cdd40236563ce33c1025aecee6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127064717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1194b17dd8f6cc845b59fdd6361e90402dec921130b7a3ac46c05ce9db90e6a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:20:15 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 18 Jun 2021 20:20:15 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Fri, 18 Jun 2021 20:20:16 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:20:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:20:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:20:47 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:20:48 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:20:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46c89c89f130dda4a2fa8535cd1d8c5211aa68796677eb190da5910a3a378d9`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cf32a0c32dd01bdc9c2e65cd6570a7dcc53d8697f0ae58300fac8079111ed8`  
		Last Modified: Fri, 18 Jun 2021 20:24:11 GMT  
		Size: 87.1 MB (87121878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a44a8662fe3beb1c65e1bb841a29a4b1bc2b4fa5bbec10fef70f15cb3bfbd07`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 5.6 KB (5563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bc186d369af050d6065c6f8cd277492b00f083b572cde6440b2be14929f08d5b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124293286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca43f26751177c92b70303c7f4c2aaec6425cced8ba479c2f5f3f2828e6a1f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:32:44 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 24 Jun 2021 01:32:44 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Thu, 24 Jun 2021 01:32:45 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:33:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:33:25 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:33:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:33:25 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:33:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9f6c58f8b1dd9f6e007c94d11c40e5f63c5334f7dc4212daa2153498c834ce`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c1a9f4904d693f1233c6e77e047f52e8692fd0ba95e562a0358e45d7fb8fd2`  
		Last Modified: Thu, 24 Jun 2021 01:37:55 GMT  
		Size: 86.1 MB (86056462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447571cb35ec60414b6f5e8057e45c29f379dd47eaa0fffc57d0989a87e3e3c`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e5ea27c4659828d903bfaec73e823da8a30f0144cd4e0cf3ef2717e6413fd157
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137562072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d55ab5148f5c99bf5173676f8af1c0e6c638f316a79d697b45b37db17301b67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:19:25 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 18 Jun 2021 20:19:31 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Fri, 18 Jun 2021 20:19:39 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:23:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:23:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:23:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:23:42 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:23:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd51d778c2a9acc80476f042540922f747bfdf693589303bfbcf5ec3334d71f8`  
		Last Modified: Fri, 18 Jun 2021 20:42:59 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80053c8c97e82889a941bde0aa93e79aca4bf587575f3db5042297b35b0fb32`  
		Last Modified: Fri, 18 Jun 2021 20:43:19 GMT  
		Size: 91.3 MB (91310013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2845b91337a7b3da573f5c4185ea80e4236844fb1524b3030133269675abd8eb`  
		Last Modified: Fri, 18 Jun 2021 20:42:59 GMT  
		Size: 5.6 KB (5563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6-focal`

```console
$ docker pull mariadb@sha256:e94cab21b4854a22eadc9f47041d75cf0a32c6bd27eade0e023e4087dd2ca659
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.6-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:8a70e1ff827c1a5265dc5059565211895d08c9cdd40236563ce33c1025aecee6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127064717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1194b17dd8f6cc845b59fdd6361e90402dec921130b7a3ac46c05ce9db90e6a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:20:15 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 18 Jun 2021 20:20:15 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Fri, 18 Jun 2021 20:20:16 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:20:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:20:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:20:47 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:20:48 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:20:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46c89c89f130dda4a2fa8535cd1d8c5211aa68796677eb190da5910a3a378d9`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cf32a0c32dd01bdc9c2e65cd6570a7dcc53d8697f0ae58300fac8079111ed8`  
		Last Modified: Fri, 18 Jun 2021 20:24:11 GMT  
		Size: 87.1 MB (87121878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a44a8662fe3beb1c65e1bb841a29a4b1bc2b4fa5bbec10fef70f15cb3bfbd07`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 5.6 KB (5563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bc186d369af050d6065c6f8cd277492b00f083b572cde6440b2be14929f08d5b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124293286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca43f26751177c92b70303c7f4c2aaec6425cced8ba479c2f5f3f2828e6a1f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:32:44 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 24 Jun 2021 01:32:44 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Thu, 24 Jun 2021 01:32:45 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:33:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:33:25 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:33:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:33:25 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:33:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9f6c58f8b1dd9f6e007c94d11c40e5f63c5334f7dc4212daa2153498c834ce`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c1a9f4904d693f1233c6e77e047f52e8692fd0ba95e562a0358e45d7fb8fd2`  
		Last Modified: Thu, 24 Jun 2021 01:37:55 GMT  
		Size: 86.1 MB (86056462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447571cb35ec60414b6f5e8057e45c29f379dd47eaa0fffc57d0989a87e3e3c`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e5ea27c4659828d903bfaec73e823da8a30f0144cd4e0cf3ef2717e6413fd157
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137562072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d55ab5148f5c99bf5173676f8af1c0e6c638f316a79d697b45b37db17301b67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:19:25 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 18 Jun 2021 20:19:31 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Fri, 18 Jun 2021 20:19:39 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:23:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:23:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:23:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:23:42 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:23:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd51d778c2a9acc80476f042540922f747bfdf693589303bfbcf5ec3334d71f8`  
		Last Modified: Fri, 18 Jun 2021 20:42:59 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80053c8c97e82889a941bde0aa93e79aca4bf587575f3db5042297b35b0fb32`  
		Last Modified: Fri, 18 Jun 2021 20:43:19 GMT  
		Size: 91.3 MB (91310013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2845b91337a7b3da573f5c4185ea80e4236844fb1524b3030133269675abd8eb`  
		Last Modified: Fri, 18 Jun 2021 20:42:59 GMT  
		Size: 5.6 KB (5563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.2`

```console
$ docker pull mariadb@sha256:e94cab21b4854a22eadc9f47041d75cf0a32c6bd27eade0e023e4087dd2ca659
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.6.2` - linux; amd64

```console
$ docker pull mariadb@sha256:8a70e1ff827c1a5265dc5059565211895d08c9cdd40236563ce33c1025aecee6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127064717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1194b17dd8f6cc845b59fdd6361e90402dec921130b7a3ac46c05ce9db90e6a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:20:15 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 18 Jun 2021 20:20:15 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Fri, 18 Jun 2021 20:20:16 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:20:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:20:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:20:47 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:20:48 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:20:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46c89c89f130dda4a2fa8535cd1d8c5211aa68796677eb190da5910a3a378d9`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cf32a0c32dd01bdc9c2e65cd6570a7dcc53d8697f0ae58300fac8079111ed8`  
		Last Modified: Fri, 18 Jun 2021 20:24:11 GMT  
		Size: 87.1 MB (87121878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a44a8662fe3beb1c65e1bb841a29a4b1bc2b4fa5bbec10fef70f15cb3bfbd07`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 5.6 KB (5563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bc186d369af050d6065c6f8cd277492b00f083b572cde6440b2be14929f08d5b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124293286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca43f26751177c92b70303c7f4c2aaec6425cced8ba479c2f5f3f2828e6a1f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:32:44 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 24 Jun 2021 01:32:44 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Thu, 24 Jun 2021 01:32:45 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:33:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:33:25 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:33:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:33:25 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:33:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9f6c58f8b1dd9f6e007c94d11c40e5f63c5334f7dc4212daa2153498c834ce`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c1a9f4904d693f1233c6e77e047f52e8692fd0ba95e562a0358e45d7fb8fd2`  
		Last Modified: Thu, 24 Jun 2021 01:37:55 GMT  
		Size: 86.1 MB (86056462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447571cb35ec60414b6f5e8057e45c29f379dd47eaa0fffc57d0989a87e3e3c`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e5ea27c4659828d903bfaec73e823da8a30f0144cd4e0cf3ef2717e6413fd157
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137562072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d55ab5148f5c99bf5173676f8af1c0e6c638f316a79d697b45b37db17301b67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:19:25 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 18 Jun 2021 20:19:31 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Fri, 18 Jun 2021 20:19:39 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:23:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:23:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:23:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:23:42 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:23:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd51d778c2a9acc80476f042540922f747bfdf693589303bfbcf5ec3334d71f8`  
		Last Modified: Fri, 18 Jun 2021 20:42:59 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80053c8c97e82889a941bde0aa93e79aca4bf587575f3db5042297b35b0fb32`  
		Last Modified: Fri, 18 Jun 2021 20:43:19 GMT  
		Size: 91.3 MB (91310013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2845b91337a7b3da573f5c4185ea80e4236844fb1524b3030133269675abd8eb`  
		Last Modified: Fri, 18 Jun 2021 20:42:59 GMT  
		Size: 5.6 KB (5563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.6.2-focal`

```console
$ docker pull mariadb@sha256:e94cab21b4854a22eadc9f47041d75cf0a32c6bd27eade0e023e4087dd2ca659
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.6.2-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:8a70e1ff827c1a5265dc5059565211895d08c9cdd40236563ce33c1025aecee6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127064717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1194b17dd8f6cc845b59fdd6361e90402dec921130b7a3ac46c05ce9db90e6a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:20:15 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 18 Jun 2021 20:20:15 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Fri, 18 Jun 2021 20:20:16 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:20:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:20:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:20:47 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:20:48 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:20:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46c89c89f130dda4a2fa8535cd1d8c5211aa68796677eb190da5910a3a378d9`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cf32a0c32dd01bdc9c2e65cd6570a7dcc53d8697f0ae58300fac8079111ed8`  
		Last Modified: Fri, 18 Jun 2021 20:24:11 GMT  
		Size: 87.1 MB (87121878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a44a8662fe3beb1c65e1bb841a29a4b1bc2b4fa5bbec10fef70f15cb3bfbd07`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 5.6 KB (5563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.2-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bc186d369af050d6065c6f8cd277492b00f083b572cde6440b2be14929f08d5b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124293286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca43f26751177c92b70303c7f4c2aaec6425cced8ba479c2f5f3f2828e6a1f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:32:44 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 24 Jun 2021 01:32:44 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Thu, 24 Jun 2021 01:32:45 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:33:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:33:25 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:33:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:33:25 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:33:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9f6c58f8b1dd9f6e007c94d11c40e5f63c5334f7dc4212daa2153498c834ce`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c1a9f4904d693f1233c6e77e047f52e8692fd0ba95e562a0358e45d7fb8fd2`  
		Last Modified: Thu, 24 Jun 2021 01:37:55 GMT  
		Size: 86.1 MB (86056462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447571cb35ec60414b6f5e8057e45c29f379dd47eaa0fffc57d0989a87e3e3c`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.6.2-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e5ea27c4659828d903bfaec73e823da8a30f0144cd4e0cf3ef2717e6413fd157
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137562072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d55ab5148f5c99bf5173676f8af1c0e6c638f316a79d697b45b37db17301b67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:19:25 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 18 Jun 2021 20:19:31 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Fri, 18 Jun 2021 20:19:39 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:23:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:23:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:23:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:23:42 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:23:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd51d778c2a9acc80476f042540922f747bfdf693589303bfbcf5ec3334d71f8`  
		Last Modified: Fri, 18 Jun 2021 20:42:59 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80053c8c97e82889a941bde0aa93e79aca4bf587575f3db5042297b35b0fb32`  
		Last Modified: Fri, 18 Jun 2021 20:43:19 GMT  
		Size: 91.3 MB (91310013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2845b91337a7b3da573f5c4185ea80e4236844fb1524b3030133269675abd8eb`  
		Last Modified: Fri, 18 Jun 2021 20:42:59 GMT  
		Size: 5.6 KB (5563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:e42a43b7912f941d61641f5e326e66e6a73e5d3ecbb36e225f44e0fae86abaeb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:0dacf119003824f9fb12d82c019195050f1d68c2266e8a884513c2cc82615051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126881550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:104f4e7cbe8335d5a59bf4e85abe94402c46898ac01ba76f54e12350b077409b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:20:55 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 18 Jun 2021 20:20:55 GMT
ENV MARIADB_VERSION=1:10.5.10+maria~focal
# Fri, 18 Jun 2021 20:20:56 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:21:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:21:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:21:16 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:21:17 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:21:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc09fec0bce19701fafca0528b5b09a1559a67156fbdc04a5424395c24b676d3`  
		Last Modified: Fri, 18 Jun 2021 20:24:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9b9043bdda0e2583685296da540210290363752743edfd54bd88fae50d104c`  
		Last Modified: Fri, 18 Jun 2021 20:24:48 GMT  
		Size: 86.9 MB (86938711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e596ee38c508da37313418760e43b1e20273d93de33bf8d544da5845d9be5a`  
		Last Modified: Fri, 18 Jun 2021 20:24:34 GMT  
		Size: 5.6 KB (5561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:54b51624f0f714e43cc58f982b525f3a8088b0f4da13b800b3c47a078806da2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124329014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e57d78eb4a332152d529b6ba2af0d085fe4ffbe9a38fd957c1f612c52fba82d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Thu, 24 Jun 2021 01:33:35 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:34:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:34:14 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:34:15 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:34:15 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:34:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16178d1583fbf0339abc345a26f507e8a48e182309e515331c40256d4a05857`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537120db29a4871816e11bfa94ce0bfbcbc843cafcafbaa75a251e73a2eb62d8`  
		Last Modified: Thu, 24 Jun 2021 01:38:38 GMT  
		Size: 86.1 MB (86092192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cd5495defa6104e2de9f25e839f70d94c3f7d9d1483c96e4715a0b5e174051`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 5.6 KB (5557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7486c3648f7981d487c319e9f2b49e67c2afc3ac328cf02f883afa530140b7ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137575866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82eca8349acd403244c99ccbe1a3e521d344e936ce5f652565474fe2e7eff326`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:24:08 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 18 Jun 2021 20:24:17 GMT
ENV MARIADB_VERSION=1:10.5.10+maria~focal
# Fri, 18 Jun 2021 20:24:24 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:27:21 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:27:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:27:37 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:27:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:27:56 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:28:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8532e19b2d04c2f706f2ac99f0bb3668325be370240666551599d45bb235be`  
		Last Modified: Fri, 18 Jun 2021 20:43:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0073b8bf118bde577f45635ca2f109e22354e72c15b6bf19551790da0db0ddb2`  
		Last Modified: Fri, 18 Jun 2021 20:44:08 GMT  
		Size: 91.3 MB (91323812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a383425a57e912232095db76f4b2a86b914621e7b899c6549dc1e9415d686e`  
		Last Modified: Fri, 18 Jun 2021 20:43:44 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:e42a43b7912f941d61641f5e326e66e6a73e5d3ecbb36e225f44e0fae86abaeb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:0dacf119003824f9fb12d82c019195050f1d68c2266e8a884513c2cc82615051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126881550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:104f4e7cbe8335d5a59bf4e85abe94402c46898ac01ba76f54e12350b077409b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:20:55 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 18 Jun 2021 20:20:55 GMT
ENV MARIADB_VERSION=1:10.5.10+maria~focal
# Fri, 18 Jun 2021 20:20:56 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:21:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:21:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:21:16 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:21:17 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:21:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc09fec0bce19701fafca0528b5b09a1559a67156fbdc04a5424395c24b676d3`  
		Last Modified: Fri, 18 Jun 2021 20:24:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9b9043bdda0e2583685296da540210290363752743edfd54bd88fae50d104c`  
		Last Modified: Fri, 18 Jun 2021 20:24:48 GMT  
		Size: 86.9 MB (86938711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e596ee38c508da37313418760e43b1e20273d93de33bf8d544da5845d9be5a`  
		Last Modified: Fri, 18 Jun 2021 20:24:34 GMT  
		Size: 5.6 KB (5561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:54b51624f0f714e43cc58f982b525f3a8088b0f4da13b800b3c47a078806da2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124329014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e57d78eb4a332152d529b6ba2af0d085fe4ffbe9a38fd957c1f612c52fba82d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 24 Jun 2021 01:33:34 GMT
ENV MARIADB_VERSION=1:10.5.11+maria~focal
# Thu, 24 Jun 2021 01:33:35 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:34:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:34:14 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:34:15 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:34:15 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:34:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16178d1583fbf0339abc345a26f507e8a48e182309e515331c40256d4a05857`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537120db29a4871816e11bfa94ce0bfbcbc843cafcafbaa75a251e73a2eb62d8`  
		Last Modified: Thu, 24 Jun 2021 01:38:38 GMT  
		Size: 86.1 MB (86092192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cd5495defa6104e2de9f25e839f70d94c3f7d9d1483c96e4715a0b5e174051`  
		Last Modified: Thu, 24 Jun 2021 01:38:22 GMT  
		Size: 5.6 KB (5557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:7486c3648f7981d487c319e9f2b49e67c2afc3ac328cf02f883afa530140b7ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137575866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82eca8349acd403244c99ccbe1a3e521d344e936ce5f652565474fe2e7eff326`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:24:08 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 18 Jun 2021 20:24:17 GMT
ENV MARIADB_VERSION=1:10.5.10+maria~focal
# Fri, 18 Jun 2021 20:24:24 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:27:21 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:27:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:27:37 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:27:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:27:56 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:28:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8532e19b2d04c2f706f2ac99f0bb3668325be370240666551599d45bb235be`  
		Last Modified: Fri, 18 Jun 2021 20:43:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0073b8bf118bde577f45635ca2f109e22354e72c15b6bf19551790da0db0ddb2`  
		Last Modified: Fri, 18 Jun 2021 20:44:08 GMT  
		Size: 91.3 MB (91323812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a383425a57e912232095db76f4b2a86b914621e7b899c6549dc1e9415d686e`  
		Last Modified: Fri, 18 Jun 2021 20:43:44 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:rc`

```console
$ docker pull mariadb@sha256:e94cab21b4854a22eadc9f47041d75cf0a32c6bd27eade0e023e4087dd2ca659
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:rc` - linux; amd64

```console
$ docker pull mariadb@sha256:8a70e1ff827c1a5265dc5059565211895d08c9cdd40236563ce33c1025aecee6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127064717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1194b17dd8f6cc845b59fdd6361e90402dec921130b7a3ac46c05ce9db90e6a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:20:15 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 18 Jun 2021 20:20:15 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Fri, 18 Jun 2021 20:20:16 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:20:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:20:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:20:47 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:20:48 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:20:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46c89c89f130dda4a2fa8535cd1d8c5211aa68796677eb190da5910a3a378d9`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cf32a0c32dd01bdc9c2e65cd6570a7dcc53d8697f0ae58300fac8079111ed8`  
		Last Modified: Fri, 18 Jun 2021 20:24:11 GMT  
		Size: 87.1 MB (87121878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a44a8662fe3beb1c65e1bb841a29a4b1bc2b4fa5bbec10fef70f15cb3bfbd07`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 5.6 KB (5563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:rc` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bc186d369af050d6065c6f8cd277492b00f083b572cde6440b2be14929f08d5b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124293286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca43f26751177c92b70303c7f4c2aaec6425cced8ba479c2f5f3f2828e6a1f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:32:44 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 24 Jun 2021 01:32:44 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Thu, 24 Jun 2021 01:32:45 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:33:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:33:25 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:33:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:33:25 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:33:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9f6c58f8b1dd9f6e007c94d11c40e5f63c5334f7dc4212daa2153498c834ce`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c1a9f4904d693f1233c6e77e047f52e8692fd0ba95e562a0358e45d7fb8fd2`  
		Last Modified: Thu, 24 Jun 2021 01:37:55 GMT  
		Size: 86.1 MB (86056462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447571cb35ec60414b6f5e8057e45c29f379dd47eaa0fffc57d0989a87e3e3c`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:rc` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e5ea27c4659828d903bfaec73e823da8a30f0144cd4e0cf3ef2717e6413fd157
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137562072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d55ab5148f5c99bf5173676f8af1c0e6c638f316a79d697b45b37db17301b67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:19:25 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 18 Jun 2021 20:19:31 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Fri, 18 Jun 2021 20:19:39 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:23:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:23:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:23:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:23:42 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:23:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd51d778c2a9acc80476f042540922f747bfdf693589303bfbcf5ec3334d71f8`  
		Last Modified: Fri, 18 Jun 2021 20:42:59 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80053c8c97e82889a941bde0aa93e79aca4bf587575f3db5042297b35b0fb32`  
		Last Modified: Fri, 18 Jun 2021 20:43:19 GMT  
		Size: 91.3 MB (91310013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2845b91337a7b3da573f5c4185ea80e4236844fb1524b3030133269675abd8eb`  
		Last Modified: Fri, 18 Jun 2021 20:42:59 GMT  
		Size: 5.6 KB (5563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:rc-focal`

```console
$ docker pull mariadb@sha256:e94cab21b4854a22eadc9f47041d75cf0a32c6bd27eade0e023e4087dd2ca659
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:rc-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:8a70e1ff827c1a5265dc5059565211895d08c9cdd40236563ce33c1025aecee6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127064717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1194b17dd8f6cc845b59fdd6361e90402dec921130b7a3ac46c05ce9db90e6a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:56:17 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 04:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:56:24 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 04:56:35 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 04:56:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:20:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:20:14 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:20:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:20:15 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 18 Jun 2021 20:20:15 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Fri, 18 Jun 2021 20:20:16 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:20:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:20:47 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:20:47 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:20:48 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:20:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea6552a46225f37637d406d551ee8fc04ad670606749bf77583984e305763f`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329b1f41043f334fc046ee77daca5b1f2da2680818c346eac07cd10135c85bec`  
		Last Modified: Fri, 18 Jun 2021 05:01:24 GMT  
		Size: 5.5 MB (5488775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d09317d80bcdbde01a7d4984a0d06edfc3b8284f2bb9a81401f0dd7b4f3be`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 3.6 MB (3615926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc055a5511da95c2f42bf255ff0275c86b2e09ad80b7360a2bb717683fe5ce6`  
		Last Modified: Fri, 18 Jun 2021 05:01:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e989e430508e65c0e3a39b9dde525b30ad0abf989e435d9e60ee539a86e8709e`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.3 MB (2274172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c98fa16f6cc547e5ae7b8d48b3bcccb781edb4ec3122bb2507b1f6fc44b55`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 2.5 KB (2485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46c89c89f130dda4a2fa8535cd1d8c5211aa68796677eb190da5910a3a378d9`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cf32a0c32dd01bdc9c2e65cd6570a7dcc53d8697f0ae58300fac8079111ed8`  
		Last Modified: Fri, 18 Jun 2021 20:24:11 GMT  
		Size: 87.1 MB (87121878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a44a8662fe3beb1c65e1bb841a29a4b1bc2b4fa5bbec10fef70f15cb3bfbd07`  
		Last Modified: Fri, 18 Jun 2021 20:23:57 GMT  
		Size: 5.6 KB (5563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:rc-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:bc186d369af050d6065c6f8cd277492b00f083b572cde6440b2be14929f08d5b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124293286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca43f26751177c92b70303c7f4c2aaec6425cced8ba479c2f5f3f2828e6a1f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:58 GMT
ADD file:9e94a579f0495fce8fac6889d0b9b2cd576d5b3ce9f18ff913ad99a503756769 in / 
# Thu, 17 Jun 2021 23:53:59 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:46:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 00:46:18 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:46:18 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:46:31 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:46:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:39:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:39:54 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 24 Jun 2021 01:32:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:32:44 GMT
ENV MARIADB_MAJOR=10.6
# Thu, 24 Jun 2021 01:32:44 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Thu, 24 Jun 2021 01:32:45 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 24 Jun 2021 01:33:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Thu, 24 Jun 2021 01:33:25 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Jun 2021 01:33:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:33:25 GMT
EXPOSE 3306
# Thu, 24 Jun 2021 01:33:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f86eded34a1950318569803a7e0c689175ebd9d76faf08798f88ac133b98a11`  
		Last Modified: Thu, 17 Jun 2021 23:56:04 GMT  
		Size: 27.2 MB (27158803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2fb22009549c382a13f19944b1f677fbd86342fb82606d2d32e270f103554`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 1.8 KB (1755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd425bf20e5a7b2f63ecc734c73ed6a0c78454e5db14f76a86cd5c725df84f42`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 5.5 MB (5455206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a1c12283e615cc52b8120fdf6b5790c90d118fa8f81ee02ec0eaef891fa69`  
		Last Modified: Fri, 18 Jun 2021 00:51:08 GMT  
		Size: 3.4 MB (3408886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aacdc09bed9ec05785f9401269330f831c51a52299e1e3f31d12b6ea17dab5f`  
		Last Modified: Fri, 18 Jun 2021 00:51:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc26e3e6fe0dbbcb92e52ef4284fcc376384aac72c48c3ba98445839c7d7345`  
		Last Modified: Fri, 18 Jun 2021 20:44:31 GMT  
		Size: 2.2 MB (2203652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e227d95049d44f8f91a2ee32cbc86aa120d4ff4118e4dd797dc1e955ce4bcb`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9f6c58f8b1dd9f6e007c94d11c40e5f63c5334f7dc4212daa2153498c834ce`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c1a9f4904d693f1233c6e77e047f52e8692fd0ba95e562a0358e45d7fb8fd2`  
		Last Modified: Thu, 24 Jun 2021 01:37:55 GMT  
		Size: 86.1 MB (86056462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447571cb35ec60414b6f5e8057e45c29f379dd47eaa0fffc57d0989a87e3e3c`  
		Last Modified: Thu, 24 Jun 2021 01:37:39 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:rc-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e5ea27c4659828d903bfaec73e823da8a30f0144cd4e0cf3ef2717e6413fd157
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137562072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d55ab5148f5c99bf5173676f8af1c0e6c638f316a79d697b45b37db17301b67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 02:33:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 18 Jun 2021 02:35:05 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 02:35:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 02:35:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 02:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Jun 2021 20:19:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 20:19:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 18 Jun 2021 20:19:20 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 18 Jun 2021 20:19:25 GMT
ENV MARIADB_MAJOR=10.6
# Fri, 18 Jun 2021 20:19:31 GMT
ENV MARIADB_VERSION=1:10.6.2+maria~focal
# Fri, 18 Jun 2021 20:19:39 GMT
RUN set -e;	echo "deb https://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 18 Jun 2021 20:23:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 18 Jun 2021 20:23:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 18 Jun 2021 20:23:25 GMT
COPY file:c520fc9f2984356e1beb79d000d5a8bf0994e8d4f935e1eeb8b253dcf83d538c in /usr/local/bin/ 
# Fri, 18 Jun 2021 20:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 20:23:42 GMT
EXPOSE 3306
# Fri, 18 Jun 2021 20:23:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892130860a067fec368c20f64f2f559deb8e9247d04a6b64ce46b0a114063e50`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c39b896efee4493ae5781757a9d5284e14a7a25ca343ff220681cde01cbf42a`  
		Last Modified: Fri, 18 Jun 2021 03:03:15 GMT  
		Size: 6.7 MB (6667940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd80d1608d833d5aea73f684fecec978d139c0929ec3d1c69c92a4ee5db0b1f`  
		Last Modified: Fri, 18 Jun 2021 03:03:14 GMT  
		Size: 3.7 MB (3725668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b8437f7227b0b42d011a9e3e8cd2e8a8bbdd7593d4c491adca03444c024021`  
		Last Modified: Fri, 18 Jun 2021 03:03:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d80b2e396d62c54b31fd3a438cb63e306ab811fb19d184e1a31a239d42bfc33`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.6 MB (2569918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d169f67d295b0793d551f8fb3648569f03858d4aad1409941a653cad6930fdd`  
		Last Modified: Fri, 18 Jun 2021 20:43:00 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd51d778c2a9acc80476f042540922f747bfdf693589303bfbcf5ec3334d71f8`  
		Last Modified: Fri, 18 Jun 2021 20:42:59 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80053c8c97e82889a941bde0aa93e79aca4bf587575f3db5042297b35b0fb32`  
		Last Modified: Fri, 18 Jun 2021 20:43:19 GMT  
		Size: 91.3 MB (91310013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2845b91337a7b3da573f5c4185ea80e4236844fb1524b3030133269675abd8eb`  
		Last Modified: Fri, 18 Jun 2021 20:42:59 GMT  
		Size: 5.6 KB (5563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
