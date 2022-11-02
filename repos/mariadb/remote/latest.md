## `mariadb:latest`

```console
$ docker pull mariadb@sha256:bb39098029f443e8b02a1736c3cb4be1c5d6663a8355d4f9eb0b05693df4b9a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:b516afae7c1b82e954bfefe011fc4df71d37f0ad0386bb4f5fe381c23b938984
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124051111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dafde72c039711e0329c566e7bf25a7205370b638d96ccc6d7d58c514089e1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:56:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 19:56:24 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:56:24 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 19:56:34 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 19:56:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 19:56:42 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:56:42 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 19:56:44 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 19:57:27 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 19:57:27 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 19:57:27 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 19:57:27 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 19:57:47 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 19:57:48 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 19:57:48 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 19:57:48 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 19:57:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 19:57:48 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 19:57:48 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13360dd5ccba7386fb34c2af66a6c1fea57fb7e83869864e15e1402d8ab746c5`  
		Last Modified: Wed, 02 Nov 2022 19:59:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7faf2e389f4fb799dfe705e363ab37161753556bd5df80f620c0dcf278ff6ff`  
		Last Modified: Wed, 02 Nov 2022 19:59:10 GMT  
		Size: 3.8 MB (3766026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff396cb19fe89c505ab684fb7ff958bc5bf0c49cc8efcd2bb03b20f80b82c32`  
		Last Modified: Wed, 02 Nov 2022 19:59:09 GMT  
		Size: 2.0 MB (1993479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f37cc3e4aac99c1fb0a623f44e3928ab378d22f6aaf5de28d54c47a3abf7be`  
		Last Modified: Wed, 02 Nov 2022 19:59:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08d9a14685313fc476b8c2fb0a57bda7869de9b7a178639d20860b7244d0e06`  
		Last Modified: Wed, 02 Nov 2022 19:59:09 GMT  
		Size: 2.3 MB (2280815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b24ce4edb73ae87cf7e069006c2bb71f2761eb68492246a3016fd00ad133567`  
		Last Modified: Wed, 02 Nov 2022 19:59:07 GMT  
		Size: 2.5 KB (2490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9aeeef984228c7924ea8fbfafd5b686715f37427522ac25f263cb31f211a5a`  
		Last Modified: Wed, 02 Nov 2022 19:59:35 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfe27382d40865ba7211b73755683bc2668b025fbdfacac48de80b3247dd615`  
		Last Modified: Wed, 02 Nov 2022 19:59:48 GMT  
		Size: 85.6 MB (85569933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b793b98f634e8d7a4c20770b66f79672d76204fc2ddaa25237acd76dbd75c451`  
		Last Modified: Wed, 02 Nov 2022 19:59:35 GMT  
		Size: 3.5 KB (3490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ce5b27f82288ed63b2374cd64f92ba20739de29d63c6ae2dc0d13349ca30f`  
		Last Modified: Wed, 02 Nov 2022 19:59:35 GMT  
		Size: 7.0 KB (7049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:31f677ba9b50beef8d48a3bbcab29485f5aa3a90677d1ebc44039bbc9bc8bde4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118604917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe889c390f208ce09bf8bfa7869b7d342d999c4279a8809e3a2d2a14332cf10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 20:07:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 20:07:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:35 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 20:07:45 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 20:07:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 20:07:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:07:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 20:07:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 20:08:36 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 20:08:36 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 20:08:36 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 20:08:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 20:08:55 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 20:08:55 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 20:08:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:08:55 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 20:08:55 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf568f815bdc2b755b642d6cad079d9e2e71dd364d2806bf4a9a3cb0fe3d18b7`  
		Last Modified: Wed, 02 Nov 2022 20:10:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5a27635d8616b3a361adc11c7e5712c05d3edef95c0573370b2c92058ed582`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 3.7 MB (3737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbce0b0cfd1e867e47d514f1de07a5da365d36bfb15513e7cf310802577ab13c`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 1.9 MB (1898793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd291b4a9d31c95c30d2580b470dd4ecbe4d2d10c11e47967a037f8b939146e`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d505d811110d4c6311181f11307bd36ac49e38d1ab561c611e562b293b90a9ef`  
		Last Modified: Wed, 02 Nov 2022 20:10:12 GMT  
		Size: 2.2 MB (2191982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf7ac4a18820861abff79a668773c9f881f45b6f47d10f21df0661e7190013b`  
		Last Modified: Wed, 02 Nov 2022 20:10:09 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5452b6a0ce3706d857279cfa1cdaef7c8b6bc76d8d6a4b1c43367203b766cd2f`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2628f7ef3cedd084f9a47495aa153853592da56561a6e3231a78435d95ff9949`  
		Last Modified: Wed, 02 Nov 2022 20:10:44 GMT  
		Size: 82.4 MB (82378919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e903661ffaca59211d235a8061c23cc51afe2459c91999d6e191b263897d86d0`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 3.5 KB (3489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ecec752f0246a09512597065787135cfb39650e56b627521d6b7a25b44bec`  
		Last Modified: Wed, 02 Nov 2022 20:10:34 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:986c35ba43c2850b7911d84081331f918000e38549e853630add39e459d49f28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117016669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e47acd883e8abe5eff966b7822646acd0bed0c6a192953367a3f79b231e3b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:12:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 19:12:26 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:12:26 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 19:12:44 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 19:12:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 19:12:58 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:12:58 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 19:13:01 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 19:14:08 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 19:14:08 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 19:14:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 19:14:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 19:14:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 19:14:58 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 19:14:58 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 19:14:59 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 19:14:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 19:14:59 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 19:15:00 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac86ff494d3eaf7d95f57bc74e48f4685e8a686b8520aa0c196d6add814e1664`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfeb46b3a1843b7ee9d01cc3d48d5188828832d30e02658a1f40e173b56774e`  
		Last Modified: Wed, 02 Nov 2022 19:17:53 GMT  
		Size: 4.5 MB (4503387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e67838a2b5666564d1410b1813495680475321a9fafc2c1181fd2c890ee43b4`  
		Last Modified: Wed, 02 Nov 2022 19:17:52 GMT  
		Size: 1.9 MB (1922247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004a22c7ec4673456e7895bcc12a8260c27e5d63f8cfbb89e497188c0ff56c06`  
		Last Modified: Wed, 02 Nov 2022 19:17:51 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a81eb319d6a4b7adfa30e05763ab3f2ee3a8f692c43979b744cc4b7a898543`  
		Last Modified: Wed, 02 Nov 2022 19:17:52 GMT  
		Size: 2.4 MB (2387882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8d479fa2d2c6c503cc8ea2b4deb0b6c5af2ff6a58b3a48ec94346053a5f4de`  
		Last Modified: Wed, 02 Nov 2022 19:17:49 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c2e50062f28f25572934e1354be67087ba900f512bdaad143946434e750a18`  
		Last Modified: Wed, 02 Nov 2022 19:18:31 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba9ea9acad2d162a2570367cc2f21af52c0b3e528d239dd2d8af13c327724ad`  
		Last Modified: Wed, 02 Nov 2022 19:18:49 GMT  
		Size: 72.5 MB (72480320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bd098559b30b498d64f7740fcf0fe3bdd0372711b2d118558adf7b2cc0f7a9`  
		Last Modified: Wed, 02 Nov 2022 19:18:31 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7613b448a79282dac8e97b54a740faeda580f7c7410e3ddaef69d39f3f1e995a`  
		Last Modified: Wed, 02 Nov 2022 19:18:31 GMT  
		Size: 7.1 KB (7051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; s390x

```console
$ docker pull mariadb@sha256:18498ac00e522618f92dc59b38e9e956ceecbbdd98523c622dd07f0c13d83c2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105142329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba90c3535e8905fd0a9e8b72aa707eafe97c2d0ee6d23f3142013b50b8860e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Wed, 02 Nov 2022 18:42:26 GMT
ADD file:0b95c08f7bfd486b0e82a12f0bc21062e9ae48f030f076c8e069bdeb00455043 in / 
# Wed, 02 Nov 2022 18:42:30 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:26:27 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 02 Nov 2022 19:26:37 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:26:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Nov 2022 19:26:51 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Nov 2022 19:26:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Nov 2022 19:27:01 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 19:27:02 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 02 Nov 2022 19:27:04 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Wed, 02 Nov 2022 19:27:59 GMT
ARG MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 19:27:59 GMT
ENV MARIADB_VERSION=1:10.9.3+maria~ubu2204
# Wed, 02 Nov 2022 19:27:59 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
# Wed, 02 Nov 2022 19:28:00 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 02 Nov 2022 19:28:30 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.9.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Wed, 02 Nov 2022 19:28:35 GMT
VOLUME [/var/lib/mysql]
# Wed, 02 Nov 2022 19:28:35 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Wed, 02 Nov 2022 19:28:35 GMT
COPY file:2a785aba6c73dfab59047fdbb26917b1ca4aa8f73ea780e92ea0891a1e9918df in /usr/local/bin/ 
# Wed, 02 Nov 2022 19:28:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Nov 2022 19:28:36 GMT
EXPOSE 3306
# Wed, 02 Nov 2022 19:28:36 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:eafd4874fb95ca754b4f86ad490a07439fba0dbde1b416c882494a56e25e92e1`  
		Last Modified: Wed, 02 Nov 2022 18:44:00 GMT  
		Size: 28.6 MB (28640756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bea011dce2c7655ef5645f35951603af4d860c6c6653b26c7670e0f6b1da9ea`  
		Last Modified: Wed, 02 Nov 2022 19:31:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d6923a043a793e468e7adb84dfe8e59e498c7ec421a7a5d045563d0f55c5f6`  
		Last Modified: Wed, 02 Nov 2022 19:31:12 GMT  
		Size: 3.7 MB (3675116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e572fb6172341fddd1f6b3353620c959e02c6e91878c938ba0b3cb37672fb664`  
		Last Modified: Wed, 02 Nov 2022 19:31:07 GMT  
		Size: 2.0 MB (1956780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c36a3af33b545e0f76f6ac57ea341b57bd51c189de6bb09d0946fcc20ffc648`  
		Last Modified: Wed, 02 Nov 2022 19:31:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e562694e4f06ec88fbe8e579c9ca66a2f205012812ce19ea9d11d4eb2615a7`  
		Last Modified: Wed, 02 Nov 2022 19:31:07 GMT  
		Size: 2.2 MB (2199313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db891bdac11eb4ad276dce571884d2ceead2b0c4a1630b7323ede0719364336b`  
		Last Modified: Wed, 02 Nov 2022 19:31:05 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89802ca4242938a62ea9e93dcc84679d6208be5a8ef8a7dbf368c196ddafc596`  
		Last Modified: Wed, 02 Nov 2022 19:31:30 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b10a0c4c56eda5ee314ee192394ab23400a90fcf6536a7fa5eec78854ac46a`  
		Last Modified: Wed, 02 Nov 2022 19:31:40 GMT  
		Size: 68.7 MB (68655104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b25788d86165ab3008742f36bd0cd6bfb36679d1928144085e0b200ae38a9d`  
		Last Modified: Wed, 02 Nov 2022 19:31:30 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa4f3538ccb9ee39af5e436a70e5c49fcb1724dead6cb95f3c0aa7942a62c12`  
		Last Modified: Wed, 02 Nov 2022 19:31:30 GMT  
		Size: 7.1 KB (7051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
