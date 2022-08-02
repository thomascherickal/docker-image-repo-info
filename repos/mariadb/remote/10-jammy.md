## `mariadb:10-jammy`

```console
$ docker pull mariadb@sha256:b5a7be78e2e4d2ea379ae02dccea34c5870295a251fa16f739ce28219a07d8d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:10-jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:483a080b5bcdf0a898ef4574209080f7a42896c7134c60c55b4d4cb5ab3a8d6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123859860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea81af801379dae14e596b55612f355a63cfca2ed53cf27d047340f4890cf25c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:25 GMT
ADD file:11157b07dde10107f3f6f2b892c869ea83868475d5825167b5f466a7e410eb05 in / 
# Mon, 06 Jun 2022 22:21:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:40:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 07 Jun 2022 00:40:56 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:40:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 07 Jun 2022 00:41:06 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 07 Jun 2022 00:41:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 07 Jun 2022 00:41:13 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:41:13 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 07 Jun 2022 00:41:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 07 Jun 2022 00:42:02 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 07 Jun 2022 00:42:03 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 07 Jun 2022 00:42:03 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 07 Jun 2022 00:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 07 Jun 2022 00:42:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 07 Jun 2022 00:42:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 07 Jun 2022 00:42:23 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 00:42:23 GMT
EXPOSE 3306
# Tue, 07 Jun 2022 00:42:23 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:405f018f9d1d0f351c196b841a7c7f226fb8ea448acd6339a9ed8741600275a2`  
		Last Modified: Wed, 01 Jun 2022 03:03:39 GMT  
		Size: 30.4 MB (30423715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a85079b8234f1744aeed618170b84c2f6b970a320e10616ff031d3be24b5cd4`  
		Last Modified: Tue, 07 Jun 2022 00:47:43 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c7ff691b1abc2640eb61104ca92a223103daf11214a248cc580163536e70d`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 3.8 MB (3765124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976663b5d6daa78634cc56c60cb837f47e79832759e9bdb8f1c592b194411bf`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.0 MB (1991845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169024b1fb136785c2ed5f758e9707ce456f38d8007d568f863be47b0873afd7`  
		Last Modified: Tue, 07 Jun 2022 00:47:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ffe8ce897f6bfdab5ac2fa06b95c2a6187161ced620b3b00e71b31e7b75e47`  
		Last Modified: Tue, 07 Jun 2022 00:47:42 GMT  
		Size: 2.3 MB (2297483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b583c09d23c314a64c34258bda89aaefc6c4b3a488297892863af1dd61bb4113`  
		Last Modified: Tue, 07 Jun 2022 00:47:39 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9f0c08d08f4ae53297606d8c0aea35c96566d2e544a8a32efb72eebc3749b6`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd51f98458654de3ea7c535ee562e9f9251fd6a0818629346bcadaaa768b71a`  
		Last Modified: Tue, 07 Jun 2022 00:48:20 GMT  
		Size: 85.4 MB (85366786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f506bb8acafbb672f41df13b1d99173b9217140c8137ecc9daec14c4e00f70`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d689f79ba4ea066cd24d5c7f7ae294a524fc166bb7f9e8b60d48472f35277a`  
		Last Modified: Tue, 07 Jun 2022 00:48:08 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b6764b02b5eb8d6274207dbb827317cafc8694c1505185aa092d5551f8a793f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104543896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc004eed0c26ad5c4e0d75baff2cb4e7fdc144f713d053c256f6455b608d280`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Mon, 23 May 2022 18:40:14 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Mon, 23 May 2022 18:40:25 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:26 GMT
ENV GOSU_VERSION=1.14
# Mon, 23 May 2022 18:40:43 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 18:40:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 18:40:53 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 18:40:53 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Mon, 23 May 2022 18:40:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Mon, 23 May 2022 18:41:40 GMT
ARG MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:41 GMT
ENV MARIADB_MAJOR=10.8
# Mon, 23 May 2022 18:41:42 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:43 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Mon, 23 May 2022 18:41:44 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Mon, 23 May 2022 18:41:45 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 23 May 2022 18:42:03 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Mon, 23 May 2022 18:42:04 GMT
VOLUME [/var/lib/mysql]
# Mon, 23 May 2022 18:42:06 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Mon, 23 May 2022 18:42:07 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Mon, 23 May 2022 18:42:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 18:42:08 GMT
EXPOSE 3306
# Mon, 23 May 2022 18:42:09 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ae07faadba444656d4d080edc85dcaba97c3ac8f3ac415b136c2add7ff5393`  
		Last Modified: Mon, 23 May 2022 18:47:26 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46428e702eff2922592a3c96fbe5e3764cbca14a5a770718e36a51ad4c9dc906`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 3.6 MB (3592731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e775e0ed5a0037f1c4cce3ef74f7025c80ec7e27e1e60a27c1f39d53e944c75`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 4.0 MB (4014468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031c54d0d9d9d4a999c13ba6733390868914e2c9c66b3ee2feb98e2a93de5d99`  
		Last Modified: Mon, 23 May 2022 18:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602265dc68e116e160f1e4da3863e9ff8313798a78e0d68554915d7cb1d970b9`  
		Last Modified: Mon, 23 May 2022 18:47:25 GMT  
		Size: 2.2 MB (2210433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1d131fb6cb45f460fd0eb002edad2f1273dd1d769fff5ad071a2356a239edc`  
		Last Modified: Mon, 23 May 2022 18:47:22 GMT  
		Size: 2.5 KB (2470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33ea1b30434b058f9b0ea3af9c9638014b6e11714eaa4888fceb806344fe49`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539c6148f07eaa2bb03fae3339771575a22824c8b4d9a6ab5cc10210d114a0c`  
		Last Modified: Mon, 23 May 2022 18:48:01 GMT  
		Size: 66.3 MB (66334981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38aa29868643c4f4f19f60129f5a981a1b09518e1621b1ffdcdf6f06c8261231`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 3.5 KB (3492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3702214dffba8174c27ba1d8d97eebb416c8b984871b3a18b8c497c26b227a77`  
		Last Modified: Mon, 23 May 2022 18:47:50 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4b3ef291e3c387bcd0cdfc34cddde6d9fc9f676a88bcc43d46758dd542ab1f82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (117033413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59318f716fe31444e3f77ff33eb1c8c7449ad201b43a82a5360170452ac4479`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:49 GMT
ADD file:62ec907c651e833838867bd541cf824f5f609ea4e2b19c4b26cec74a57b60470 in / 
# Tue, 07 Jun 2022 05:46:54 GMT
CMD ["bash"]
# Fri, 29 Jul 2022 15:52:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 29 Jul 2022 15:53:07 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 15:53:08 GMT
ENV GOSU_VERSION=1.14
# Fri, 29 Jul 2022 15:53:28 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 29 Jul 2022 15:53:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jul 2022 15:53:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 15:53:44 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 29 Jul 2022 15:53:46 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Fri, 29 Jul 2022 15:55:07 GMT
ARG MARIADB_MAJOR=10.8
# Fri, 29 Jul 2022 15:55:07 GMT
ENV MARIADB_MAJOR=10.8
# Fri, 29 Jul 2022 15:55:07 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Fri, 29 Jul 2022 15:55:08 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Fri, 29 Jul 2022 15:55:08 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Fri, 29 Jul 2022 15:55:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 29 Jul 2022 15:55:48 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Fri, 29 Jul 2022 15:55:51 GMT
VOLUME [/var/lib/mysql]
# Fri, 29 Jul 2022 15:55:51 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Fri, 29 Jul 2022 15:55:52 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Fri, 29 Jul 2022 15:55:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jul 2022 15:55:52 GMT
EXPOSE 3306
# Fri, 29 Jul 2022 15:55:52 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b851cfa9fcbcb74629241502e21ebbae255fe40a2f26949573f278672b65c308`  
		Last Modified: Tue, 07 Jun 2022 05:49:53 GMT  
		Size: 35.7 MB (35717509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83c9f12c8befc3a9f9f7508d55ae427024a847b91a6da6d31a17a61f292596a`  
		Last Modified: Fri, 29 Jul 2022 16:06:43 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ae77d5d9a70753c47546506981c448a3064527bf5433a78fe47a81e6c82ede`  
		Last Modified: Fri, 29 Jul 2022 16:06:41 GMT  
		Size: 4.7 MB (4695004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc2141a8b58617341e722a340ff2804b81f3f72870b47f78c7b05d9be1dec1c`  
		Last Modified: Fri, 29 Jul 2022 16:06:40 GMT  
		Size: 1.9 MB (1921148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c7cc34594b8f62e8bcd71c291a7bc3295fd015e27a85578acf8bb43faf30dc`  
		Last Modified: Fri, 29 Jul 2022 16:06:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50987474c15ab1204d0593376fcd19230d56893befca9ead4f628b9191fb2001`  
		Last Modified: Fri, 29 Jul 2022 16:06:40 GMT  
		Size: 2.4 MB (2404180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3bfb7ebbf6cd97da4feb539afca5dbae350ec4d6a978a08a1359cd65811c25`  
		Last Modified: Fri, 29 Jul 2022 16:06:37 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a779227467a6dbd449eae30c1967efa4b10fce09ea5bb32b8693f0c96791ba`  
		Last Modified: Fri, 29 Jul 2022 16:07:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a514903849123decd7eb49c864e07df6a0d4ae1a90c488cbcab7f1990e339a04`  
		Last Modified: Fri, 29 Jul 2022 16:07:36 GMT  
		Size: 72.3 MB (72280659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac38737a039ea43eb40392c485d7382a110e4a69b3ae52238f01921ee97f61e`  
		Last Modified: Fri, 29 Jul 2022 16:07:18 GMT  
		Size: 3.5 KB (3494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9008c24f99313b6d6970ec168501e451beadf253cbd7e0ae0cf103d76bbc5e19`  
		Last Modified: Fri, 29 Jul 2022 16:07:18 GMT  
		Size: 6.7 KB (6700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:12097ab474fe2ee789b394e1e8a6b489f2ca4ce5ebc8904a14cfddeedb17b8e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104979316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95792c9ef5a984b01f32025b66c1495e316d034e94d5975da4069d260d40064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:17 GMT
ADD file:d5a5e56e0ca8287f27b257e3ddbc9675a1bdac1912afbbab6cddd891056cd144 in / 
# Tue, 02 Aug 2022 01:02:19 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:55:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 02 Aug 2022 12:56:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 02 Aug 2022 12:56:16 GMT
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 02 Aug 2022 12:56:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 02 Aug 2022 12:56:22 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:56:22 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 02 Aug 2022 12:56:23 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -fr "$GNUPGHOME"; 	apt-key list
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_MAJOR=10.8
# Tue, 02 Aug 2022 12:57:08 GMT
ARG MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:08 GMT
ENV MARIADB_VERSION=1:10.8.3+maria~jammy
# Tue, 02 Aug 2022 12:57:09 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
# Tue, 02 Aug 2022 12:57:09 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 02 Aug 2022 12:57:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-10.8.3/repo/ubuntu/ jammy main
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	if [ ! -L /etc/mysql/my.cnf ]; then sed -i -e '/includedir/i[mariadb]\nskip-host-cache\nskip-name-resolve\n' /etc/mysql/my.cnf; 	else sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/[mariadbd]\nskip-host-cache\nskip-name-resolve\n\n\2\n\1/}'                 /etc/mysql/mariadb.cnf; fi
# Tue, 02 Aug 2022 12:57:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:03ef406a869fc1d453794e4b0c7e8da3dee6816b3267c63fa57c93b4a38c8c52 in /usr/local/bin/healthcheck.sh 
# Tue, 02 Aug 2022 12:57:38 GMT
COPY file:e4da674ce3a4afd5069ca1fdb1c5969db396f58ba4a9105ee3e377f2391b91c5 in /usr/local/bin/ 
# Tue, 02 Aug 2022 12:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Aug 2022 12:57:39 GMT
EXPOSE 3306
# Tue, 02 Aug 2022 12:57:39 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:f97967c51aac02138b615522a1bab9c75addd5896f43ade17ddaac44e0644283`  
		Last Modified: Tue, 02 Aug 2022 01:03:51 GMT  
		Size: 28.6 MB (28642785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518030038f927b55f39a26dbee5d8d6e8c31cc0ddf7f23268b3dee3f001182c2`  
		Last Modified: Tue, 02 Aug 2022 13:01:03 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5074a746c3e8a07e66d2d76ac4a7b9e0af6ffbf0cc8a87f601bb8b6913662`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 3.7 MB (3675041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6140902b730422bc6cad80b27cf9005104adc5047e2e34955e4fbb5cf7d394`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.0 MB (1955931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67105478e75b1563365dc4986a18198b1230a86bb142ade80fa52d1f71e2b6d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af39a56c0cc78baeec34ac8d7b93879b9b0878bfcc89737ffecf164a865bd46b`  
		Last Modified: Tue, 02 Aug 2022 13:01:02 GMT  
		Size: 2.2 MB (2216654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c8957d63d730d9dbe5d508e565371ce9f1a318e16ad05c720373da4dbbe208`  
		Last Modified: Tue, 02 Aug 2022 13:01:00 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5461cdd4f49c09bdda524801b26ccc244a1f3b4daa635e39c8d982532b8646d7`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c9a941eeee8bd3fcf6d0504466a69f3b30632b6d14fed1f53bc29439ded147`  
		Last Modified: Tue, 02 Aug 2022 13:01:30 GMT  
		Size: 68.5 MB (68473998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7458611c3efeaaf589463cdc0dff355cd54d57b45ece924dd1f1e136b26ef8dc`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 3.5 KB (3493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf3286637af3a581d1537b503e2b8404768d5a37566247553295844ea4b760d`  
		Last Modified: Tue, 02 Aug 2022 13:01:21 GMT  
		Size: 6.7 KB (6699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
