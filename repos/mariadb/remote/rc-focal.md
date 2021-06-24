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
